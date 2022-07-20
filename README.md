# Face Swap AI
## In Constrained Environment
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
https://user-images.githubusercontent.com/71924682/179946894-4010f735-d5c5-4aca-a2b7-2d7a441d4e7c.mp4
---

---
Input Video                |  Processed Video
:-------------------------:|:-------------------------:
!https://user-images.githubusercontent.com/71924682/179947153-65e0bf7b-40d2-4fed-a20f-bb7cd75b3269.mp4   |  ![video3.webm](https://user-images.githubusercontent.com/71924682/179947249-bdb5cee7-4369-42df-bcf5-72427aa3ed9f.webm)

---
#Input Video:
---
We split the video into frames
and then crop those frames with
the help of a face align algo.
For the position we use the
optimal Postition. Then we
put the cropped frames
back together. 
---
<img width="382" alt="Bildschirmfoto 2022-07-19 um 09 50 06" src="https://user-images.githubusercontent.com/71924682/179947822-515b0fb6-5ee5-4456-be51-687fd9fc7395.png">
---

# Face Swap NN:
---
Now we can put our prepared video and our cropped image into the neural network, which changes specific attributes that can be seen on the colormap. You can swap the whole face and also just the lips, hair a.s.o.
---
Input Image                | Input Video               | Output Video
:-------------------------:|:-------------------------:|:-------------------------:
|!<img width="224" alt="Bildschirmfoto 2022-07-19 um 09 34 03" src="https://user-images.githubusercontent.com/71924682/179948115-4ea8c375-3698-4f35-a2f3-b11e0a11691a.png">|<img width="306" alt="Bildschirmfoto 2022-07-19 um 09 25 08" src="https://user-images.githubusercontent.com/71924682/179948200-c40981cf-b60f-4827-85c9-a378e02c742e.png">|<img width="306" alt="Bildschirmfoto 2022-07-19 um 09 38 37" src="https://user-images.githubusercontent.com/71924682/179948303-41423ed1-59e0-4848-b9de-c5639f1e8d97.png">
---
# Usage:
---
First you have to process your video so 
the face is in the middle. Then you have 
to align your importet image. At last you 
can then start the prediction which will 
be automaticly saved.
---
# Optimisations:
---
The code has already been optimized. The Picture
and Video should be taken in good lighting
for a good result. Too much head movement
and a wobbly Video will worsen the result <br>
immensely.
---
## Bad Lighting / Movement
https://user-images.githubusercontent.com/71924682/179948916-3468a00e-ded3-4c48-bbef-68fec722870c.mp4
---
## Movement
https://user-images.githubusercontent.com/71924682/179948949-f16453f1-a907-461c-a5f4-3269fd065080.mp4
---
## Better Lighting & Movement
https://user-images.githubusercontent.com/71924682/179948969-9ca2d7e9-75b0-4cf9-b2a1-d7b5aeba31b4.mp4
---
#Output Examples
---  
                           |                           |                           |
:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
|https://user-images.githubusercontent.com/71924682/179949650-1ad736ed-69b0-4ed1-b427-b6ab40519e20.mp4|[mask_video.webm](https://user-images.githubusercontent.com/71924682/179949753-fae88880-2adf-4c04-9bb2-2041e5394aeb.webm)|https://user-images.githubusercontent.com/71924682/179949790-af92ecca-3fd3-46ed-a84c-139dde1f0711.mp4|https://user-images.githubusercontent.com/71924682/179949783-2837117c-d06e-4fd3-b857-ddec698f447d.mp4
---







