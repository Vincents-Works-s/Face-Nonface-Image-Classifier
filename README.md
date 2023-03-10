# Facial-Image-Detection

Objective: Classify images as having a face or not having a face.

Model uses 3 convolutional layers, a flattening layer and finally a dense layer. It appears that convolutional layers are very powerful and are preferred over dense layers for image detection. l2 regularization was used only on the main dense layer.

Trained on 408 faces and 1751 nonfaces (mostly images of home interiors) that were gotten from search engine generated images.

I had difficulty making a model that generalizes well to completely random images. It overpredicted images as faces at an overwhelming rate, which seemed odd because I added more nonface images and retrained the model.
Another thing that was odd was that when training, the model actually consistently performed slightly better on the cross-validation set than the training set, and within a few epochs, the model achieved ~99% accuracy on the training, cross-validation, and test data, yet it feels like it was overfitting and not generalizing to new random samples.

Possibly the dataset was just too small? Or we needed more regularization or was the content of the images too different (different locations, different lighting)? For a general purpose task like classify images as face/noface, are insanely large datasets needed to achieve high performance? For a small dataset, maybe I can try to limit the images to a certain location. Wouldn't that specify the model for just that location and not generalize? Not sure how much training can be done with a macbook air... 
