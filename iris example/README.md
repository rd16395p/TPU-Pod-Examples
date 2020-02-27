# Iris Example

This is modfied code from the creaters of the code over at the [tpu repository.](https://github.com/tensorflow/tpu/tree/master/models/samples/core/get_started) I changed it to serve as an example of tensorflow code running on a TPU.

# How to run the code

Once you have finished setting up the enviroment, and creating the TPU Pod, I have ran the code by using the following command;

python TPU_Iris_Example.py --tpu="$TPU_NAME" --tpu_zone="$TPU_ZONE" --model_dir='gs://$BUCKET_NAME' --num_cores_per_replica=$TPU_NUMBER --batch_size=$TPU_NUMBER

My command using a v3-256 was as the following;

python3 TPU_Iris_Example.py --tpu="$TPU_NAME" --tpu_zone="$TPU_ZONE" --model_dir='gs://$BUCKET_NAME' --num_cores_per_replica=256 --batch_size=256

where I used python3 command to run my code. 
