**Project Description**  
A web application that empowers farmers to diagnose corn leaf diseases from images, track local outbreaks, and forecast disease spread based on upcoming weather conditions.

---

**Key Details**

- **Core Functionality**  
  - **Image‑based Diagnosis:** Upload a photo of a corn leaf to receive an instant prediction of disease type (e.g., Gray Leaf Spot, Northern Leaf Blight, Common Rust) along with confidence scores.  
  - **Local Outbreak Reports:** View community‑submitted predictions in your area, complete with disease type, confidence, predicted spread risk, location, and timestamp.  
  - **Weather‑Driven Forecasting:** Leverage a 15‑day forecast (temperature, humidity, precipitation) via a custom Weather API (built on Open‑Meteo) to flag high‑risk windows for disease propagation.

- **Dataset**  
  - Sourced from the [Maize Leaf Disease Dataset on Kaggle](https://www.kaggle.com/datasets/farmannaim/maizeleaf), containing labeled images of healthy and diseased corn leaves.

- **Machine Learning Model**  
  - **Architecture:** Convolutional Neural Network implemented in TensorFlow/Keras.  
  - **Data Augmentation:** Rotations, flips, zooms, shifts using `ImageDataGenerator`.  
  - **Hyperparameter Tuning:** Hyperband for optimizing learning rate, batch size, and network depth.  
  - **Performance:**  
    - **Training Accuracy:** 96.25%  
    - **Test Accuracy:** 95.70%

- **Tech Stack**  
  - **Frontend:** CSS, HTML, Javascript 
  - **Backend:** Django, Azure, REST API  
  - **Database:** PostgreSQL (user accounts, predictions, reports)  
  - **Deployment:** Docker containers behind Nginx; hosted via Azure

- **User Flow**  
  1. **Register/Login:** Secure account creation with SQL‑backed credentials.  
  2. **Upload Image:** Navigate to the “Predict” page and submit a corn leaf photo.  
  3. **View Results:** See disease prediction, confidence score, and local outbreak map.  
  4. **Forecast Spread:** Check the “Forecast” tab for a 15‑day disease‑risk outlook based on weather.

- **Live Demo & Resources**  
  - **Web App:** https://teamshark.duckdns.org/  
  - **Model Notebook:** Contact me at a.tamimdostyar@gmail.com
  - **Video Walkthrough:** Contact me at a.tamimdostyar@gmail.com
