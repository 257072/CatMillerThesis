📱 MindAR Image Tracking with Audio Playback

This is a simple Augmented Reality (AR) web app built using A-Frame and MindAR, designed to play a specific audio clip when an image target is detected by your device's camera.
🧠 What It Does

    You press a Start AR button to begin the experience.

    Your camera opens and starts scanning for one of 10 pre-defined images (called "targets").

    When the camera recognizes one of these images, it will:

        Play a matching audio file (e.g., target 0 triggers audio0.mp3).

        Stop any other audio that might already be playing.

    When the image is no longer visible, the audio stops and resets.

    For example: Imagine pointing your phone camera at a postcard. When it’s recognized, it plays a message or sound related to that postcard. When you move the postcard out of view, the sound stops.

🔧 How It Works (Simplified)
Technologies Used

    A-Frame: A web framework for building 3D/VR/AR in the browser using HTML.

    MindAR: An image tracking AR engine that works with A-Frame.

    HTML & JavaScript: For setting up the scene and controlling behavior.

Key Features

    ✅ 10 image targets (target-0 to target-9)

    ✅ 10 matching audio files (audio0.mp3 to audio9.mp3)

    ✅ Only one audio plays at a time

    ✅ Audio automatically stops when the image is lost

    ✅ Works in mobile and desktop browsers (requires camera access)

🚀 How to Use

    Host this project on a server (can be local or on the web).

    Make sure your device has a camera and allows camera permissions.

    Click the "Start AR" button.

    Point your camera at one of the image targets (as defined in targets.mind).

    Enjoy the matching audio playback when the target is found!

🗂 Folder Structure

project/
│
├── index.html              # Main AR app code
├── targets.mind            # File defining the 10 image targets
└── audio/
    ├── audio0.mp3
    ├── audio1.mp3
    ├── ...
    └── audio9.mp3

📝 Notes

    Audio playback may require user interaction (especially on iOS), which is why there’s a Start AR button to trigger it.

    The targets.mind file must be created using the [MindAR image compiler tool](https://hiukim.github.io/mind-ar-js-doc/tools/compile) and should include 10 image targets.

👀 Example Use Cases

    AR audio guide for a gallery or museum.

    Flashcards for language learners with spoken pronunciation.

    Audio storytelling for books, flyers, or posters.

📋 Credits

    Built with MindAR

    3D rendering via A-Frame

    Audio handling using standard HTML5 <audio> and JavaScript