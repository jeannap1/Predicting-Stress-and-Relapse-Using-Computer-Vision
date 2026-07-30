# Predicting Stress and Relapse Using Computer Vision
Research project exploring whether multimodal (vision + language) signals can predict high-stress 
or relapse-relevant states in video data, using facial/gaze features and LLM-based linguistic markers.



— Project Framework — 

The VLM & Eye-Tracking Execution: 
- Use a lightweight, open-source model like OpenFace or a specialized Vision-Language Model (VLM) like LLaVA to extract features from the video
- OpenFace can automatically track eye-gaze vectors, facial landmarks, and micro-expressions frame-by-frame, converting video into a clean timeline of numerical data

The LLM & Word Choice Execution: 
- Compile a list of behavioral markers from psychological literature (e.g., specific linguistic indicators of high stress or anxiety)
- Feed transcripts of the text into a smaller open-source LLM (like Llama-3-8B) using structured prompting or sentiment analysis embeddings to flag "high-risk" language patterns.

The Fusion: 
- Combine the visual timeline (eye gaze/stress expressions) and the textual data to see if a simple machine learning classifier (like a Random Forest or an LSTM network) can accurately predict when a speaker is entering a high-stress state.
