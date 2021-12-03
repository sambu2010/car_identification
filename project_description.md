## Car Identification

### Abstract

The traditional vehicle recognition system relies on manual human observation or automated license plate recognition technique, these indirect progresses make the vehicle system hardly meets the real-time constraints. Through manual observation, it is practically difficult to remember and efficiently distinguish between the wide variety of vehicle makes and models. It becomes a laborious and time-consuming task for a human observer to monitor and observe the multitude of screens and record the incoming or outgoing makes and models or to even spot the make and model being looked for. This task can be automated by leveraging the Convolutional Neural Nets and Transfer Learning.

### Design

Create a deep learning model that will try to identify make and model of a particular car by looking at the picture of the car.

### Data

Dataset consists of 8218 pictures of 100 different classes of cars. All pictures have different sizes and different resolutions.

### Algorithms

Data is inspected after acquisition (images quality, folders structure)

Data is preproccesed using ImageDataGenerator. 

Baseline model is build using CNN. Baseline model consists of input layer, 3 sets of convolutional and max pooling layers, and 2 fully connected dense layers at the top. The accuracy of a base model is very low (~0,3).

Transfer learning is applied (InceptionV3 with the pretrained imagenet weights).

Tuning of the pretrained model is done after training to improve results (optimizer, batch size, learning rate, regularization tuning)

### Tools

- Pandas and Numpy are used for data cleaning and manipulation
- Sklearn and keras are used for modeling
- Matplotlib and Seaborn are used for visualization

### Communication

The jupyter notebook containing data and full analysis, and PP presentation are located in the GitHub repo folder for this project.
