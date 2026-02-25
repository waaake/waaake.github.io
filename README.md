[<img src="images/hey_vivek.png" width="1000"/>](images/hey_vivek.png)

### Hey, I'm Vivek 👋

Nice to meet you! I'm a software developer working in VFX technology. I spend my time building tools, pipelines and systems that make the creative workflows better and faster. Performance and efficiency are the things I really care about.

I'm intrested in VFX and gaming industry, especially in Graphics programming. The math behind rendering each frame (pixels and voxels) excites me and keeps me curious to learn more.
Before moving into software development, I worked on the creative side of VFX, animating 3D characters. That experience helps me understand the creaive vision behind projects, making me better at designing technical systems that support creative teams.

## I Geek out on...
- Managing memory efficiently
- SIMD (speeeeeeed matters over everything!!)
- Game Engines (especially their architectures and the performance they squeeze out)
- Prince of Persia which was written entirely in assembly.

## Nightmares for me?
- My program running slower
- My least favourite is the Memory leaks (the silent types)


# Where I've been building

## Senior Pipeline Developer
### Redefine: Originals, Hyderabad
#### (May 2025 - Present)

> - <h3>Implemented a backend service to maintain realtime sync between the various production management systems in-house. </h3>
>   We were dealing with multiple in-house production management systems to make the pipeline experience better for the artists. This demanded a real time sync of information accross all the PMS systems, publishes being tracked from the artists side and pushed over to the production and status updates, new ingested shots, feedbacks from the creative supervisors and production to the artists. <br>
> - <h3>Prototyped a custom Hair Shading Model in Unreal.</h3>
>   Provided a prototype for a solution that was being discussed to target a look required for a specific show. <br>
>   One of the noted problems with unreal engine's original hair shading model was that even with specular field set to 0, it still has a bit of highlight across other lobes. To tackle this, created another hair shading model based off (copy of) the existing hair shading model but with custom data enabled and also by updating the existing shader to work with additional input of Specular Strength and push that via the GBuffer to be used as a multiplier to the existing Specular value, this gave fine grain control from the UE material graph to the creatives who want to tinker around with it and set the overall look. <br>
>   Not only this was challenging, but at the same time helped me get a few more insights of how the shading in Unreal Engine works. <br>
> - <h3>Implemented a Content plugin Caching system in Unreal for seamless workflows while publishing/updated through perforce</h3>
>   One of the other problems that I was able to deal with was with Unreal's asset locking, which means if unreal has an asset open (in Windows) it's locked and cannot be updated. <br>
>   The use case for the team was to publish and retrive the updated assets which were pushed into perforce for the various content plugins used across the shows, since Unreal locks entities being used, hence the publish process had to wait for everyone to close their unreal sessions for a fair amount of time till the publish/update process is finished. This bottleneck was solved with a simple yet meaningful approach of having reading mirror for the artists in Unreal for the content plugins. Next to the published content plugins, we added a cached clone of the existing content plugins. This allowd the artists to seamlessly work in unreal without having to worry about the publishes and updates happening to the content plugins. It is when the resources are idle, the backend service aspect of this system syncs the updates to the cached plugins directory so that the artists can continue to get the latest of the plugins, with just a minor restart on Unreal.

## Senior Software Developer
### Moving Picture Company, Bangalore
#### (July 2023 - February 2025)

> - <h3>Developed an end-to-end updated rendering architecture for streamlining the compositing render workflow. </h3>
>   This system was based on the nuke dcc's render commandline and was coupled with the Pixar's tractor engine to provide a farm based rendering solution for the team. The system also had the option to render locally via a custom Queue mechanism with a dedicated user interface, which tracked the render and release processes and also gave the users flexibility to stop a process or retry in case the process failed. <br>
> - <h3>Played a part in the overall upgrade towards latest VFX platforms (2022 and 2024)</h3>
>   As a studio, the team wanted to use the latest and greatest of DCCs, Nuke being one of them. <br>The main problem to tackle before moving to the updated VFX reference platform was to ensure all of the required dependencies of the Nuke stack is all compliant with the requirements, and them being python 3, OpenEXR 3.x and updated Qt version compatibility. The first migration to CY 2022 platform was relatively difficult than the second migration for CY 2024 platform as the former one needed to ensure all dependent projects are python 3 migrated and also OpenEXR 3.x compatible. Being part of the lager effort and contributing to many different projects helped me gain a wider insight around many other departments' workflows.<br>
> - <h3>Initial prototyping for Node based Visual scripting system and extending Meshroom as a Platform to support visual scripting</h3>
>   Visual programming is one of the aspects which intrigues everyone, including the creatives. <br>This was driven by an agenda to describe and configure workflows for shows in a way that's managed through visual node graph. This allows the creatives to have more control over the workflows without having to worry about programming knowledge for config files.<br>I was involved in the early protyping of the workflow to demonstrate the feasibility of the approach and also help decide the platform on which the visual scripting should happen.<br>There were many platforms explored for this, e.g Houdini PDG, Alicevision Meshroom, Inbibo Shift and few other thirdparty applications. In the end, the decision was to go with Meshroom. Having done the initial POC, I moved to the Meshroom development as the platform for the Node based workflow system, targeted for the BU technical directors to create and provide nodes and creative supervisors to configure workflows.<br>
> - <h3>Developing and Integrating Compositing templating to the Render System</h3>
>   Was involved in developing a templating system for compositing in Nuke which allows a base template to be created and setup for a show and released. This template then becomes available to be gathered in any context that supports the provided asset names regex, once gathered in Nuke, the asset resolver would find assets with the provided name regex for the current/provided context and resolve the template to released asset and automate the creation of the first version of the slap comp. This was also coupled with the render workflow (as described above) to allow the creatives to create a slap-comp on the fly without even having to open Nuke and do a QC in the in-house Review system. My contributions on this project included the asset resolver backend and the integration with the Rendering architecture. This system had a full-fledged front end UI for Gathering and Release templates at the Show or Sequence level to make them available to all of the child contexts.

