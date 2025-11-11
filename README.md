# WORKSHOP-3--Canny-Edge-Detection
## NAME: Dharshan V
## REG NO: 212224240035

# PROGRAM:
```python
import cv2
import matplotlib.pyplot as plt
img = cv2.imread('a.jpg',cv2.IMREAD_GRAYSCALE)
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
<img width="978" height="328" alt="Screenshot 2025-11-11 160644" src="https://github.com/user-attachments/assets/0f035aa3-e7dc-489f-986d-74a9611e17de" />
