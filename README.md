# Pneumonia-Detection
Experimenting various learning rates of different optimization functions and comparing them to VGG16


# CNN Model

The first attempt was a regular CNN model with 4 CNN layers. 
Dropout and L2 regaularization were also used to fight overfitting.
SGD was used as initial optimizer function with a lr = 1e-4
The model gave a training accuracy of 79% and val_accuracy of 79%.

# Experimentation with optimization functions and learning rates

Optimiization functions is one major tunable parameter which one always looks upto. Since the theorotical difference does not provide a concrete measure for the perfect optimization function for every problem, the best way is to experiment.
I have taken 3 optimization functions namely SGD, RMSProp and Adam optimization functions. Different learning rates from 1e-8 to 1e-3 were tested for all 3 optimizers using a learning rate scheduler.

# VGG16

The results were finally compared to the VGG16 model which gave a training accuracy of 90% and val accuracy of 80%.
The val_accuracy was quite similar to the custome model which shows that the model generalizes well and does not fall prey to overfitting.
