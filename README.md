# 🌿 GreenGuardian Plant Disease Detection App

GreenGuardian is a Flutter application designed to help users identify plant diseases by scanning images of leaves taken from a mobile camera or from the device's storage. The app utilizes the Haar Cascade algorithm for image processing and disease detection.

## Features

- **📸 Image Capture:** Users can capture images of plant leaves using their mobile camera directly from within the app.
- **🖼️ Image Selection:** Alternatively, users can choose images from their device's storage for analysis.
- **🔍 Disease Detection:** The app uses the Haar Cascade algorithm to detect diseases present in the scanned leaf images.
- **📋 Results Display:** Detected diseases are displayed to the user along with relevant information such as possible causes and suggested remedies.
- **📢 User Feedback:** Users can provide feedback on the accuracy of disease detection, helping to improve the app's performance over time.

## 🎥 Video Demo
[![Watch the video](https://raw.githubusercontent.com/username/repository/branch/path/to/thumbnail.jpg)](https://raw.githubusercontent.com/kaustubhr7/GreenGuardian-Plant_Disease_Doctor/main/Demo/Plant Diease Detection DEMO Video (with Code).mkv)

## Installation

To use GreenGuardian, follow these steps:

1. Clone this repository to your local machine.
2. Ensure you have Flutter installed. For installation instructions, refer to the [Flutter documentation](https://flutter.dev/docs/get-started/install).
3. Navigate to the project directory and run `flutter pub get` to install dependencies.
4. Connect your mobile device or set up an emulator.
5. Run `flutter run` to launch the app on your device or emulator.

## Usage

Once installed, follow these steps to use the GreenGuardian app:

1. Launch the app on your mobile device.
2. Choose whether to capture an image using the camera or select an image from your device's storage.
3. After selecting an image, the app will process it using the Haar Cascade algorithm to detect any plant diseases present.
4. View the results displayed on the screen, including detected diseases and related information.
5. Provide feedback on the accuracy of the detection if desired.

## Haar Cascade Algorithm

The Haar Cascade algorithm is a machine learning-based approach used for object detection in images. It works by converting the input image to grayscale and then applying a series of operations to identify specific patterns or features within the image.

### How it Works

1. **Feature Selection:** Haar-like features, which are essentially rectangular filters, are used to detect edges, lines, and textures in the image.

2. **Integral Image:** To efficiently compute the features, an integral image is calculated from the original grayscale image. This allows for rapid computation of pixel sums within any rectangular region of the image.

3. **Adaboost Training:** The algorithm uses a machine learning technique called Adaboost to select a small number of important features out of a large set of potential features. These selected features are then combined to form a strong classifier.

4. **Cascade Classifier:** The strong classifier is constructed as a cascade of weak classifiers, each of which focuses on a specific aspect of the object being detected. This cascade structure allows for efficient processing by quickly rejecting regions of the image that are unlikely to contain the object.

5. **Sliding Window Detection:** The trained cascade classifier is applied to the input image using a sliding window approach. The classifier is moved across the image, evaluating each subregion to determine whether it contains the object of interest.

6. **Thresholding and Detection:** Each subregion is evaluated based on a threshold, and if it passes, it is classified as containing the object. This process is repeated at multiple scales to detect objects of different sizes within the image.

In the case of GreenGuardian, the Haar Cascade algorithm is trained to recognize patterns associated with various plant diseases, allowing the app to accurately detect and diagnose diseases based on input leaf images.

The Haar Cascade algorithm, commonly used in object detection tasks, works by converting the input image to grayscale and then applying a series of operations to identify specific patterns or features within the image. These features are typically rectangles of varying sizes and positions.

The algorithm assigns a binary number to each pixel in the image based on whether it meets certain criteria defined by the patterns being detected. This binary representation is then used to analyze the image and identify regions that match the desired patterns.

In the case of GreenGuardian, the Haar Cascade algorithm is trained to recognize patterns associated with various plant diseases, allowing the app to accurately detect and diagnose diseases based on input leaf images.





## Contributing

Contributions to GreenGuardian are welcome! If you'd like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and ensure that the code follows the project's coding style and conventions.
4. Test your changes thoroughly.
5. Commit your changes with clear and descriptive commit messages.
6. Push your changes to your fork.
7. Submit a pull request to the main repository's `develop` branch.

## Acknowledgements

The GreenGuardian app utilizes the following open-source libraries:

- Flutter: A UI toolkit for building natively compiled applications for mobile, web, and desktop from a single codebase.
- Haar Cascade Algorithm: An efficient object detection algorithm used in computer vision applications.

