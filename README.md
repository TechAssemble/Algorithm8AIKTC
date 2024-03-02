# Object Detection and Distance Measurement

## Overview

This repository contains two modules aimed at addressing distinct challenges using object detection techniques. The first module focuses on detecting and naming objects in real-time using YOLOv8 (You Only Look Once version 8), while the second module is designed for distance measurement, particularly applicable in scenarios with reduced visibility, such as foggy conditions, using LiDAR technology.

### Modules:

1. **Object Detection:**
    - This module is dedicated to the real-time detection and naming of objects using YOLOv8.
    - It includes functionality to capture live video feed and process it for object detection.
    - Detected objects are identified and their names are announced via a speaker.
    - Additionally, the module displays the distance of detected objects from the camera.

2. **Distance Measurement:**
    - The focus of this module is on measuring distances, particularly targeting scenarios with limited visibility, such as foggy conditions.
    - It utilizes LiDAR technology to accurately calculate distances, especially between the camera and detected persons or objects.
    - The primary application envisioned for this module is enhancing safety in situations where visibility is compromised, such as on roads during foggy weather.

## Motivation

These modules address various real-world challenges by leveraging object detection and distance measurement techniques. The motivation behind this project includes:

- Assisting visually impaired individuals by providing real-time object detection and identification.
- Enhancing educational experiences for children through interactive object recognition.
- Improving safety measures, particularly in scenarios with reduced visibility, such as foggy conditions on roads.

## Installation

To utilize these modules, follow the steps below:

1. Clone this repository:
    ```
    git clone https://github.com/your-username/ObjectDetection-DistanceMeasurement.git
    ```

2. Navigate to the respective directories:
    - `cd ObjectDetection` for the Object Detection module.
    - `cd DistanceMeasurement` for the Distance Measurement module.

3. Install dependencies:
    ```
    pip install -r requirements.txt
    ```

## Usage

### Object Detection:

1. Run the object detection script:
    ```
    python object_detection.py
    ```

2. Ensure that a live camera feed is available for real-time object detection.

### Distance Measurement:

1. Execute the distance measurement script:
    ```
    python distance_measurement.py
    ```

2. Make sure the LiDAR device is properly configured and connected for accurate distance measurements.

## Contributing

Contributions to this project are welcome. If you would like to contribute, please follow these guidelines:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/improvement`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add new feature'`).
5. Push to the branch (`git push origin feature/improvement`).
6. Create a new Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Special thanks to the creators and contributors of YOLOv8 and LiDAR technologies for their innovative solutions.
- Appreciation to the open-source community for their valuable contributions and support.

## Contact

For any inquiries or feedback regarding this project, please contact:

- Your Name
- Email: your@email.com

---

Feel free to customize the README with additional information or sections as needed. Let me know if you need further assistance!
