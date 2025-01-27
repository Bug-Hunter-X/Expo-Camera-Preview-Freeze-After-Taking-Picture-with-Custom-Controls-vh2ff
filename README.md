# Expo Camera Preview Freeze Bug

This repository demonstrates a bug encountered when using the Expo Camera API with custom controls. After capturing an image, the camera preview freezes, requiring a phone restart to resolve.  This issue does not reproduce when using the standard Expo Camera UI components.

## Bug Reproduction

1. Clone this repository.
2. Run `npm install`.
3. Run `expo start`.
4. Take a picture using the custom camera controls.
5. Observe the preview freeze.

## Solution

A solution is provided in `bugSolution.js` which addresses the issue by ensuring proper cleanup of resources after taking a picture.  Specifically, the `onCameraReady` event is used to reset the camera state, preventing the freeze.

## Technologies Used

* Expo
* React Native
* expo-camera

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.