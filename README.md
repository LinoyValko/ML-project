# ML-project

This project focuses on Multi-Class Texture Analysis in Colorectal Cancer Histology using a dataset comprising 5000 histological images of human colorectal cancer. The dataset encompasses 8 different tissue types: 'Tumour epithelium', 'Simple stroma', 'Complex stroma', 'Immune cells', 'Debris', 'Normal mucosal glands', 'Adipose tissue', and 'Background', each with dimensions of (150, 150, 3).

Data Preprocessing
The pixel values in the images, originally ranging from 0 to 255, were normalized to a float dataset between 0 and 1.
The dataset was split into 90% training (4500 images) and 10% testing (500 images) sets.
Results
The most successful model was the 9th experiment, utilizing the VGG 16 model. This model demonstrated effective dimensionality reduction for image data while maintaining data variance. With only 16 layers, the VGG 16 model, with 'relu' and 'softmax' activation functions, proved optimal for classification. The 8th experiment also yielded favorable results, emphasizing the effectiveness of softmax activation for normalizing neural network outputs.

Recommendations
VGG 16 Model Usage: Based on the superior performance in the 9th experiment, we recommend employing the VGG 16 model for image data classification.
Increase Network Depth: To enhance results, consider expanding the neural network by adding more layers that further reduce dimensions for increased accuracy.
Diversify Training Data: Train the model on a larger dataset and different images to mitigate overfitting.
Introduce Development Set: Divide the data into three groups (train, test, and dev) to prevent overfitting and enhance model generalization.
