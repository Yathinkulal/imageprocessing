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
img1=ImageColor.getrgb("yellow")<br>
print(img1)<br>
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

7.Write a program to display the image attributes?<br>
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

8.Resize the original image?<br>
import cv2<br>
img=cv2.imread('flower3.jpg')<br>
print('original image length width',img.shape)<br>
cv2.imshow('original image',img)<br>
imgresize=cv2.resize(img,(150,160))<br>
cv2.imshow('resized image',imgresize)<br>
print('Resized image length width',imgresize.shape)<br>
cv2.waitKey(0)<br>

output:<br>original image length width (720, 480, 3)<br>
Resized image length width (160, 150, 3)<br>Original size<br>
![image](https://user-images.githubusercontent.com/87934584/174052544-647bd975-9c97-4d0d-94f0-9d71f2239edb.png)<br>
Resized<br>
![image](https://user-images.githubusercontent.com/87934584/174052666-8dc4911b-f512-4b01-9e09-498d7e1a6b2b.png)

9.Convert the original image to gray scale and then to binary?<br>
/*raed the image file*/<br>
img=cv2.imread('flower3.jpg')<br>
cv2.imshow("RGB",img)<br>
/*gray scale*/<br>
img=cv2.imread('flower3.jpg',0)<br>
cv2.imshow("Gray",img)<br>
/*binary image*/<br>
ret,bw_img=cv2.threshold(img,127,255,cv2.THRESH_BINARY)<br>
cv2.imshow("Binary",bw_img)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
output:<br>![image](https://user-images.githubusercontent.com/87934584/174053635-551b6858-1c66-46b5-8e8c-adeade67bc8c.png)<br>
![image](https://user-images.githubusercontent.com/87934584/174053757-83ee3766-1ddb-4047-94d1-ed86853f8a71.png)<br>
![image](https://user-images.githubusercontent.com/87934584/174053879-82cc481a-c5ff-4c50-8abd-ab50bf4d3104.png)

10.Develop a program to readimage using URL?<br>
from skimage import io<br>
import matplotlib.pyplot as plt<br>
url='https://www.alfredapp.com/blog/tips-and-tricks/tiny-png-workflow-compress-images/tinypng-panda.png'<br>
image=io.imread(url)<br>
plt.imshow(image)<br>
plt.show()<br>

output:<br>
![image](https://user-images.githubusercontent.com/87934584/175267752-1bb4a140-4b67-4c3b-a490-0dd6a8ab7388.png)

12.Write a program to perform arithmatic operations on images?<br>
import cv2<br>
import matplotlib.image as mpimg<br>
import matplotlib.pyplot as plt<br>

*/reading imsge files/*<br>
img1=cv2.imread('website.jpg')<br>
img2=cv2.imread('m.jpg')<br>

*/applying NumPy addition on images/*<br>
fimg1=img1+img2<br>
plt.imshow(fimg1)<br>
plt.show()<br>

*/saving the otput image/*<br>
cv2.imwrite('output.jpg',fimg1)<br>
fimg2=img1-img2<br>
plt.imshow(fimg2)<br>
plt.show()<br>


*/saving the output image/*<br>
cv2.imwrite('output.jpg',fimg2)<br>
fimg3=img1*img2<br>
plt.imshow(fimg3)<br>
plt.show()<br>

*/saving the output image/*<br>
cv2.imwrite('output.jpg',fimg3)<br>
fimg4 = img1 / img2<br>
plt.imshow(fimg4)<br>
plt.show()<br>

*/saving the output image/*<br>
cv2.imwrite('output.jpg',fimg4)<br>
output:<br>
![image](https://user-images.githubusercontent.com/87934584/175269198-52ead221-e121-4fe0-ba85-09751b60abc0.png)<br>
![image](https://user-images.githubusercontent.com/87934584/175271054-ab7b624d-074e-4e92-9c13-315185689fc3.png)<br>
![image](https://user-images.githubusercontent.com/87934584/175271256-6c5490fc-eeb7-4ec8-965e-4a0cc0a5d18d.png)


