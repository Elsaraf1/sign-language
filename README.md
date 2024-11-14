# Sign Language MNIST Dataset

The **Sign Language MNIST** dataset is a real-world-inspired, drop-in replacement for the classic MNIST dataset. It presents a challenging multi-class problem with **24 classes of American Sign Language (ASL) hand gestures** representing the alphabetic letters (A-Z), excluding **J** and **Z**, which require motion.  

### Dataset Overview
- **Image Format**: Grayscale, 28x28 pixels  
- **Labels**: Numeric (0-25) mapped to letters A-Z  
- **Training Data**: 27,455 samples  
- **Test Data**: 7,172 samples  
- **Format**: CSV with rows containing labels and 784 pixel values  

### Data Creation
The dataset was created using an extensive pipeline:
1. Original color images were cropped to hands-only, gray-scaled, resized, and augmented.
2. Augmentations included:
   - Filters (`Mitchell`, `Robidoux`, `Catrom`, `Spline`, `Hermite`)
   - Brightness/contrast adjustments (+/-15%)
   - 3-degree rotation
   - 5% random pixelation  

These enhancements improved the dataset's resolution and class separation, offering a unique challenge for machine learning models like Convolutional Neural Networks (CNNs).  

### Applications
A robust visual recognition model trained on this dataset could:
- Benchmark modern computer vision models
- Enable ASL translation tools for the deaf and hard-of-hearing  
Potential integrations include affordable devices like Raspberry Pi with OpenCV and Text-to-Speech capabilities.
