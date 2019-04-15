# Detection-on-Chest-X-Rays

diseases (14 diseases labels) Detection on Chest X-Rays image with Deep Learning (Convolutional Neural Network).



# training:
I randomly split the dataset into training (70%), validation (10%), and test (20%) sets (same chexnet), but I use an initial learning rate of 0.0001(and the chexnet use 0.001) that is decayed by a factor of 3 each time (for fast result) the validation loss plateaus after an epoch, and pick the model with the lowest validation loss.
I use inception-resnet-v2 instead of densnet121 (chexnet model). Also not to overfit I use 3-way image augmentation:
1. random flip 
2. random crop 
3. random rotate 

# result:
I have also proposed a slightly-improved model which achieves a mean AUROC of 0.852(v.s. 0.841 of the original CheXNet).
