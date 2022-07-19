# video-chat-app
A video calling web app built using webRTC.<br>
(PS: Still in intial stage of development; trying different methods to implement the functionality)

## Setup

- ### Firebase cloud firestore
  - Create `calls` collection.

  - Initialize a new document with `offer` as a map:
     ```js
    offer: {
        sdp: '',
        type: ''
    }
    ```
  - Create `offerCandidates` and `answerCandidates` as subcollections of the `calls` collection.
  - Initialize a new document inside `offerCandidates` and `answerCandidates` with the following fields.
    ```js
    candidate: ''
    sdpMLineIndex: ''
    sdpMid: ''
    ```

- ### Clone this repository
- ### cd `video-chat-app`
- ### Add your firebase config in `main.js`
- ### Save and run `npm run dev`