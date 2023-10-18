## Google Summer of Code (GSoC'23) Final Report

### Project Title : [Whiteboard Integration](https://github.com/RocketChat/Apps.Whiteboard) 🚀

### Organization : [Rocket.Chat](https://github.com/RocketChat) 🌟

### Mentee : Vinayak Sharma 👨‍💻

### Mentors : Shiqi Mei 🌟 and Douglas Gubert 🌟

### Project Summary
The Whiteboard Integration project enhances collaborative experiences in Rocket.Chat by introducing a powerful Whiteboard App. This integration facilitates real-time visual communication, making it easy for users to create and share diagrams, drawings, and more. With a user-friendly interface and features like slash commands and action buttons, users can effortlessly create and collaborate on whiteboards. The project also offers a convenient local setup guide, allowing users to deploy the app locally for testing. This integration adds a new dimension to communication within Rocket.Chat, fostering creativity and efficient collaboration.

## Live Demo at GSoC 2023 Demo Day 🚀

<p align="center">
  <a href="https://www.youtube.com/watch?v=Z1mx4Of5UjE&t=17s&ab_channel=Rocket.Chat">
    <br><strong>Tap to View the Demo</strong>
  </a>
</p>

## Work Done ✅
### - We can use slash commands or action buttons to start up a new whiteboard.
 [Screencast from 18-10-23 10:43:12 PM IST.webm](https://github.com/CulturalProfessor/Google-Summer-of-Code-23/assets/92238941/1f1304e9-d751-4dce-91f8-f42c3e06c458)

#### - We can store real-time previews of our boards.
[Screencast from 18-10-23 10:46:02 PM IST.webm](https://github.com/CulturalProfessor/Google-Summer-of-Code-23/assets/92238941/994aa494-4fb9-4541-af24-7b154c3fa3d1)

#### - We can store external files like images in our records.
[Screencast from 18-10-23 10:47:17 PM IST.webm](https://github.com/CulturalProfessor/Google-Summer-of-Code-23/assets/92238941/884034b0-20ef-4ae7-b778-6dc60abb122c)

#### - We can modify settings to edit the board name.
[Screencast from 18-10-23 11:05:30 PM IST.webm](https://github.com/CulturalProfessor/Google-Summer-of-Code-23/assets/92238941/e412c362-98c4-4fb6-94af-0ced6dd2d35b)

#### - We can modify the permission system to make the board public/private.
[Screencast from 18-10-23 11:08:36 PM IST.webm](https://github.com/CulturalProfessor/Google-Summer-of-Code-23/assets/92238941/7c332c2d-4c0c-4d04-bab1-834ab0d72da9)


## Architecture of Whiteboard App:
<img src="https://github.com/CulturalProfessor/Google-Summer-of-Code-23/assets/92238941/1f696c03-8cf6-496e-9588-a1fdf11bf04c" width="1000px"></img>

### Code Contributions 💻

<div align="center">

| PR Link   | Description  | Status | 
| :-----------: | :------------------------------------:| :------:|
| [PR #3](https://github.com/RocketChat/Apps.Whiteboard/pull/3) | <b> [FEAT] Initialized Basic commands</b>  | <img src="https://i.imgur.com/tskv8MM.png" width=40 height=35> |
| [PR #4](https://github.com/RocketChat/Apps.Whiteboard/pull/4) | <b> [FEAT] Initialized Webpack Excalidraw build </b>  | <img src="https://i.imgur.com/tskv8MM.png" width=40 height=35> |
| [PR #11](https://github.com/RocketChat/Apps.Whiteboard/pull/11) | <b> [FEAT] Made Preview Block for Board </b>  | <img src="https://i.imgur.com/tskv8MM.png" width=40 height=35> |
| [PR #14](https://github.com/RocketChat/Apps.Whiteboard/pull/14) | <b> [FEAT] Created Whiteboard Action Buttons  </b>  | <img src="https://i.imgur.com/tskv8MM.png" width=40 height=35> |
| [PR #15](https://github.com/RocketChat/Apps.Whiteboard/pull/15) | <b> [FEAT] Excaidraw Source code integration </b>  | <img src="https://i.imgur.com/tskv8MM.png" width=40 height=35> |
| [PR #16](https://github.com/RocketChat/Apps.Whiteboard/pull/16) | <b> [FEAT] Integration Rocket.Chat-apis support in source code  </b>  | <img src="https://i.imgur.com/tskv8MM.png" width=40 height=35> |
| [PR #17](https://github.com/RocketChat/Apps.Whiteboard/pull/17) | <b> [FIX] Stable update for files and boards </b>  | <img src="https://i.imgur.com/tskv8MM.png" width=40 height=35> |
| [PR #18](https://github.com/RocketChat/Apps.Whiteboard/pull/18) | <b> [FEAT] Settings modal </b>  | <img src="https://i.imgur.com/tskv8MM.png" width=40 height=35> |
| [PR #19](https://github.com/RocketChat/Apps.Whiteboard/pull/19) | <b> [FEAT] Permission System </b>  | <img src="https://i.imgur.com/tskv8MM.png" width=40 height=35> |
| [PR #20](https://github.com/RocketChat/Apps.Whiteboard/pull/20) | <b>  [Chore] : Publishing App to Rocket.Chat marketplace </b> |  <img src="https://user-images.githubusercontent.com/70485812/189489748-ed27630f-36e7-4eb9-a9a4-e082d6894490.png" width=40 height=35> |
| [PR #21](https://github.com/RocketChat/Apps.Whiteboard/pull/21) | <b> [Chore] : Integration of Socket.io Source code</b>  |  <img src="https://user-images.githubusercontent.com/70485812/189489748-ed27630f-36e7-4eb9-a9a4-e082d6894490.png" width=40 height=35> |

</div>


## Challenges Faced 🤔
- <b>Iframe Inefficiency</b>: Our initial Iframe approach lacked scalability and flexibility.

- <b>Webpack Transition</b>: Adapting to Webpack for bundling and serving posed technical hurdles and learning curves.

- <b>Real-time Previews</b>: Generating and storing real-time previews in base64 format demanded efficient coding and handling.

- <b>External Files Storage</b>: Managing external files storage added complexity to the project's infrastructure and data handling.

## Future Work 🔮
- <b>Implement Live Collaboration</b>: Enabling live collaboration is a complex task because it involves integrating Excalidraw's collaboration features, which rely on websockets. However, there's a challenge because the Rocket.Chat App's Engine currently doesn't support sockets. The future goal here is to overcome this challenge and find a way to implement live collaboration, allowing multiple users to work on a whiteboard simultaneously and in real-time.

- <b>Implement a Context Bar</b>: To enhance the usability and management of boards, the project aims to implement a Context Bar. This feature will provide a user-friendly interface for users to easily navigate and manage their boards. It could include options to switch between different boards, organize and categorize boards, and access board-specific settings. The goal is to make the user experience more intuitive and efficient when working with multiple whiteboards.

## Acknowledgments 🙌

#### Mentors

-    <b>Shiqi Mei</b> 🚀: Your mentorship and expertise were instrumental in shaping this project. Your guidance steered me through challenges and inspired creative solutions.

-    <b>Douglas Gubert</b>🚀: Your mentorship and dedication to this project were truly remarkable. Your insights and feedback were invaluable in driving progress.

-    <b>Rocket.Chat</b> 🚀: I am grateful to Rocket.Chat for providing me with the opportunity to work on this project. Your commitment to open source and community-driven development is commendable.

#### My Fellow GSoC Participants

-    I'd like to extend my thanks to my fellow GSoC participants who shared their knowledge and experiences. Your camaraderie made this journey even more rewarding.

#### Family and Friends

-    To my family and friends who supported me throughout this endeavor, your encouragement and understanding were my pillars of strength.

#### Open Source Community

-    To the broader open source community, I'm thankful for the wealth of resources and collaborative spirit that enabled me to succeed in this project.

This GSoC journey wouldn't have been possible without the support and encouragement of these individuals and organizations. Thank you all for making this a truly enriching experience.

  
### Connect with Us 🌐

| Mentee: Vinayak Sharma        | Mentor: Shiqi Mei          | Mentor: Douglas Gubert   |
| ----------------------------- | -------------------------- | ------------------------- |
| <img src="https://github.com/CulturalProfessor/Google-Summer-of-Code-23/assets/92238941/7f62da47-5470-4349-8b4b-e7d448d2aadc" width="400px"> | <img src="https://github.com/CulturalProfessor/Google-Summer-of-Code-23/assets/92238941/90aae87f-f67c-4387-aa37-2468bb5124e0" width="400px"> | <img src="https://github.com/CulturalProfessor/Google-Summer-of-Code-23/assets/92238941/5a73b147-4f47-4e13-b1e2-a7cfaafad134" width="400px"> |
| [LinkedIn](https://www.linkedin.com/in/vinayak-sharma-308071225/) | [LinkedIn](https://www.linkedin.com/in/shiqimei/) | [LinkedIn](https://www.linkedin.com/in/douglas-gubert-66798127/) |
| [GitHub](https://github.com/CulturalProfessor) | [GitHub](https://github.com/shiqimei) | [GitHub](https://github.com/d-gubert) |
