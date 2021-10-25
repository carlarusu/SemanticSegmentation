## Semantic Segmentation with three popular architectures on the ADE20k dataset

### General information
Image segmentation is the process of classifying each pixel in an image belonging to a certain class and hence can be thought of as a per prixel classification problem. Thus, the task of image segmentation is to train a neural network to output a pixel-wise mask of the image. Image segmentation has many applications in medical imaging, self-driving cars and satellite imaging to name a few.

### Dataset
The dataset used is the ADE20K Dataset which contains more than 20K scene-centric images exhaustively annotated with objects and object parts. Specifically, the dataset is divided into 20K images for training, 2K images for validation, and another batch of held-out images for testing. There are totally 150 semantic categories included for evaluation, which include stuffs like sky, road, grass, and discrete objects like person, car, bed. The type of data we are going to manipulate consist in:
- RGB jpg images
- 1 channel jpg masks where each pixel has a value from 0 to 150 defining its class
- 150 possible classes + 1 undefined

### Models
All experiments were carried out in Google Colab. The three models used for the experiments are:
- MobileNetV2
- UNet
- VGG16
