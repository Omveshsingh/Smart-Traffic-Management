# Smart Traffic Control System 🚦

An intelligent traffic management system that uses computer vision and machine learning to optimize traffic flow at intersections based on real-time vehicle detection.

## 📹 Demo Video

Watch the system in action:

![Smart Traffic Management Demo](SmartRoadTrafficManagementSystem.mp4)

_If video doesn't display, [click here to watch](https://github.com/ayushman12baghel/Smart-Traffic-Control-System/raw/main/SmartRoadTrafficManagementSystem.mp4)_

## 🌟 Features

- **Real-time Vehicle Detection**: Uses YOLOv8 for detecting vehicles (cars, buses, trucks, rickshaws)
- **Dynamic Signal Timing**: Adjusts traffic signal timing based on vehicle density
- **Multi-lane Support**: Manages traffic from four directions (up, down, left, right)
- **Phone Camera Integration**: Can process input from phone cameras for real-time monitoring
- **Ambulance Priority**: Special handling for emergency vehicles
- **Traffic Simulation**: Visual simulation of traffic flow and signal management

## 🛠️ Technologies Used

- Python 3.x
- OpenCV
- YOLOv8 (Ultralytics)
- NumPy
- Pandas
- Pygame (for simulation)

## 📁 Project Structure

```
Smart-Traffic-Control-System/
├── Final_Simulation.py              # Main traffic simulation
├── vehicle_detection.py             # Vehicle detection using YOLO
├── traffic_management_system.py    # Traffic signal management logic
├── Detect_From_Phone_CPU.py        # CPU-based phone detection
├── input_from_phone_camera.py      # Phone camera input handler
├── final_ambulance.py              # Ambulance detection and priority
├── model_training_script.py        # ML model training
├── data/
│   └── traffic_signal_data.csv     # Traffic data
├── images/                         # Vehicle and signal images
├── models/                         # Trained models
├── input/                          # Input images for testing
└── output/                         # Detection output images
```

## 🚀 Installation

1. Clone the repository:

```bash
git clone https://github.com/ayushman12baghel/Smart-Traffic-Control-System.git
cd Smart-Traffic-Control-System
```

2. Install required dependencies:

```bash
pip install opencv-python
pip install ultralytics
pip install numpy
pip install pandas
pip install pygame
```

3. Download YOLOv8 model (if not included):

```bash
# The model will be downloaded automatically on first run
```

## 💻 Usage

### Run Traffic Simulation

```bash
python Final_Simulation.py
```

### Vehicle Detection from Image

```bash
python vehicle_detection.py
```

### Phone Camera Input

```bash
python input_from_phone_camera.py
```

### Ambulance Detection

```bash
python final_ambulance.py
```

## 🎯 How It Works

1. **Vehicle Detection**: The system uses YOLOv8 to detect and count vehicles in each lane
2. **Density Calculation**: Calculates vehicle density for each direction
3. **Signal Optimization**: Dynamically adjusts green signal duration based on traffic density
4. **Priority Handling**: Gives priority to lanes with ambulances or higher vehicle density
5. **Visual Feedback**: Provides real-time simulation with visual representation of traffic flow

## 📊 Features Breakdown

### Vehicle Detection

- Detects multiple vehicle types: cars, buses, trucks, rickshaws
- Real-time counting and classification
- Supports both image and video input

### Traffic Management

- Adaptive signal timing algorithm
- Minimum and maximum signal duration constraints
- Queue-based lane prioritization

### Simulation

- Visual representation of traffic intersection
- Real-time vehicle movement animation
- Signal status display

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is open source and available under the MIT License.

## 👨‍💻 Author

**Ayushman Baghel**

- GitHub: [@ayushman12baghel](https://github.com/ayushman12baghel)

## 🙏 Acknowledgments

- YOLOv8 by Ultralytics
- OpenCV community
- Python community

---

⭐ If you found this project helpful, please consider giving it a star!
