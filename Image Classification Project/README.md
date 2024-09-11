# Flower Species Classification with Transfer Learning

This project focuses on classifying different species of flowers using transfer learning techniques. The **Xception** model, pre-trained on the ImageNet dataset, was fine-tuned and adapted to classify the flower species in the provided dataset.

## Dataset - Flower Species

The dataset consists of images from 10 different flower species:
`class_names = ['Roses', 'Magnolias', 'Lilies', 'Sunflowers', 'Orchids', 'Marigold', 'Hibiscus', 'Firebush', 'Pentas', 'Bougainvillea']`.

The dataset is split as follows:
- **Training set**: 1,492 images
- **Test set**: 415 images

The flower species dataset is available for [download here](https://ufl.instructure.com/courses/459156/files/folder/Project%203/Dataset%201%3A%20Flower%20Species%20Classification).

## Transfer Learning with the Xception Model

In this project, we utilized the **Xception** model as the backbone of the CNN architecture. Xception, pre-trained on the ImageNet dataset, provides robust feature extraction capabilities learned from millions of diverse images.

### Model Customization
- **Input Layer**: A custom input layer was added to process the flower species dataset, ensuring the input dimensions matched our data.
- **Classifier**: Instead of using the original classifier layers pre-trained for ImageNet (which classifies over 1,000 categories), we created a custom classifier designed specifically for the 10 flower species in our dataset. This allows the model to focus on the smaller, more specific problem of flower classification.
  
### Freezing Weights
- **Frozen Xception Layers**: To maintain the powerful feature extraction capabilities of the pre-trained Xception model, we froze the weights of its middle layers. This means the pre-trained weights were not modified during training, preserving their knowledge from ImageNet.
- **Training the Custom Layers**: Only the custom input layer and the final classifier layers were trained on the flower species dataset. This approach significantly reduces training time while still benefiting from the deep feature extraction provided by Xception.
