# Predicting Stress and Relapse Using Computer Vision
Research project exploring whether multimodal (vision + language) signals can predict high-stress 
or relapse-relevant states in video data, using facial/gaze features and LLM-based linguistic markers.



— Project Framework — 

The VLM & Eye-Tracking Execution:
- Use a lightweight, open-source model like OpenFace or a specialized Vision-Language Model (VLM) like LLaVA to extract features from each static image
- OpenFace can automatically detect eye-gaze direction, facial landmarks, and Action Unit intensities per image, converting each PNG into a clean numerical feature vector

Classification:
- Combine the extracted facial features (gaze direction, AU intensities, expression markers) across images to see if a simple machine learning classifier (like a Random Forest or gradient boosting model) can accurately predict stress-relevant expression states from a single photo
