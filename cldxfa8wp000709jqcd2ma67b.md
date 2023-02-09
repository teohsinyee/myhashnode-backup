# Computer Vision: Compare thresholding methods

Thresholding is a technique used in computer vision to separate an object from its background. There are three main types of thresholding: Global, Multiple, and Adaptive thresholding.

I will use a simple analogy to differentiate the methods.

**Let's imagine that you have a basket with apples and you want to separate the big apples from the small apples. 🧺🍎🍏**

In Global Thresholding, you use <mark>one rule</mark> to separate all the apples, for example, "apples that are bigger than a certain size are big apples."

In Multiple Thresholding, you use <mark>multiple rules</mark> to separate the apples, for example, "apples that are bigger than this size are big apples, apples that are smaller than this size are small apples."

In Adaptive Thresholding, you use a <mark>different rule for different parts</mark> of the basket, for example, "apples that are bigger than this size are big apples in this part of the basket, apples that are bigger than this size are big apples in this part of the basket."

### When to use which methods? 🤔🤔

Global thresholding is used when the image has a clear separation between the object and the background, and the pixel intensity values are approximately the same across the entire image. An example use case could be separating the text from the background in a scanned document.

Multiple thresholding is used when the object and the background have different intensity values in different regions of the image. This method separates the image into multiple segments based on these varying intensities. An example use case could be separating multiple objects in an image with different intensities, like separating apples and oranges in a basket.

Adaptive thresholding is used when the object and the background have varying intensity values, but the image is not necessarily divided into clear regions of uniform intensity. This method computes a threshold for each small region of the image, allowing for better accuracy in separating the object from the background. An example use case could be separating the text from the background in a document where the background has varying intensity, like a watermarked image.

### Strengths and weaknesses of each method 😊😖

Global thresholding works well when the object and background have distinct intensity values, but it can produce poor results when the intensity values are similar or when the object has multiple intensity values.

Multiple thresholding is useful when the object and background have different intensity values, but it can become complex when there are multiple objects or multiple intensity values in the image.

Adaptive thresholding is useful when the object and background have different intensity values, but the intensity values vary across the image. Adaptive thresholding is particularly useful when the object and background have similar intensity values, as it can adapt to the local intensity values to produce accurate results.

### Is adaptive thresholding the same as optimal thresholding? 🤔

Yes, Adaptive thresholding and Optimal thresholding can refer to the same thing. Adaptive thresholding refers to a method where the threshold value is calculated for each individual pixel or region in the image, rather than using a single global threshold for the entire image. The goal is to find the optimal threshold for each pixel or region, hence the name "Optimal thresholding".