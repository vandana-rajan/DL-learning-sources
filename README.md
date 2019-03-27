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

5. For RNN-LSTM learning use Andrew Ng's lectures at https://www.youtube.com/playlist?list=PL1w8k37X_6L_s4ncq-swTBvKDWnRSrinI
   and Christopher Olah's blog http://colah.github.io/posts/2015-08-Understanding-LSTMs/
   
6. An intuitive explanation of cross-entropy loss https://towardsdatascience.com/understanding-binary-cross-entropy-log-loss-a-visual-explanation-a3ac6025181a

7. L0,L1,L2 and L-infinity norms: https://medium.com/@montjoile/l0-norm-l1-norm-l2-norm-l-infinity-norm-7a7d18a4f40c and https://rorasa.wordpress.com/2012/05/13/l0-norm-l1-norm-l2-norm-l-infinity-norm/

8. A bit of history about phonetically balanced sentences: https://gizmodo.com/the-harvard-sentences-secretly-shaped-the-development-1689793568 [Not exactly related to DL but audio engineering.]

9. Bias-Variance Trade Off: https://en.wikipedia.org/wiki/Bias%E2%80%93variance_tradeoff


