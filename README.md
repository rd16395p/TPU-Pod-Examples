# TPU-Pod-Examples

[Tensorflow Research Cloud](https://www.tensorflow.org/tfrc/)

Research supported with Cloud TPUs from Google's TensorFlow Research Cloud (TFRC). 

# Contents of this repository 

- Example iris code from the [tensorflow tpu repository](https://github.com/tensorflow/tpu/tree/master/models/samples/core/get_started) that has been modified to work on pods. This is found under 'iris example' folder. Instructions on how to run the code is found there as well.

- (Coming Soon!) Code from my master's thesis project titled "emotionnet". This will be added as soon as the paper is published!

# How to get any Google Compute Engine VM set up for use with TPU Pods

First, make sure that the GCE VM is set up with all permissions enabled to access the [tpu pods.](https://github.com/tensorflow/tpu/issues/596)

This can be done through the gui by clicking the name of the VM under VM instances. I would recommend creating the VM instance in the same zone as the TPU pod as it is easier to set up to the connection to the pod. 

Second, make sure that the packages are also installed on the VM instance. For these examples, I would install pandas and tensorflow 1.14. There will also be text that will appear stating to download new packages. Install the packages by following the dialog that appears. I woud also ensure that the TPU Pod software version is 14.0, matching the tensorflow version. These commands are `pip install --upgrade google-api-python-client` and `pip install --upgrade oauth2client`. 

# Other related guides I found helpful 

[TPU Pod Documentation](https://cloud.google.com/tpu/docs/training-on-tpu-pods)
