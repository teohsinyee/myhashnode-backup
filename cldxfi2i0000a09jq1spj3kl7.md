# Computer Vision Practice (Case studies)

Have you ever wondered how a child can effortlessly recognize objects just by seeing them? This ability captivated the imagination of Li Fei-fei, a name you definitely should know in the field of computer vision. She was determined to train a system to do the same, and so began the **ImageNet** project in 2007.

The ImageNet project involved collecting millions of images from online sources and hiring 50,000 labelers to annotate the images. In 2009, the result was a dataset with over 15 million labeled images and 20,000 categories, which has become a valuable asset in the field of computer vision.

Li Fei-fei's work on ImageNet has had a significant impact on the field and continues to inspire new advances.

Whether you're a student studying computer vision or a professional in the industry, the story of the ImageNet project is a testament to the power of passion and dedication in driving progress.

Source: [How we teach computers to understand pictures | Fei Fei Li](https://youtu.be/40riCqvRoMs)

Okay enough story, let's start to do revision!

---

### Case Study 1: Automated Traffic Surveillance System

1\. (10 marks) Describe the basic **components** of a computer vision system and explain **how** they can be used in an automated traffic surveillance system.

<mark>My answer:</mark>

\* Assuming the goal of the system is to analyse the real-time traffic condition, the desired input will be the cars on the road, how congested it is, average speed of the cars.

\* Camera is used to capture the image on road, the image will be preprocessed, analysed and interpreted through AI, and output the traffic condition.

<mark>Chat-GPT answer:</mark>

\* What are the components of CV: Input, Processing, Output

\* Goal of input & how: Capture cars on road through camera

\* Goal of processing & how: Object detection through image preprocessing techniques such as segmentation (Segment cars from the background)

\* Goal of output & how: Display result on screen. E.g. Display the degree of congestion, number of cars.

2\. (10 marks) Discuss the **importance of image preprocessing** in this system, and **describe the steps** involved in cleaning up and enhancing the images captured by the cameras.

<mark>My answer:</mark>

* Importance: Ensure system accuracy & effectiveness because the raw images captured can often contain noise or other distortions that make it difficult to accurately detect cars on road
    
* Steps:
    
    * Image enhancement by adjust the image contrast/brightness to highlight the car of interest
        
    * Noise reduction by filtering out random noise to improve image quality, e.g. Gaussian noise
        
    * Background subtraction by subtracting background image from each frame
        
    * Image segmentation to partition image into regions or segments based on attributes such as intensity to isolate cars of interest.
        

3\. (10 marks) Explain the **techniques used in image segmentation** in this system, and describe how they can be used to separate vehicles from the background in the images.

<mark>My answer:</mark>

* Thresholding
    
* Edge-based segmentation
    
* Region-based segmentation
    

4\. (10 marks) Discuss the **importance of image feature extraction** in this system, and **describe the types of features** that can be extracted from the images of vehicles.

(To be discussed next day)

5\. (10 marks) Discuss the applications of an automated traffic surveillance system and the impact it can have on road safety and traffic management.

(To be discussed next day)