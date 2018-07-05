# learn-pytorch
My examples for learning PyTorch written in Jupyter notebooks, adapted from [Chenyuntc's book](https://github.com/chenyuntc/pytorch-book).

## Contents
1. [pytorch_chapter02_basics.ipynb](https://github.com/GaoYang-Thu/learn-pytorch/blob/master/pytorch_chapter02_basics.ipynb) 介绍 pytorch 的基本知识和使用神经网络的流程。
2. [pytorch_chapter03_tensor.ipynb](https://github.com/GaoYang-Thu/learn-pytorch/blob/master/pytorch_chapter03_tensor.ipynb) 详细介绍 tensor 的操作，并且提供一个线性回归的经典例子。掌握这个例子，就基本足够了。
3. [pytorch_chapter03_autograd.ipynb](https://github.com/GaoYang-Thu/learn-pytorch/blob/master/pytorch_chapter03_autograd.ipynb) 详细介绍了 autograd 的细节，再次实现了经典线性回归的例子。
4. [pytorch_chapter04_nn.ipynb](https://github.com/GaoYang-Thu/learn-pytorch/blob/master/pytorch_chapter04_nn.ipynb) 详细介绍了 nn.Module 神经网络工具箱。首先，手把手帮你建立最简单的全连接层，然后介绍工具箱自带的标准层： `Linear`, `Conv2d`, `ReLU`, `MaxPool2d`等。接下来教你如何使用 `nn.Sequential()` 等方法将简单网络堆叠成大网络。最后综合上述知识，利用不到80行代码，实现了残差神经网络 ResNet34。我去掉了过时的 `Variable()` 方法，对 ResNet34 网络各层的参数做了详细注释。

## Comments
* 查阅官方文档后，我发现 `Variable(tensor)` 这种方法已经被官方弃用。想要得到一个能求导的 tensor，只需在新建 tensor 的时候声明要求导 `x = torch.ones((1,1),requires_grad = True` 就可以得到能求导的 tensor。关于这一点，我已经在教程页面提交了 [issue](https://github.com/chenyuntc/pytorch-book/issues/70)。



## _References_
1. [Chenyuntc's Pytorch Tutorial Book](https://github.com/chenyuntc/pytorch-book)
2. [PyTorch Official Docs](https://pytorch.org/docs)


## :sunglasses:
Happy coding!
