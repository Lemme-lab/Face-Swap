# Face Swap AI - In Constrained Environment
---
![cropped_input_image-2](https://user-images.githubusercontent.com/71924682/179951079-3f1acb1a-c3f1-458a-9b35-9ce9bf003c22.jpg)
---
![ezgif com-gif-maker-3](https://user-images.githubusercontent.com/71924682/179952109-f0e9c279-a1b7-4daa-805e-8051fa8115ae.gif)
---
![ezgif com-gif-maker-4](https://user-images.githubusercontent.com/71924682/179952116-24957de3-5ded-4be2-b723-8fb258449cc6.gif)

---
# Face Swap Idea
---
The idea was to create a Face swap AI that can be deployed in Constrained Environments. 
It swapes the face of the input video with the input image.
---
![ezgif com-gif-maker-5](https://user-images.githubusercontent.com/71924682/179953028-cd528aba-4c51-434f-8554-c5249ec480a5.gif)
---
![ezgif com-gif-maker-6](https://user-images.githubusercontent.com/71924682/179953372-1d901100-264d-4bdb-b79d-fa21d45d6f4d.gif)
---
![ezgif com-gif-maker-8](https://user-images.githubusercontent.com/71924682/179953696-82af6b6b-dfec-4000-a1d8-1413fe64f607.gif)
---
# Input Video:
---
### We split the video into frames and then crop those frames with the help of a face align algo. For the position we use the optimal Postition. Then we put the cropped frames back together. 
---
<img width="382" alt="Bildschirmfoto 2022-07-19 um 09 50 06" src="https://user-images.githubusercontent.com/71924682/179947822-515b0fb6-5ee5-4456-be51-687fd9fc7395.png">
---

# Face Swap NN:
---
### Now we can put our prepared video and our cropped image into the neural network, which changes specific attributes that can be seen on the colormap. You can swap the whole face and also just the lips, hair a.s.o.
---


Input Image                | Mask + Image               | Mask
 :-------------------------:|:-------------------------:|:-------------------------:
 |!<img width="250" alt="Bildschirmfoto 2022-07-19 um 09 34 03" src="https://user-images.githubusercontent.com/71924682/179948115-4ea8c375-3698-4f35-a2f3-b11e0a11691a.png">|<img width="250" alt="Bildschirmfoto 2022-07-19 um 09 25 08" src="https://user-images.githubusercontent.com/71924682/179948200-c40981cf-b60f-4827-85c9-a378e02c742e.png">|<img width="250" alt="Bildschirmfoto 2022-07-19 um 09 38 37" src="https://user-images.githubusercontent.com/71924682/179948303-41423ed1-59e0-4848-b9de-c5639f1e8d97.png">

---
# Usage:
---
### First you have to process your video so the face is in the middle. Then you have to align your importet image. At last you can then start the prediction which will be automaticly saved.
---
# Optimisations:
---
### The code has already been optimized. The Picture and Video should be taken in good lighting for a good result. Too much head movement and a wobbly Video will worsen the result immensely.
---
## Bad Lighting / Movement
![ezgif com-gif-maker-9](https://user-images.githubusercontent.com/71924682/179955262-f515fb2a-7c67-450c-83bd-10add78cd53d.gif)
---
## Bad Movement
![ezgif com-gif-maker-10](https://user-images.githubusercontent.com/71924682/179955289-035796f4-fddb-4f3a-9a8c-34d019d082bd.gif)
---
## Better Lighting & Movement
![ezgif com-gif-maker-11](https://user-images.githubusercontent.com/71924682/179955324-f1e5723b-31e0-452c-bd17-3e44bc5b039c.gif)
---
#Output Examples
---
![ezgif com-gif-maker-12](https://user-images.githubusercontent.com/71924682/179956175-06bf372a-1bf1-4dff-a865-799983533487.gif)
---
![ezgif com-gif-maker-13](https://user-images.githubusercontent.com/71924682/179956214-a7fe5edd-c509-466f-a334-1e7a5ef5ab49.gif)
---
![ezgif com-gif-maker-14](https://user-images.githubusercontent.com/71924682/179956244-59608e70-0fe3-46df-b253-f98073847a0c.gif)
---
![Uploading ezgif.com-gif-maker-15.gif…]()







