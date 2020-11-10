# HW5: PhotoChat
**SI669 Fall 2020**

## Video Walkthrough
See the [Demo Video](https://youtu.be/izDEgnqXP7g) for an example of what your video should look like.

## Learning Goals
This homework will give you practice working user accounts, realtime updates, Firebase Storage, images, and the Camera.

## Project Goals
The starting point is the chat669 app built in class during weeks 9 and 10, with added functionality to take a photo to share within a chat. Everything is implemented except for the method `DataModel.addChatImage()`, which you will need to complete.

## What to Do
1. Accept the GitHub Classroom invitation.
2. Clone this repo to your local machine.
3. `cd` into the directory that was created when you cloned the repo (it should be called `hw5-photochat-<your-github-id>`).
4. Run `yarn install` to install all dependencies.
5. Integrate a firebase project that you “own” into the app (this can be a project you created previously or a new one).
6. Complete the implementation of `DataModel.addChatImage()`.
7. Create a screencast video and submit the link to Canvas before the deadline.
8. Push your final changes to GitHub before the deadline.

## Video Script
1. Before recording your video, create at least two accounts.
2. Log in using one account (User A).
3. Choose a different person (User B) to chat with.
4. Click the camera button within the Chat screen to take a picture.
5. Send a text message.
    <ol type="a">
    <li>Test Case 1: Text message should display within the chat as having come from the current user (on the right side of the screen).</li>
    </ol>
6. Use the Camera screen to take a picture
7. After returning to the chat screen, wait for the picture to display
    <ol type="a">
    <li>Test Case 2: Photo should display within chat as having come from the current user (on the right side of the screen).</li>
    </ol>
8. Reload the app, log in as the same user (User A), and choose the previously chosen chat partner (User B)
    <ol type="a">
    <li>Test Case 3: Both text message and photo should display in the chat as having come from the current user.</li>
    </ol>
9. Reload the app, log in as the other user (User B). Choose the original user (User A) as the chat partner.
    <ol type="a">
    <li>Test Case 4: Both text message and photo should display in the chat as has having come from the other user (on the left side of the screen).</li>
    </ol>
10. Send a text message and a photo message.
    <ol type="a">
    <li>Test Case 5: Both text message and photo should display in the chat as having come from the current user (on the right side of the screen).</li>
    </ol>
11. Reload the app, log in as the original user (User A), and choose the second user (User B) as the chat partner
    <ol type="a">
    <li>Test Case 6: All photos and text messages should be displayed as coming from the correct users.</li>
    </ol>

## Grading (up to 120 points)
| No. | Requirement  | Points |
| --- | ------------- | ------------- |
| 1 | Test Case 1 | 20 |
| 2 | Test Case 2 | 20 |
| 3 | Test Case 3 | 20 |
| 4 | Test Case 4 | 20 |
| 5 | Test Case 5 | 20 |
| 6 | Test Case 6 | 20 |
|   | **Total** | **120**

## Extra Credit
Implement “unread messages” capability. When a user has “unread messages” in a particular chat, the chat partner’s name should appear in **bold**. See the [Demo Video](https://youtu.be/MG08G-baqyk) for an example.

## Extra Credit Video Script
1. Before recording your video, create at least two accounts.
2. Log in using one account (User A).
3. Choose a different person to chat with (User B).
4. Send a text message
5. Reload the app and log in as User B.
    <ol type="a">
    <li>Test Case 1: User A should appear in bold.</li>
    </ol>
6. Choose User A to navigate to the Chat Screen.
7. Send a text message.
8. Without reloading the app, navigate “back” to the People screen
    <ol type="a">
    <li>Test Case 2: User A should no longer appear in bold.</li>
    </ol>
9. Reload the app and log in as User B again
    <ol type="a">
    <li>Test Case 3: User A should not appear in bold.</li>
    </ol>
10. Reload the app and log in as User A.
    <ol type="a">
    <li>Test Case 4: User B should appear in bold due to the unread message sent in step 7.</li>
    </ol>

## Grading (up to 4 points)
| No. | Requirement  | Points |
| --- | ------------- | ------------- |
| 1 | Test Case 1 | 1 |
| 2 | Test Case 2 | 1 |
| 3 | Test Case 3 | 1 |
| 4 | Test Case 4 | 1 |
|   | **Total** | **4**