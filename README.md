# From DnCNN to UDnCNN and DUDnCNN

ReLU
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/joseph-cheung/From-DnCNN-to-UDnCNN-and-DUDnCNN/blob/main/%E4%BB%8E_DnCNN_%E5%88%B0_UDnCNN_%E5%86%8D%E5%88%B0_DUDnCNN_%E7%9A%84%E5%9B%BE%E5%83%8F%E9%99%8D%E5%99%AA.ipynb)

Leaky_ReLU
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/joseph-cheung/From-DnCNN-to-UDnCNN-and-DUDnCNN/blob/main/DnCNN_UDnCNN_DUDnCNN_with_LeakyReLU.ipynb)

# DnCNNs with ReLU/Leaky_ReLU Activation

Models trained with CUDA, batch = 4, after 200 epochs each.  

No statistically significant [improvement](https://ieeexplore.ieee.org/document/9350117) with Leaky_ReLU in replace of ReLU, period.

### Raw DnCNNs with ReLU Activation

| Eval / CNNs | DnCNN       | UDnCNN      | DUDnCNN     |
| ----------- | ----------- | ----------- | ----------- |
| **PSNR**    | 29.0762     | 28.4196     | 29.3118     |
| **Loss**    | 0.005108381 | 0.005901728 | 0.004859959 |

![1](1.png)



### "Improved?" DnCNNs with Leaky_ReLU Activation

| Eval / CNNs | DnCNN             | UDnCNN            | DUDnCNN           |
| ----------- | ----------------- | ----------------- | ----------------- |
| **PSNR**    | 29.0926 **↑**     | 28.3110 **↓**     | 29.1659 **↓**     |
| **Loss**    | 0.005087597 **↓** | 0.006038793 **↑** | 0.005011519 **↑** |

![2](2.png)


###三种网络的比较
