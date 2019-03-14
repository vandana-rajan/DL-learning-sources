# DL-learning-sources and tricks and tips

Blog posts and tutorials for learning the nuances of DL.

1. https://medium.com/@jonathan_hui/deep-learning-designs-part-3-e0b15ef09ccc 

2. https://machinelearningmastery.com/visualize-deep-learning-neural-network-model-keras/ 

3. To get reproducible results every time you run your network, initialize seeds of random generators. Use the following.

import numpy as np

np.random.seed(7)

import random

random.seed(7)

from tensorflow import set_random_seed

set_random_seed(7)

Also, initialize weights of conv layers without randomness. Example, use 'glorot_uniform' which uses fan_in and fan_out as factors. 

