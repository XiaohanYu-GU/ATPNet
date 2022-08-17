# ATPNet


### Implmentation
We initialize our model by the ImageNet pre-trained model. For new parameters, they are randomly initialized. The input images are resized to $256 \times 256$ for CelebA and $448 \times 448$ for the remaining datasets. We augment the datasets with random crop, random horizontal flipping, and color jittering. In our experiment setting, the batch size is set to $32$. 
We use the SGD optimizer to train our model. The base learning rate is initialized at $5e-3$ for CelebA and $1e-3$ for the remaining datasets. In the following experiments, the number of parts is set to 5, $\theta$ is set to be $\theta = 0^ \circ$, $\alpha$, $\beta$ and $\gamma$ is set to 0.1, 0.01, 0.5 unless specified. At the inference stage, results are reported by using center crop operation. All experiments are implemented with PyTorch framework on one Nvidia V100 GPU.

### How to use
install pytorch 1.6.0, python 3.7, cuda 10.1, cudnn7.6.3 and any necessary python package that is required.

Use the following order to run the training code in a default setting.

"sh main.sh"

Or revise the hyper-parameters (batch size, learning rate) in config.py if needed and then run "sh main.sh".



### Acknowledgement
The code is revised based on source code provided by (see "https://github.com/zxhuang1698/interpretability-by-parts"). We sincerely thank their contribution.


## Author contact info
*Xiaohan Yu*, *yuxiaohan112@gmail.com*


## Code
The code is being organized and will be released soon.
