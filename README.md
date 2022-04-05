#### Monitoring NVIDIA GPU
```
nvidia-smi
```

#### To check CUDA version
```
nvcc --version
```

#### To resolve out of memory error in Tensorflow 2.
```
from tensorflow.compat.v1 import ConfigProto
from tensorflow.compat.v1 import InteractiveSession
config = ConfigProto()
config.gpu_options.allow_growth = True
session = InteractiveSession(config=config)
```
