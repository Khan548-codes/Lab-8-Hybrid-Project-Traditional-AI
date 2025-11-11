# Lab-8-Hybrid-Project-Traditional-AI

Hybrid Computer Vision Pipeline Explanation 🧠

1. Setup and Initialization
   
The pipeline begins by loading the peppers.png image and initializing the SqueezeNet Convolutional Neural Network (CNN). SqueezeNet acts as the AI component responsible for classification. This network requires the input image to be resized to 227×227 pixels.

2. Traditional Pre-processing (K-Means Segmentation) 🎨
   
The core traditional technique used is K-Means clustering applied to the image's color data. This step performs segmentation to achieve two goals:

Generate a Mask: Create a binary mask that separates the main objects (the peppers and vegetables) from the background.

Isolate the Object: 
Apply this mask to the original image to produce the Isolated Object (peppers on a black background).

This traditional step is crucial because it removes visual clutter (the complex purple and white background), allowing the AI to focus only on the features of the target objects.

3. AI Classification and Analysis 📊
The Isolated Object is resized to fit the SqueezeNet input requirement. The CNN then processes this cleaner, pre-processed image.

Classification Result: The AI model classified the isolated object as: 
[Insert Classification Result]

Confidence: [Insert Probability]%

This hybrid approach demonstrates that using traditional segmentation to clean the input image can lead to a more focused and potentially higher-confidence classification result from the AI component compared to classifying the original, busy image directly. The two methods combine to improve overall pipeline performance.

![images](https://github.com/Khan548-codes/Lab-8-Hybrid-Project-Traditional-AI/blob/main/images/Screenshot%202025-11-11%20194723.png)
