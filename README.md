# **Drowsiness Detection System**

## **Overview**

This project detects whether a person in a vehicle is **awake or asleep** using **eye state detection** and also predicts their **age** from facial images. It supports **multiple people detection** in both images and videos.
If someone is detected as sleeping, the system:

* Highlights them with a **red bounding box**.
* Displays their **age**.
* Shows a **popup alert** with the number of sleeping individuals and their ages.

The application comes with a **Graphical User Interface (GUI)** for easy use.
Users can upload an **image or video**, preview the result, and get alerts instantly.


## **Features**

* Detect multiple faces in an image or video.
* Classify each person as **Awake** or **Sleeping** (based on eye state).
* Predict **age** for each detected face.
* Real-time popup alerts for sleeping individuals.
* User-friendly **Tkinter GUI** with options for:

  * **Image Input**
  * **Video Input**
  * **Live Preview**
* Models trained using:

  * **MRL Eye Dataset** (for eye open/closed detection).
  * **UTKFace Dataset** (for age prediction)



**requirements.txt**

```
opencv-python
numpy
matplotlib
scikit-learn
tensorflow>=2.11
keras>=2.11
mtcnn
pillow
```


## **Model Details**

* **Eye Detection Model**: CNN trained on **MRL Eye Dataset**.
* **Age Prediction Model**: CNN regression model trained on **UTKFace Dataset**.
* Performance:

  * Eye Detection Accuracy: **\~95%**
  * Age Prediction MAE: **4-6 years**


## **Outputs**

* Real-time bounding boxes:

  * **Red** → Sleeping
  * **Green** → Awake
* Popup alert showing:


## **Future Improvements**

* Add **yawning detection** for advanced drowsiness analysis.
* Optimize for **real-time video stream**.
* Deploy as a **mobile app** for vehicle dashboards.


