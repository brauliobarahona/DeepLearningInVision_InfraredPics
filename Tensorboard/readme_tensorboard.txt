#import packages and libraries
import time
from tensorflow.keras.callbacks import TensorBoard

# define a variable with the name of your model
name = f"network_01_3-conv-64-layers-0-dense + {int(time.time())}"


# define a variable with the TensorBoard package, calling the defined name
tensorboard = TensorBoard(log_dir=f"logs/{name}")

# implement callback in your cnn.fit
network_1 = cnn.fit(
    		train_dataset,
    		epochs=20,
    		validation_data=val_dataset,
    		callbacks = tensorboard
		)

# code works only with the variables train_dataset and validation_data set correctly
# the compile and model build part is skipped
# the code above should generate: 
	log folder in the folder where the script is running
	the folder should contain for test and validation set each one folder with a v2 file

# further procedure:
open your shell of the environment, the script is running from
root to the folder which contains the log folder (not the log-folder itself!)
call: tensorboard --logdir=logs #logs is the name of the folder containing the v2 files
follow the instruction to open localhost:6006

Enjoy your Tensorboard!