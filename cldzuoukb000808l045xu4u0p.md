# Computer Vision: Compare edge segmentation methods

When it comes to detecting the shape of an object in an image, there are several methods that can be used. The most commonly used methods are edge thresholding, edge linking, border tracing, and graph searching. In this article, we will compare these methods and understand when to use each one.

### Edge Thresholding

Edge thresholding is the first step in detecting the edges of an object in an image. The process involves converting the image into a binary format and finding the intensity gradients along the edges of the object. The intensity gradient refers to the change in intensity of pixels in an image and helps to identify pixels with a significant change in intensity, which usually corresponds to edges in the image.

#### Finding the Intensity Gradient using Derivatives

Edge detection involves finding the boundaries between different regions in an image. One way to do this is by detecting the intensity gradient in the image, which is the rate of change of intensity at each point.

Two methods to detect the intensity gradient are:

1. Detecting the local maxima or minima of the first derivative:
    
    The first derivative is a measure of the rate of change of intensity at each point. Local maxima or minima of the first derivative indicate points where the intensity changes rapidly, which correspond to edges in the image.
    

1. Detecting the zero-crossings of the second derivative:
    
    The second derivative is a measure of the rate of change of the first derivative. Zero-crossings of the second derivative occur at points where the second derivative changes sign, meaning it goes from positive to negative or vice versa. These points correspond to the locations of the edges in the image.
    

To visualize this, consider an image of a car.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1676112426554/0369dc21-cf18-45af-927d-a87f28d7da6e.jpeg align="left")

The edges of the car in the image correspond to points where there is a rapid change in intensity, either from <mark>one color to another</mark> or from a <mark>bright region to a dark region</mark>. The first derivative measures this change, and the second derivative further refines this information by indicating the zero-crossings, which correspond to the actual edges of the car.

### Edge Linking

After edge thresholding, the next step is edge linking, where the edges that were detected in the first step are connected to form lines that represent the boundaries of the object. This step helps to connect the dots along the edges to create a complete representation of the object.

### Border Tracing

The third step is border tracing, where the lines formed in the edge linking step are followed to determine the exact shape of the object. This involves tracing the boundaries of the object by following the connected lines.

### Graph Searching

Finally, graph searching is performed to find the coordinates of the object in the image. This step involves finding the x,y coordinates of the object in the image and using those coordinates to locate the object within the image.

### Edge Thresholding vs Global Thresholding

When it comes to comparing edge thresholding and global thresholding, edge thresholding is considered to be more accurate, especially in cases where the object and background have similar intensity values. This allows for a more accurate representation of the object and its edges compared to the simple threshold value used in global thresholding.

On the other hand, simple images with clear intensity values can be effectively segmented using global thresholding, while more complex images with multiple intensity values may require the use of edge segmentation techniques. Global thresholding is faster and may be sufficient for some applications, but edge-based methods may be more appropriate for applications where accuracy is a higher priority.

In conclusion, the <mark>choice of method depends on the application and the desired level of accuracy</mark>. Simple images can be effectively segmented using global thresholding, while more complex images may require the use of edge segmentation techniques. It's also worth mentioning that the choice of edge segmentation method may also <mark>depend on the computational resources</mark> available, as some methods may be more computationally expensive than others. For example, graph searching can be computationally intensive, but may be necessary for applications that require a high degree of accuracy.

### Bonus: Common algorithms used for edge thresholding

| **Algorithm** | **Description** |
| --- | --- |
| Canny Edge Detection | One of the most popular edge detection algorithms, it uses the first and second derivatives of the image intensity to detect edges. It includes steps such as Gaussian smoothing, finding intensity gradients, non-maximum suppression, and double thresholding. |
| Sobel Operator | A popular edge detection algorithm that uses a kernel with horizontal and vertical filters to find edges. |
| Prewitt Operator | A type of gradient-based edge detection algorithm that uses a kernel with horizontal and vertical filters to find edges. |
| Laplacian | An edge detection algorithm that uses a Laplacian kernel to find the second derivative of the image intensity, which indicates where the intensity changes rapidly. |