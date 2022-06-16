# imageprocessing
1.Develop a program   to dispaly grayscale image using read & write operation import cv2 ?<br>
<br>
import cv2<br>
img=cv2.imread('flower.jpg',0)<br>
cv2.imshow('Image',img)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>

output:<br>![image](https://user-images.githubusercontent.com/87934584/173816906-e0c7944b-2439-467f-94ec-f31fcef66887.png)<br>

2.Develop a program to display yhe image using matplotlib?<br>
import matplotlib.image as mping<br>
import matplotlib.pyplot as plt<br>
img=mping.imread('leaf1.jpg')<br>
plt.imshow(img) <br>

 output:<br>![image](https://user-images.githubusercontent.com/87934584/174043139-fe957ed6-32c4-4784-a3e4-e6e537c6ed57.png)

3.Develop a program to perform Linmear tranforamtion rotation?<br>
from PIL import Image<br>
img=Image.open('butterfly.jpg')<br>
img=img.rotate(180)<br>
img.show()<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
<br>
output:<br>![image](https://user-images.githubusercontent.com/87934584/174043984-80c0af26-5dab-48ba-8940-19fda9ed5397.png)
