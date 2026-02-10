# campus_navigation_and-assistance-appp-using-indoor-loacalization-

# Project Overview
Indoor navigation is difficult because GPS does not work reliably inside buildings.  
This project focuses on estimating a user’s indoor location using Wi-Fi signal strength (RSSI) values and Machine Learning, and using that information to assist campus navigation.
The system predicts the user’s current indoor location based on Wi-Fi fingerprints and provides navigation assistance to reach a selected destination inside the campus.
# Problem Statement
Wi-Fi signals behave unpredictably indoors due to walls, obstacles, and multipath effects.  
New students and visitors often struggle to locate rooms, labs, and departments inside large campus buildings.

This project addresses the problem by using Wi-Fi RSSI-based indoor localization combined with Machine Learning.
# Solution Approach
- Wi-Fi RSSI values from multiple access points are used as input features
- Each indoor area (room/zone) is treated as a location class
- A Machine Learning model predicts the most probable indoor location
- The predicted location is used as the starting point for navigation assistance
# Dataset Description
- Simulated Wi-Fi RSSI dataset representing indoor signal variations
- Features:
  - AP1, AP2, AP3, … AP7 (RSSI values in dBm)
- Target:
  - Indoor Location (Room_A, Room_B, Lab, Library, etc.)
The simulated dataset represents realistic indoor Wi-Fi fingerprinting behavior.
## Machine Learning Model
- Algorithm Used: **K-Nearest Neighbors (KNN)**
- Reason for Selection:
  - Indoor locations with similar RSSI patterns are physically close
  - KNN performs well for Wi-Fi fingerprinting based localization
# Workflow
1. Dataset creation (Wi-Fi RSSI values)
2. Data preprocessing and normalization
3. Feature and label separation
4. Train-test split
5. Model training using KNN
6. Location prediction
7. Accuracy evaluation
# Results
- The trained model successfully predicts indoor locations based on Wi-Fi RSSI patterns
- Achieved reliable localization accuracy under simulated indoor conditions
# Navigation Concept
- The predicted indoor location acts as the starting point
- A logical campus map defines connectivity between rooms
- Navigation guidance is provided step-by-step to the selected destination
# Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Google Colab
- Machine Learning (Classification)
# Applications
- Campus navigation for students and visitors
- Indoor guidance during events or examinations
- Accessibility assistance for visually impaired users
- Extension to hospitals, malls, and office building
# Future Scope
- Real-time Wi-Fi signal collection using mobile devices
- Integration with mobile or web applications
- Bluetooth beacon or IoT sensor fusion
- Deep Learning models for improved accuracy
- Voice-based navigation assistance

## Author
Sharanya Bolem
