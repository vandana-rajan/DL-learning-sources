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

In PyTorch, use

torch.backends.cudnn.deterministic = True

torch.backends.cudnn.benchmark = False

torch.manual_seed(999)

4. Use ProgramCreek for example codes. Example https://www.programcreek.com/python/example/107694/torch.nn.LSTM 

5. For RNN-LSTM learning use https://www.youtube.com/playlist?list=PL1w8k37X_6L_s4ncq-swTBvKDWnRSrinI


