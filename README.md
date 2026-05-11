# Image Handling and Pixel Transformations Using OpenCV

## 📌 Project Overview
This project demonstrates basic image handling and pixel transformation operations using Python and OpenCV. The notebook contains multiple exercises related to reading, displaying, saving, cropping, splitting, merging, and transforming images.

The project is designed as a college laboratory exercise for learning the fundamentals of Digital Image Processing (DIP) using OpenCV.

---

# 🎯 Objectives
- Understand the basics of image processing using OpenCV.
- Learn how to read and display grayscale and color images.
- Perform image transformations such as cropping and resizing.
- Explore image channel manipulation using RGB and HSV color models.
- Understand pixel-level operations in digital images.
- Learn how to save processed images using OpenCV.
- Gain hands-on experience with NumPy and Matplotlib for image visualization.

---

# 🛠 Technologies Used
| Technology | Purpose |
|---|---|
| Python | Core programming language |
| OpenCV (cv2) | Image processing operations |
| NumPy | Numerical and array operations |
| Matplotlib | Image visualization and plotting |
| Jupyter Notebook | Development environment |

---

# 📂 Project Structure
```bash
Project Folder/
│
├── Ex. 01.ipynb
├── Eagle_in_Flight.jpg
├── boy.jpg
├── outputs/
│   ├── grayscale_image.png
│   ├── cropped_image.png
│   ├── rgb_channels.png
│   ├── hsv_channels.png
│   └── merged_images.png
└── README.md
```

---

# ⚙️ How It Works

## 1. Import Required Libraries
The project starts by importing the required Python libraries:

```python
import cv2
import numpy as np
import matplotlib.pyplot as plt
```

---

## 2. Read Image Using OpenCV
The image is loaded using OpenCV's `imread()` function.

```python
img = cv2.imread("Eagle_in_Flight.jpg")
```

---

## 3. Display Image
The loaded image is displayed using Matplotlib.

```python
plt.imshow(img)
plt.show()
```

---

## 4. Print Image Dimensions
The height, width, and number of channels are obtained using:

```python
print(img.shape)
```

---

## 5. Save Image
The processed image is saved using:

```python
cv2.imwrite("output.png", img)
```

---

## 6. Convert Image Color Space
The project converts images from BGR to RGB using:

```python
rgb = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
```

---

## 7. Crop Specific Object
A specific region of the image (such as the eagle) is cropped using array slicing.

```python
crop = img[y1:y2, x1:x2]
```

---

## 8. Split RGB Channels
The image is split into Blue, Green, and Red channels.

```python
b, g, r = cv2.split(img)
```

---

## 9. Merge RGB Channels
The separated channels are merged back into a single image.

```python
merged = cv2.merge([b, g, r])
```

---

## 10. Convert to HSV Color Space
The RGB image is converted into HSV format.

```python
hsv = cv2.cvtColor(img, cv2.COLOR_BGR2HSV)
```

---

## 11. Split HSV Channels
The Hue, Saturation, and Value channels are separated.

```python
h, s, v = cv2.split(hsv)
```

---

## 12. Merge HSV Channels
The HSV channels are merged back to reconstruct the image.

```python
merged_hsv = cv2.merge([h, s, v])
```

---

# 🖼 Output Section
Place all generated outputs inside the `outputs/` folder.
- Grayscale image:
  <img width="516" height="415" alt="image" src="https://github.com/user-attachments/assets/36ebf5c5-b40f-49bc-bc55-8b4fbff55e2c" />

- RGB image
  <img width="485" height="414" alt="image" src="https://github.com/user-attachments/assets/095b457d-dab4-48ea-bb54-d36f911d06e6" />

- Cropped image
  <img width="600" height="358" alt="image" src="https://github.com/user-attachments/assets/2cf2523b-5fbe-4eb2-9442-8e378edf8baf" />
- Draw a magenta rectangle that encompasses the launch tower and the rocket.
  <img width="605" height="324" alt="image" src="https://github.com/user-attachments/assets/fb9d1519-0cd4-40ae-abfb-80abc3887ace" />

- Split RGB channels
 <img width="703" height="208" alt="image" src="https://github.com/user-attachments/assets/8fc5e8d8-734e-4242-95ba-bf6cbd22bc85" />

- Split HSV channels
  <img width="711" height="192" alt="image" src="https://github.com/user-attachments/assets/9ff68b52-9a8f-4c83-a673-853e317fc8df" />

- Merged RGB image
  <img width="704" height="281" alt="image" src="https://github.com/user-attachments/assets/9219b83c-f288-42a7-8405-62221db930c2" />

- Merged HSV image
<img width="700" height="279" alt="image" src="https://github.com/user-attachments/assets/3f5af74f-b413-4514-8746-d83fc342d2a1" />

---

# ▶️ Steps to Run the Project

1. Install required libraries:

```bash
pip install opencv-python matplotlib numpy
```

2. Open Jupyter Notebook:

```bash
jupyter notebook
```

3. Run the notebook file:

```bash
Ex. 01.ipynb
```

---

# 📚 Learning Outcomes
After completing this project, you will be able to:

- Handle images using OpenCV.
- Perform basic image transformations.
- Understand image color spaces.
- Work with image channels.
- Visualize images using Matplotlib.
- Apply pixel-level manipulations in Python.

---

# 👨‍💻 Author
**Pravin Kumar**  
Department of Artificial Intelligence and Data Science

