## Explanation
This notebook integrates face recognition with mood detection using Python and OpenCV. The face recognition algorithm used is based on LBPH (Local Binary Patterns Histograms), which was previously used in our face recognition group activity and I simply modified it to include mood detection.

### Techniques Used
1. **LBPH Face Recognition Algorithm**: The LBPH algorithm is used for face recognition. It compares local binary patterns of pixels in images to recognize faces.

2. **DeepFace for Mood Detection**: DeepFace, a facial analysis library, is used for mood detection. It analyzes facial expressions to detect emotions such as happiness, sadness, anger, surprise, fear, disgust, and neutral.

### Encountered Problems
1. **TensorFlow and Keras Compatibility**: DeepFace works best with TensorFlow and Keras v2.15.0. However, there were compatibility issues with my TensorFlow module, likely due to frequent downgrading and upgrading. This led to a corrupted TensorFlow module, so I had to uninstall and reinstall it.

2. **Missing "Confused" Mood**: While DeepFace detects a range of emotions, including happiness, sadness, anger, surprise, fear, disgust, and neutral, it does not include a "confused" mood in its list of recognized emotions.
