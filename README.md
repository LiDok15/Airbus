# Airbus
This repo contains my attempt to solve the problem of recognition ships using tf.keras for training UNet.

The competition aims to study satellite pictures of container ships and create masks that outline the ships' shapes.

First, we have to download the data from [here](https://www.kaggle.com/competitions/airbus-ship-detection/data?select=train_ship_segmentations_v2.csv) and store it in the base dir.  
` - train_v2 
  - test_v2
  - train_ship_segmentations_v2.csv
  - sample_submission_v2.csv`

The solution consists of one jupyter notebook. There, loading and displaying of data, decryption of the RLE code for displaying the mask is implemented. There is implemented:

- Loading and displaying of data
- Decryption of the RLE code for displaying the mask
- Demonstrated data imbalance (the best way to solve this problem is to reduce the number of images without ships or remove them altogether)
- Given theoretical information about the task, the U-Net model and the Dice coeficient.
- Given the construction of the U-net model.

Since I am not yet very good at processing data in the form of images and working with tensorflow, I borrowed some functions from notebooks of other developers. I left all links to these works.

Due to the difficulties that I encountered during the implementation of this project, I could not finish it. Namely the part with model training and prediction. The more I delved into how to deal with this problem, the more I needed to use someone else's code, and the harder it was for me to understand that code. 
I think it is necessary to take a break for a while and look at the competition with new eyes after a few days :)
