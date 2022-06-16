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

4.Devlop a program to convert color string to RGB color value?<br>
from PIL import ImageColor<br>
# using getrgb for yellow<br>
img1=ImageColor.getrgb("yellow")<br>
print(img1)<br>
# using getrgb for red<br>
img2=ImageColor.getrgb("red")<br>
print(img2)<br>
output:<br>
(255, 255, 0)<br>
(255, 0, 0)<br>

5.write program to convert image using colors?<br>
from PIL import Image<br>
img=Image.new('RGB',(200,400),(255,255,0))<br>
img.show()<br>
output:<br>![image](https://user-images.githubusercontent.com/87934584/174045340-b68e99d2-efd1-448f-82fa-5a60ba0f7d0c.png)

6.Develop a program to utilize the image using varoius color spaces?<br>
import cv2<br>
import matplotlib.pyplot as plt<br>
import numpy as np<br>
img=cv2.imread('tree.jpg')<br>
plt.imshow(img)<br>
plt.show()<br>
img=cv2.cvtColor(img,cv2.COLOR_BGR2RGB)<br>
plt.imshow(img)<br>
plt.show()<br>
img=cv2.cvtColor(img,cv2.COLOR_RGB2HSV)<br>
plt.imshow(img)<br>
plt.show()<br>
img= cv2.cvtColor(img, cv2.COLOR_BGR2GRAY )<br>
plt.imshow(img)<br>
plt.show()<br>
output:<br>![image](https://user-images.githubusercontent.com/87934584/174047092-6dc17c6e-5059-46d6-a2bf-a55ab868b90b.png)<br>![image](https://user-images.githubusercontent.com/87934584/174047235-e777a1c4-ad6b-4d76-8c88-4952e937829e.png)<br>![image](https://user-images.githubusercontent.com/87934584/174047345-e8d61201-a6f0-4693-bd97-4b182acec4f9.png)<br>![image](https://user-images.githubusercontent.com/87934584/174047481-c564f4de-28e7-4d4d-88eb-6c43887554f9.png)

7.write a program to display the image attributes?<br>
from PIL import Image<br>
image=Image.open('tree.jpg')<br>
print("filename:",image.filename)<br>
print("format:",image.format)<br>
print("mode:",image.mode)<br>
print("size:",image.size)<br>
print("width:",image.width)<br>
print("height:",image.height)<br>
image.close()<br>

output:<br>filename: tree.jpg<br>
format: JPEG<br>
mode: RGB<br>
size: (1334, 888)<br>
width: 1334<br>
height: 888<br>


