# Sign Language Translation using Gaussian Mixture Models

Real-time ASL alphabet recognition using webcam hand landmarks and Gaussian Mixture Models.

## Pipeline

1. Capture labeled hand-landmark data.
2. Normalize and engineer landmark features.
3. Train a class-conditional GMM.
4. Map GMM components to alphabet classes.
5. Run live webcam inference.

## Tech stack

Python, OpenCV, MediaPipe, NumPy, pandas, scikit-learn, joblib, Gaussian Mixture Models.

## Repository

- `model_sign_language_translator_2.ipynb` - feature processing, PCA, GMM training and evaluation
- `gmm_model.pkl` - trained GMM artifact from the original project
- `ASL_alphabets.xlsx` - landmark dataset used by the training notebook
- Additional notebooks in the original project cover webcam collection and deployment.

## Result

The supplied training notebook records **96.48% accuracy** on its filtered test evaluation.

## Run

```bash
pip install opencv-python mediapipe numpy pandas scikit-learn joblib openpyxl
```

Then open the training notebook in Jupyter or Google Colab.

This project recognizes a predefined alphabet vocabulary rather than continuous sign-language sentences.