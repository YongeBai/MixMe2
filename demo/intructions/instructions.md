
# Target Project: MixMe
You are building a web application called MixMe, that allows users to upload a video of a basketball game, and create a highlight reel by selecting the player they want to highlight. The user will select the player and the ball and the model will extract the frames where the player and the ball are within X pixels distance from each other. The user can then select the clips they want to add to their highlight reel and download the highlight reel.

You will be using the same tech stack as the template:
Backend:
- python
- flask
- strawberry
- sam 2
- And any other libraries used in the template

Frontend:
- react
- typescript
- graphql
- tailwind
- And any other libraries used in the template

Technical pipeline
There are 2 nouns in this project:

User (the person using the app)

The player/s (the people in the video) So when there is a reference to a "player", it refers to the player or players in the video. When there is a reference to "the user" it refers to the person using the app.

From the user's point of view they will preform the following steps:

1. Upload a video of a basketball or soccer game.
2. Select the player they want to highlight and the ball
3. The SAM 2 model will extract the frames where the player and the ball are within X pixels distance from each other, then create clips from the extracted frames
4. The user will be able to preview the clips the model detected as relating to the players they selected
5. The user will be able to select the clips they want to add to their highlight reel
6. The user will be able to download their highlight reel


# Template
You are given a template that will be used as a starting point for the project. The template contains a frontend and backend setup. But also contains several features that need to be removed as they are not needed for MixMe the project explanined above. There are also several features lacking that will need to be added.

Here is a list of some key features that we will need to keep:
- The ability to upload a video
- The ability to select objects as the user skips through the video

Here is a list of features that need to be removed:
- The default video, there should be no video by default
- The option to select multiple object, please only allow the user to select one player and one ball. By actively prompting the user to select only one player and one ball.
- The Gallery section, this should be removed. 
- The entire "Add effects" section, this should be removed. 
- The limit of "Max 70MB" for the video upload, we want to remove this limit.

Here is a list of features that need to be added:
- The entire clip selection and preview section, this should be built. We will keep the same UI as the template. After the user select the player and the ball, hit the "Next" button to see the clips detected by the model. This will show the clips in a verticall scrollable grid, when the user hovers over a clip it will show a play button, when the user clicks on a clip it will show a preview of the clip. In the main video player where they used to select the player and the ball, there will now be a "Done selecting clips" button. Once the user clicks on it, the highlight reel will be created and the user will be able to download it.
- The creation of the highlight reel, this should be built.
- The download of the highlight reel, this should be built.