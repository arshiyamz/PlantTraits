# PlantTraits
Kaggle PlantTraits Competition.

You can run the notebook cells one by one up to the second to last cell. This cell will attempt to run the model for 100 epochs, you must monitor the train and validation losses, and if they start diverging (i.e. overfit) or they stop decreasing, then you can stop the model's training early by just stopping the exectution. At this point, you can run the last cell, which will run the model on the test dataset and output the predictions to a csv file. Note that the model is checkpointed after each epoch, and the last cell automatically picks the checkpoint with the highest validation coefficient of determination.

Prereqs: numpy, torch, torchvision, PIL, scikit-learn.

The code also assumes that there is a cuda device available. Your cuda device needs at least 16GB VRAM in order to be able to fit the model and the data and perform the training.

My training was done on:
RTX 4080S - 16 GB VRAM
Xeon E5 CPU with 64 GB RAM
