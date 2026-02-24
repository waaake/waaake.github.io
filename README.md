[<img src="images/hey_vivek.png" width="1000"/>](images/hey_vivek.png)

### Hey, I'm Vivek👋

Nice to meet you! I'm a software developer working in VFX technology. I spend my time building tools, pipelines and systems that make the creative workflows better and faster. Performance and efficiency are the things I really care about.

I'm intrested in VFX and gaming industry, especially in Graphics programming. The math behind rendering each frame (pixels and voxels) excites me and keeps me curious to learn more.
Before moving into software development, I worked on the creative side of VFX, animating 3D characters. That experience helps me understand the creaive vision behind projects, making me better at designing technical systems that support creative teams.


# Where I've been building and creating

## Senior Pipeline Developer
### Redefine: Originals, Hyderabad
#### (May 2025 - Present)

> - Started with a backend service to maintain realtime sync between the various production management systems in-house. <br>
>   We were dealing with multiple in-house production management systems to make the pipeline experience better for the artists working. This demanded a real time sync of information accross all the PMS systems, publishes being tracked from the artists side and pushed over to the production and status updates, new ingested shots, feedbacks from the creative supervisors and production to the artists. <br><br>
> - Provided a prototype for a solution that was being discussed to target a look required for a specific show. <br>
>   One of the noted problems with unreal engine's original hair shading model was that even with specular field set to 0, it still has a bit of highlight across other lobes. To tackle this, created another hair shading model based off (copy of) the existing hair shading model but with custom data enabled and also by updating the existing shader to work with additional input of Specular Strength and push that via the GBuffer to be used as a multiplier to the existing Specular value, this gave fine grain control from the UE material graph to the creatives who want to tinker around with it and set the overall look. <br>
>   Not only this was challenging, but at the same time helped me get a few more insights of how the shading in Unreal Engine works. <br><br>
> - One of the other problems that I was able to deal with was with Unreal's asset locking, which means if unreal has an asset open (in Windows) it's locked and cannot be updated. <br>
>   The use case for the team was to publish and retrive the updated assets which were pushed into perforce for the various content plugins used across the shows, since Unreal locks entities being used, hence the publish process had to wait for everyone to close their unreal sessions for a fair amount of time till the publish/update process is finished. This bottleneck was solved with a simple yet meaningful approach of having reading mirror for the artists in Unreal for the content plugins. Next to the published content plugins, we added a cached clone of the existing content plugins. This allowd the artists to seamlessly work in unreal without having to worry about the publishes and updates happening to the content plugins. It is when the resources are idle, the backend service aspect of this system syncs the updates to the cached plugins directory so that the artists can continue to get the latest of the plugins, with just a minor restart on Unreal.

## Senior Software Developer
### Moving Picture Company, Bangalore
#### (July 2023 - February 2025)

> - Developed an end-to-end updated rendering architecture for streamlining the compositing render workflow. <br> This system was based on the nuke dcc's render commandline and was coupled with the Pixar's tractor engine to provide a farm based rendering solution for the team. The system also had the option to render locally via a custom Queue mechanism with a dedicated user interface, which tracked the render and release processes and also gave the users flexibility to stop a process or retry in case the process failed. <br><br>
> - As a studio, the team wanted to use the latest and greatest of DCCs, Nuke being one of them. <br>The main problem to tackle before moving to the updated VFX reference platform was to ensure all of the required dependencies of the Nuke stack is all compliant with the requirements, and them being python 3, OpenEXR 3.x and updated Qt version compatibility. The first migration to CY 2022 platform was relatively difficult than the second migration for CY 2024 platform as the former one needed to ensure all dependent projects are python 3 migrated and also OpenEXR 3.x compatible. Being part of the lager effort and contributing to many different projects helped me gain a wider insight around many other departments' workflows.<br><br>
> - Visual programming is one of the aspects which intrigues everyone, including the creatives. <br>This was driven by an agenda to describe and configure workflows for shows in a way that's managed through visual node graph. This allows the creatives to have more control over the workflows without having to worry about programming knowledge for config files.<br>I was involved in the early protyping of the workflow to demonstrate the feasibility of the approach and also help decide the platform on which the visual scripting should happen.<br>There were many platforms explored for this, e.g Houdini PDG, Alicevision Meshroom, Inbibo Shift and few other thirdparty applications. In the end, the decision was to go with Meshroom. Having done the initial POC, I moved to the Meshroom development as the platform for the Node based workflow system, targeted for the BU technical directors to create and provide nodes and creative supervisors to configure workflows.

### Software Developer

> Moving Picture Company, Bangalore (July 2021 - June 2023)
>
>> - Developed a Conform ingest workflow for Editorial using Foundry hiero. 
>> - This process extended hiero’s conform functionality and connected the data exporter to the in-house AMS system. 
>>


### Junior Software Developer

| Moving Picture Company, Bangalore (November 2020 - June 2021)                                                                                             |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| - Developed a set of custom Nuke nodes to connect to the in-house AMS suite. <br> - Developed a toolset to automate ingesting internal cross-BU 2d turnovers (including elements and grades) into the Asset Management System. <br> - Extended a photoshop plugin to export the layers as separated tiff images. |



<div align="right">

### Matchmove & RotoAnim Artist | Technical Artist

| Moving Picture Company, Bangalore (June 2016 - October 2020)                                                                                                                         |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| - Worked on feature films such as Ghost in the Shell, Jumanji, Alien: Covenant, Fantastic Beasts, Mummy. <br> - Led the team on Cats project focusing on Roto-animation tasks. <br> - Developed few toolsets for Maya (Multiview Playblast, Anim IO – animCurves) helping the artists to deliver shots quickly.

</div>

<!-- 
Vivek here - a Software Developer working in VFX technology.
I spend my time building tools, pipelines and systems to make the creative workflows faster (performance-enthusiastic). -->

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vivek-vrma/)
[![Email](https://img.shields.io/badge/Outlook-white?style=for-the-badge&logo=microsoft-outlook&logoColor=0078D4)](mailto:vivek_ve@outlook.com) 

### I Geek out on...
- Managing memory efficiently
- SIMD (speeeeeeed matters over everything!!)
- Game Engines (especially their architectures and the performance they squeeze out)
- Prince of Persia which was written entirely in assembly.

### Nightmares for me?
- My program running slower
- My least favourite is the Memory leaks (the silent types)

### What I'm playing with right now?
- Writing an actual "Player", a high performance media player and a growing review system.
- Learning to encode-decode the audio and video streams for fast and efficient playback.

### Tech I work with
- VFX tools and pipelines, including Nuke and Maya as the digital content creators.
- Exploring Unreal Engine too.
- Frameworks: Qt, OpenGL, OpenImageIO
- Tools: Docker

### On the Programming side
- Decent with: C++, Python
- Familiar with: QML, Javascript

### Next up on My List...
- Vulkan swapchains
- Exploring Assembly language

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
