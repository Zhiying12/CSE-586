# CSE-586 Project
   
## How to run it

1. Clone the project to your local computer and load the submodules
```
git clone <link to this repo>
cd <folder for this repo>
```

2. Install dependencies. Dependencies can be found in the requirements file.

3. To train the model, please run:
```
python main.py -v <version> --lr 0.002 --epochs 800 --batch-size 2048
```
The parameter `version` indicates the MoCo version you want to use to train your model.

4. If you want to test it with the pre-trained models, you can run:
```
python test.py -v <version> --resume <path to the pre-trained model>
```
The parameter `version` should be consistent with the version of the MoCo used to train the model. 
For a pre-trained model whose name is v1-xxx, you should set the version parametmer as "1": `-v 1`.

## References

Papers:
[MoCo-v1](https://arxiv.org/pdf/1911.05722.pdf), 
[MoCo-v2](https://arxiv.org/pdf/2003.04297v1.pdf),
[MoCo-v3](https://arxiv.org/pdf/2104.02057v3.pdf).

[MoCo-v1 and MoCo-v2 Code](https://github.com/facebookresearch/moco)

[MoCo-v1 on Colab](https://colab.research.google.com/github/facebookresearch/moco/blob/colab-notebook/colab/moco_cifar10_demo.ipynb)

[MoCo-v3 Skeleton Code](https://github.com/CupidJay/MoCov3-pytorch)

[MoCo-v3 Code](https://github.com/searobbersduck/MoCo_v3_pytorch)
