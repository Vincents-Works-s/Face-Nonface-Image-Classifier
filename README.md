# Facial-Image-Detection

Dataset that is "nonfaces" is really skewed. It only consists of interior home photos. Therefore the model overfits images of those type and fails to accurately predict images without faces and aren't inside homes.

Model uses 3 convolutional layers, a flattening layer and finally a dense layer. It appears that convolutional layers are very powerful and are preferred over dense layers for image detection.

The project was based on a tutorial on Youtube: https://www.youtube.com/watch?v=jztwpsIzEGc&ab_channel=NicholasRenotte 
