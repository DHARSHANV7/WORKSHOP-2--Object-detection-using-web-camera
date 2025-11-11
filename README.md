# WORKSHOP-3--Canny-Edge-Detection
## NAME: ROGITH. K
## REG NO: 212223110042

# PROGRAM:
```python
import cv2
import matplotlib.pyplot as plt
img = cv2.imread('Rogith.jpg',cv2.IMREAD_GRAYSCALE)
blurred =cv2.GaussianBlur(img, (5,5),0)
edges = cv2.Canny(blurred, 50, 150) 
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()
```

# OUTPUT:
<img width="921" height="532" alt="Screenshot 2025-11-11 153138" src="https://github.com/user-attachments/assets/26dcd159-b55a-4516-92ef-2d9bb4a9abf6" />

