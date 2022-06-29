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
![image](https://user-images.githubusercontent.com/87934584/175267752-1bb4a140-4b67-4c3b-a490-0dd6a8ab7388.png)<br>
11.
import cv2<br>
import matplotlib.image as mpimg<br>
import matplotlib.pyplot as plt<br>
img=mpimg.imread('images.jpg')<br>
plt.imshow(img)<br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/87934584/175288897-b09f70dc-787b-4b19-beb5-aa9b54cb04cb.png)<br>

hsv_img=cv2.cvtColor(img,cv2.COLOR_RGB2HSV)<br>
light_orange=(0,50,50)<br>
dark_orange=(10,255,255)<br>
mask=cv2.inRange(hsv_img,light_orange,dark_orange)<br>
result=cv2.bitwise_and(img,img,mask=mask)<br>
plt.subplot(2,1,1)<br>
plt.imshow(mask,cmap="gray")<br>
plt.subplot(2,1,2)<br>
plt.imshow(result)<br>
plt.show()<br>
output:<br>
![image](https://user-images.githubusercontent.com/87934584/175289105-10541db3-c382-4f66-8dab-a73fbf23faa5.png)
![image](https://user-images.githubusercontent.com/87934584/175289116-33e1fd8a-8b01-4389-81ff-299755b1ebdf.png)<br>
light_white=(0,0,200)<br>
dark_white=(145,60,255)<br>
mask_white=cv2.inRange(hsv_img,light_white,dark_white)<br>
result_white=cv2.bitwise_and(img,img,mask=mask_white)<br>
plt.subplot(1,2,1)<br>
plt.imshow(mask_white,cmap="gray")<br>
plt.subplot(1,2,2)<br>
plt.imshow(result_white)<br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/87934584/175289164-cc631749-91e1-4fc6-9ad2-03f093de4ab2.png)
![image](https://user-images.githubusercontent.com/87934584/175289196-4e81d1dc-b5c5-44d5-8545-7fbc9d6817f7.png)<br><br>
final_mask=mask+mask_white<br>
final_result=cv2.bitwise_and(img,img,mask=final_mask)<br>
plt.subplot(1,2,1)<br>
plt.imshow(final_mask,cmap="gray")<br>
plt.subplot(1,2,2)<br>
plt.imshow(final_result)<br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/87934584/175289261-eab81fc0-4e8e-4266-9691-6410cbccc286.png)
![image](https://user-images.githubusercontent.com/87934584/175289283-ab0a0a56-c9b8-4d92-965b-ef3fa899d725.png)<br>
blur=cv2.GaussianBlur(final_result,(7,7),0)<br>
plt.imshow(blur)<br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/87934584/175289334-3e3334c1-60fa-440b-8b80-ac5b9f636260.png)







12.Write a program to perform arithmatic operations on images?<br>
import cv2<br>
import matplotlib.image as mpimg<br>
import matplotlib.pyplot as plt<br>

*/reading imsge files/*<br>
*/image should be in same size but different img/*
img1=cv2.imread('goat.jpg')<br>
img2=cv2.imread('king.jpg')<br>

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
![image](https://user-images.githubusercontent.com/87934584/175277477-3e87a4cf-031e-4283-8e10-ce7043cf7b94.png)
<br>
![image](https://user-images.githubusercontent.com/87934584/175277567-05318f3a-8ca8-41f4-9a80-e2281f9429f0.png)<br>
![image](https://user-images.githubusercontent.com/87934584/175277618-95bed0a2-fb71-424a-acae-24e245b5f218.png)<br>
![image](https://user-images.githubusercontent.com/87934584/175277676-573d6804-5892-414f-b67c-74302224c2a0.png)<br>


13.Develop the program to change the image into different color?<br>
import cv2<br>
img=cv2.imread("car.jpg")<br>
gray=cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)<br>
hsv=cv2.cvtColor(img,cv2.COLOR_BGR2HSV)<br>
lab=cv2.cvtColor(img,cv2.COLOR_BGR2LAB)<br>
hls=cv2.cvtColor(img,cv2.COLOR_BGR2HLS)<br>
yuv=cv2.cvtColor(img,cv2.COLOR_BGR2YUV)<br>
cv2.imshow("GRAY image",gray)<br>
cv2.imshow("HSV image",hsv)<br>
cv2.imshow("LAB image",lab)<br>
cv2.imshow("HLS image",hls)<br>
cv2.imshow("YUV image",yuv)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
Output:<br>
![image](https://user-images.githubusercontent.com/87934584/175274437-7b2f1867-0376-4aeb-9952-d4d3ae43390c.png)<br>
![image](https://user-images.githubusercontent.com/87934584/175274546-c1a28c63-5fb3-40c7-9d1c-f154104a4bf3.png)<br>
![image](https://user-images.githubusercontent.com/87934584/175274629-e9b4f270-323a-497e-8455-eb20076ca287.png)<br>
![image](https://user-images.githubusercontent.com/87934584/175274748-e60c136d-7c75-4e3d-881f-92764fb0243d.png)<br>
![image](https://user-images.githubusercontent.com/87934584/175274893-754300ef-2708-493a-9cff-1ab252328f5a.png)<br>
14.Program to create an image using 2D array?
import cv2 as c<br>
import numpy as np<br>
from PIL import Image<br>
array=np.zeros([100,200,3],dtype=np.uint8)<br>
array[:,:100]=[255,130,0]<br>
array[:,100:]=[0,0,255]<br>
img=Image.fromarray(array)<br>
img.save('img1.png')<br>
img.show()<br>
c.waitKey(0)<br>
Output:<br>
![image](https://user-images.githubusercontent.com/87934584/175275363-32b08489-6317-4b74-8bc1-ff2d4261f2fd.png)


