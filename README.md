1. install conda
2. build pytorch from source
3. `conda install nb_conda` so that you can choose the conda environment in `kernel` in Jupyter

At first I was getting `Illegal Instruction 4` when trying to run torch, then saw this [issue](https://github.com/pytorch/pytorch/issues/29967) telling me to try the nighly version, and it solved the problem for me.

After installation, the base environment should have already been created. Use `conda activate` to activate the environment. Open a python interpreter. Check where the pytorch library is located in the environment:
```
import torch
print(torch.__file__)
```
Do the same in Jupyter to make sure they are the same. 

