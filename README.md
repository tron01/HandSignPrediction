# Hand Sign Recognition

This project is a **Hand Sign Recognition System** using MediaPipe's hand tracking capabilities to detect and recognize hand gestures via a webcam.

## Features
- Train the system with custom hand signs.
- Store multiple samples per sign for better recognition accuracy.
- Predict hand signs in real-time based on trained data.

## How It Works
### 1. Training Process
1. Enter a **Hand Sign Name** in the input field.
2. Click **Train Now** to set the hand sign name.
3. Click **Start Training** to begin capturing hand sign samples.
4. Click **Stop Training** when enough samples are captured.
5. Repeat for multiple hand signs.

### 2. Prediction Process
1. Click **Predict** to switch to prediction mode.
2. Show a trained hand sign to the camera.
3. The system compares the detected landmarks with stored samples.
4. The closest match is displayed on the screen.

## Components
### HTML Structure
- Input field for **Hand Sign Name**.
- Buttons for **Train Now, Start Training, Stop Training, Predict**.
- A **canvas** for displaying hand landmarks.
- A hidden **video** element for webcam input.
- A section to display trained hand signs.

### JavaScript Logic
- **Training Mode**: Captures hand landmarks and stores them under the given sign name.
- **Prediction Mode**: Compares detected hand landmarks with stored samples using **Euclidean Distance**.
- **MediaPipe Integration**: Uses MediaPipe's **Hands** API to detect hand keypoints and draw them on a canvas.

## Technologies Used
- **HTML & CSS**: UI structure and styling.
- **JavaScript**: Hand gesture recognition logic.
- **MediaPipe Hands API**: Real-time hand tracking.
- **Bootstrap**: Responsive design.

## Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/tron01/hand-sign-recognition.git
   ```
2. Open `index.html` in a browser.

## Future Improvements
- Implement persistent storage for trained signs.
- Improve recognition accuracy with ML models.
- Add an export/import feature for trained gestures.

## License
This project is open-source and available under the MIT License.
