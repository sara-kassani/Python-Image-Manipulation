# Python-Image-Manipulation



from tensorflow.python.client import device_lib
print(device_lib.list_local_devices())

device_name = "/device:GPU:0"    


import tensorflow as tf
print(tf.test.gpu_device_name())
# See https://www.tensorflow.org/tutorials/using_gpu#allowing_gpu_memory_growth
config = tf.ConfigProto()
config.gpu_options.allow_growth = True
