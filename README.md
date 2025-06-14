# 🚀 Project-ML: Object Identifier & Distance Estimator

Ever wondered how far something is from your camera? Or how far two objects are from each other — all using just a regular webcam?  
This project does exactly that — with a mix of computer vision, math, and a bit of ML magic.

---

## 🧠 What It Does

### 🔍 Part 1: Object Detection  
- Detects multiple object classes using the **COCO dataset**.  
- Outputs bounding boxes **with confidence scores**.  
- Built using **SSD MobileNet** — fast, light, and solid for real-time detection.

🎯 Example:  
Detects things like people, bottles, chairs, etc. in real-time.

---

### 📏 Part 2: Camera-to-Object Distance Estimation  
- Uses **Haar Cascade** (frontal face detection) for face-based distance calibration.  
- Calibrates using an image taken at a known distance (e.g., **30 inches**) to calculate object distance using simple math.  
- Replace `lena.png` with your own calibration image — it's more accurate that way.

🖼️ Reference Diagram:  
![Distance Estimation](https://user-images.githubusercontent.com/75139237/123779777-28037d00-d8f0-11eb-94fc-f344e204eb8f.png)

🎬 Output Preview:
<video src="https://user-images.githubusercontent.com/75139237/123778696-fd64f480-d8ee-11eb-8e1d-39fba3dbdef5.mp4" controls width="100%"></video>

---

### 📐 Part 3: Object-to-Object Distance  
- Calculates the **midpoint** of each detected object’s bounding box.  
- Uses **Euclidean distance** to measure how far two objects are from each other in the frame.

🖼️ Multi-object Example:  
![Multi-object](https://user-images.githubusercontent.com/75139237/123779239-985dce80-d8ef-11eb-9523-df63967d8958.png)

🖼️ Single-object Output:  
![Single-object](https://user-images.githubusercontent.com/75139237/123779352-b4fa0680-d8ef-11eb-84ca-e051562bb19e.png)

🎬 Final Output:
<video src="https://user-images.githubusercontent.com/75139237/123779034-5e8cc800-d8ef-11eb-9d60-da0dc9882615.mp4" controls width="100%"></video>

📸 Final Frame:  
![Final Frame](https://user-images.githubusercontent.com/75139237/123779525-e2df4b00-d8ef-11eb-9364-f041327a39ec.png)

---

## 🛠️ Built With

- **Python**
- **OpenCV**
- **COCO Dataset**
- **Haar Cascade Classifiers**
- **SSD MobileNet**

---

## 💡 Cool Use Cases
- Social distancing tracker  
- Smart surveillance systems  
- AR object placement accuracy  
- Robotics vision applications
