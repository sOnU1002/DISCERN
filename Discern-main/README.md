# Discern
    An AI-powered solution for accurate disease prediction and noise elimination using filters in Chest X-rays. Providing a radiologist-like second opinion, it enhances reliability in diagnosing common chest diseases.
X-rays are an important tool in modern medicine, allowing doctors to detect and treat a wide range of illnesses. Despite its extensive use, noise in medical imaging remains a prevalent issue that can have a substantial impact on diagnostic image quality and accuracy. Noise is ubiquitous and unavoidable in images produced by medical imaging equipment. Currently, DSIP methods are used for noise reduction, but as AI advances, it will be possible to train the machine to diagnose the patient's underlying health condition after the X-ray image is made clearer with less noise making it easier for the AI to diagnose the patient.

Discern is an AI-powered medical image diagnosis system. It is designed to analyze medical images, specifically Chest X-rays, and provide an accurate diagnosis of the underlying health condition. The system utilizes deep learning algorithms to analyze the images and provide a diagnosis with high accuracy.
The python library gradio is used to provide the GUI for our AI and its in the form of a hosted website which uses our AI to remove the noise and diagnose the patient.
The user has to upload an Image which is then cleared using various filters and techniques and then the image is used as an input in our model who the diagnosis or rather classifies the image into normal or a percentage of probable diseases.
For the AI, we utilized various libraries for ML models, data manipulation and processing, and data visualization, such as TensorFlow, keras, numpy, sklearn, PIL, matplotlib, seaborn, and plotly.
To address the problem of imbalanced data, we used the variants of the images in the dataset by transforming them, changing their orientation, etc and other similar mentors which are generally used to remove the bais
The system has the potential to significantly improve the accuracy of medical image diagnosis and provide a valuable tool for healthcare practitioners in diagnosing various health conditions.


## Objective
- Improve diagnostic accuracy: By removing noise from medical images, the system can provide clearer and more accurate images as input, enabling the AI to identify the disease more accurately
-  Improve efficiency: The AI system can help medical practitioners make faster and more accurate diagnoses, resulting in more efficient patient care.
- Increase access to medical diagnosis: Because AI systems can remove noise from images and diagnose patients, they can enable access to medical diagnosis in locations where medical specialists may not be readily available.

## Scope
- Image acquisition and processing: Our AI GUI has a drag and drop mechanism through which the user can upload x-ray images for diagnosing. The image is then desnoised and placed into our model for processing and diagnosing.
- Noise reduction approaches: To reduce the presence of noise in the chest X-ray pictures, Discern uses advanced noise reduction techniques and Filters such as Gaussian filter, Median filter etc.
- AI model training: To effectively recognise and classify numerous abnormalities and diseases, the AI model must be trained on a huge dataset of chest X-ray pictures using a variant of Vgg16 algorithm.


## Tech/ Requirements
- Jupyter Notebook
        Jupyter Notebook is particularly favorable in the creation of AI due to its collaborative environment, reproducibility, visualization capabilities, interactivity, integration with other tools and platforms, and ease of use. 

- Open CV
		Image and video processing is one of the most prominent OpenCV 	applications in AI projects. OpenCV is an extremely powerful and versatile tool for AI developers. Its versatility and ease of use.
	
- Tensorflow-keras
	    TensorFlow with Keras offers a complete and powerful framework for constructing deep learning models. TensorFlow provides the foundational capability for developing and training artificial neural networks, but Keras streamlines the process by providing a high-level interface. TensorFlow and Keras can be used by developers to build complicated deep learning models such as convolutional neural networks (CNNs), recurrent neural networks (RNNs), and generative adversarial networks (GANs), among others. 

- Other python libraries such as gradio, pytorch, matplotlib, etc.

## Model

The AI model I employed was a variation of the VGG16 model, meticulously trained on a comprehensive chest X-ray dataset readily available on Kaggle.

## Result

UI for input & output 
 ![Image](https://github.com/Kunj-Pate1/Discern/blob/main/output%20imgs/input.png) 
| Pneumonia | Tuberculosis |
| --- | --- |
| ![Image 1](https://github.com/Kunj-Pate1/Discern/blob/main/output%20imgs/pneumonia.png) | ![Image 2](https://github.com/Kunj-Pate1/Discern/blob/main/output%20imgs/tuber.png) |

| Covid | Normal |
| --- | --- |
| ![Image 3](https://github.com/Kunj-Pate1/Discern/blob/main/output%20imgs/covid.png) | ![Image 4](https://github.com/Kunj-Pate1/Discern/blob/main/output%20imgs/normal.png) |
