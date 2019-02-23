------
README
------

DenoiseNet and Unet

###################
 Code instructions
###################


--------------------------
 DenoiseNet Parameters Configuration
--------------------------

-------------------------------------------------
configure Parameters variable in the Main cell:
-------------------------------------------------


1. 'weights_path' - name of weights to load
2. 'noise_sigma' - sigma of the additive gaussian noise.
3. 'load_weights_flag' - load saved weights or not.
4. 'train_or_test' - if 1 training will be performed, if zero it will test the network.
5. 'mode' - flag, if its 0, it will load the images with real noise, while both images clean, and noisy are at the same directory, and 'gt_suf', and 'noise_suff' parameters determine 
	which images are noisy and which are clean (images should have the same name except the suffix).   
6. 'gt_suf' - string, ground truth images suffix, if 1 it will load a directory of clean images, and add a gaussian i.i.d noise sigma = 'noise_sigma'. 
7. 'noise_suf' - string, noisy images suffix
8. 'im_type' - images type for example 'jpg'
   
--------------------------
 Unet Parameters Configuration
--------------------------

-------------------------------------------------
configure Parameters variable in the Main cell:
-------------------------------------------------

1. 'weights_path' - name of weights to load
2. 'noise_sigma' - sigma of the additive gaussian noise.
3. 'load_weights_flag' - load saved weights or not.
4. 'train_or_test' - if 1 training will be performed, if zero it will test the network.
5. 'mode' - flag, if its 0, it will load the images with real noise, while both images clean, and noisy are at the same directory, and 'gt_suf', and 'noise_suff' parameters determine 
	which images are noisy and which are clean (images should have the same name except the suffix).   
6. 'gt_suf' - string, ground truth images suffix, if 1 it will load a directory of clean images, and add a gaussian i.i.d noise sigma = 'noise_sigma'. 
7. 'noise_suf' - string, noisy images suffix
8. 'im_type' - images type for example 'jpg'
9. 'lr' - learning rate
10. 'epoch_num' - number of epochs to train
11. 'model_dir' - directory to save the model


notice - visdom is not working properly on google colab 
--------------------
How to run the code:
--------------------

for both notbooks, run all and mound the google drive when requested