## Software Developer
### Moving Picture Company, Bangalore
#### (July 2021 - June 2023)

> - <h3>Developed a Conform Ingest workflow for Editorial to improve the overall ingest experience</h3>
>   Having worked with editors for the past year and maintaining their toolsets for ingesting Grades and supporting on the Client sends, one of key areas of improvments that we saw was that all of the toolsets were separate and there was not much of a relation between them apart from the data being ingested.<br>Though the editors batch those commands but the end-to-end workflow requirements for the editors were never practically met and only after the ingestion of grades and doing a test client send, were they able to see issues with the grades or turnover not matching to what was shared as part of the edit. This caused a lot of delay in communicating early issues with the creative supervisors and the client at times.<br>I was involved in developing a full system for editorial that supports "Conform" process allowing the editors to quickly use the provided edls from client to re-build the entire timeline based on the input turnover. This workflow was developed as an extension to Foundry's Hiero/Nukestudio conform system.<br>This in-house extension allowed the input exr turnover match to the correct sections in the edl by addition of custom conform rules for hiero. I also worked along with the Production Operations and Imaging team to come up with custom Softeffects for the timeline, called as MasterGrade (Ensures linear output followed by the client grade) and MasterReformat (for reformatting to the final edit resolution). The softeffects allow the editor to simultaneously QC the input turnover against the edit through the comparison Viewer buffer of Hiero without having to ingest any of the materials.<br>It is only after a successful initial QC, is when the data ingested into the in-house AMS and PMS systems. Any discrepancies can be flagged at a very early stage.<br>While setting up the system to work with edls received from the client, we discovered that there are many occurances where the edls are not received, so I continued on developing the system further to support building the entire timeline just from the turnover received based on the edit. This workflow started from identifying cuts in the edit and move towards assigning shot numbers to those cuts and then auto-aligning the turnover materials into a multi track layout in the dcc.<br>The other parts of the workflow remained the same for both types of ingest.


## Junior Software Developer
### Moving Picture Company, Bangalore
#### (November 2020 - June 2021)

> - One of the first tools that I worked on was an extension to an already available Photoshop plugin, this was a javascript plugin that allowed the current image to be exported into various formats in an automated manner. The request was to enable layers of the tool to export into .tiff format images with transparency to be used in 3Ddmp department for layering in Nuke.<br><br>
> - There was a lot of data which was being sent over to MPC from other Business Units (within technicolor) for roto and prep work, since this was only required for prep and did not really need a color or reformatting pipeline, it had to be ingested in the pipeline through a simpler process. Part of the problem was to also look at the turnover directory and detect the scene and shot names from the structured path, and validating the pre-populated data from the user before pushing it for ingestion. The second part was to create an ingestion template within nuke to handle all of the provided material based on the camera metadata correctly through correct paths within the Nuke -SwitchNode graph.<br><br>
> - I was also involved in the process of creating an updated suite of Custom Nuke nodes with Qt based knobs to connect to the newer in-house Asset Management System (Tessa). The decision for the Qt based knobs were taken due to the overall modern looking UI that Qt provides over the standard Nuke knobs.


## Matchmove & RotoAnim Artist | Technical Artist
### Moving Picture Company, Bangalore
#### (June 1016 - October 2020)

> - Worked on feature films such as Ghost in the Shell, Jumanji, Alien: Covenant, Fantastic Beasts, Mummy.<br><br>
> - Led the RotoAnim team on Cats project.<br><br>
> - Developed a few toolsets for Maya to help the team deliver shots quickly.
>   - Multiview Playblast
>   - Anim IO - animCurves Exporter/Importer


<!-- 
Vivek here - a Software Developer working in VFX technology.
I spend my time building tools, pipelines and systems to make the creative workflows faster (performance-enthusiastic). -->


### What I'm playing with right now?
- Writing an actual "Player", a high performance media player and a growing review system.
- Learning to encode-decode the audio and video streams for fast and efficient playback.


### Side Projects
- VOID Media player and Review System
- Quickblast (Multi View Playblast tool in Maya)
- Hiddenline wireframe view with Viewport 2.0 in Maya


## Tech I work with
#### VFX & Creative Tools
    - Nuke, Maya, ShotGrid.
    - Recently started exploring Unreal Engine universe too.
#### Frameworks & Libraries
    - Quite decent in working with Qt, OpenGL.
    - Familiar with OpenImageIO and have worked on its uses in a few places.
    - Recently exploring FFmpeg as well.
#### Workflow Tools
    - Docker


### On the Programming side
- I'm quite decent in working with C++ and Python,
- Have some experience and familiarity with QML and Javascript.


### Next up on My List...
- Vulkan swapchains
- Exploring Assembly language


## You can contact me 

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vivek-vrma/)
[![Email](https://img.shields.io/badge/Outlook-white?style=for-the-badge&logo=microsoft-outlook&logoColor=0078D4)](mailto:vivek_ve@outlook.com)

<!--
**waaake/waaake** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
