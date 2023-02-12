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

* Assuming the goal of the system is to analyse the real-time traffic condition, the desired input will be the cars on the road, how congested it is, average speed of the cars.
    
* Camera is used to capture the image on road, the image will be preprocessed, analysed and interpreted through AI, and output the traffic condition.
    

<mark>Chat-GPT answer:</mark>

* What are the components of CV: Input, Processing, Output
    
* Goal of input & how: Capture cars on road through camera
    
* Goal of processing & how: Object detection through image preprocessing techniques such as segmentation (Segment cars from the background)
    
* Goal of output & how: Display result on screen. E.g. Display the degree of congestion, number of cars.
    

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

* Thresholding (Detailed explanation refer to: [Compare thresholding methods](https://teohsinyee.hashnode.dev/computer-vision-compare-thresholding-methods))
    
* Edge-based segmentation (Detailed explanation refer to: [Compare edge segmentation methods](https://teohsinyee.hashnode.dev/edge-segmentation-methods))
    
* Region-based segmentation (Detailed explanation refer to: [Compare region-based segmentation methods](https://teohsinyee.hashnode.dev/computer-vision-compare-region-based-segmentation-methods))
    

4\. (10 marks) Discuss the **importance of image feature extraction** in this system, and **describe the types of features** that can be extracted from the images of vehicles.

<mark>My answer:</mark>

Feature extraction is important to extract useful information from the image. There are three types of features can be extracted for vehicles images:

1. region features: features that describe shape of vehicles, can be used to identify vehicle type such as car, motorcycle
    
2. line features: features that describe edges of vehicles, can be used to identify the car speed
    
3. point features: features that describe unique points on the vehicles in the images, such as the headlights, taillights, and license plate, can be used to identify individual vehicles and track them over time.
    

5\. (10 marks) Discuss the applications of an automated traffic surveillance system and the impact it can have on road safety and traffic management.

<mark>Chat-GPT answer:</mark>

The applications of an automated traffic surveillance system are as below:

1. Traffic Monitoring: The system can monitor the flow of traffic, counting the number of vehicles and their speed. This information can be used to optimize traffic management strategies and reduce congestion.
    
2. Law Enforcement: The system can assist law enforcement agencies in enforcing traffic laws, such as identifying speeding vehicles or those that run red lights. This can help to reduce the number of accidents and improve road safety.
    
3. Congestion Management: By monitoring traffic flow and counting vehicles, the system can help to identify and reduce congestion. This can lead to a reduction in travel time and fuel consumption, as well as improved air quality.
    
4. Toll Collection: The system can be used to automate the collection of tolls, reducing the need for manual labor and improving the efficiency of toll collection.
    
5. Accident Investigation: The system can be used to gather evidence in the event of an accident, assisting in investigations and helping to determine fault.
    
6. License Plate Recognition: The system can perform license plate recognition, which can be used to identify vehicles for a variety of purposes, such as parking management, access control, and criminal investigations.
    

The system can improve road safety by reducing the number of accidents and enforcing traffic laws. It can also improve traffic management by reducing congestion, optimizing traffic flow, and improving the efficiency of toll collection. By automating many of the manual tasks associated with traffic management and road safety, the system can free up human resources and resources to be used elsewhere.