1. Crop Recommendation System (Ensemble with Stacking Classifier)
Goal: Recommend a suitable crop based on soil type, previous crop, land area, rainfall frequency, and porosity.
Techniques Used:
Label Encoding, Standard Scaling
Oversampling (RandomOverSampler)
Ensemble Stacking (RandomForest, XGBoost, CatBoost + LogisticRegression)
NLP-based fuzzy matching for user inputs
Key Function: recommend_crop()

2. Disease & Treatment Recommendation System (Voice Input)
Goal: Diagnose disease and recommend pesticide/fertilizer based on voice inputs of crop and symptoms.
Techniques Used:
Label Encoding
Decision Tree Classifier
Speech recognition (speech_recognition)
NLP (fuzzy matching) for converting spoken words to closest dataset terms
Key Function: get_voice_input() + classification logic

3. Fertilizer Recommendation System using Q-Learning (Reinforcement Learning)
Goal: Recommend the best fertilizer using a Q-Learning agent.
Techniques Used:
Custom Q-table with states from soil nutrients and weather data
Reward system based on correctness of predicted fertilizer
Key Function: recommend_fertilizer()

4. Crop Suitability Classification using Neural Network (TensorFlow/Keras)
Goal: Predict crop type based on weather, temperature, soil type, and other agricultural features.
Techniques Used:
Label Encoding and NLP with fuzzy matching
Preprocessing like temperature range conversion
Neural Network model using TensorFlow/Keras
Key Function: Crop suitability model training and prediction

