# Face Verification Computer Vision
Final Project of the course taken at Shahid Beheshti University

This face verification system is implemented by fine-tuning Facenet (Inception ResNet v1) using the Labeled Faces in the Wild (funneled) dataset. We have added some layers at the end of the Facenet layer to create a Siamese network. Then, we have constructed a dataset from images in the database, ensuring that we have positive and negative pairs to train the network. The Contrastive Loss function is used because it is a Siamese network and there is a limited number of images for each person. Training is halted from layers 0-300, and the rest are trained, which means 13M parameters out of 22M are being trained.
