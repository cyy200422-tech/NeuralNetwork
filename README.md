# NeuralNetwork-MNIST (C++)
### 项目简介
本项目是一个 基于 C++ 实现的简单神经网络Neural Network的图像分类实践项目，使用 MNIST 手写数字数据集，实现从数据读取、训练到预测的完整流程。
项目不依赖深度学习框架（如 PyTorch / TensorFlow），而是用手写实现矩阵运算、前向传播、反向传播和 SGD 训练过程，适合理解神经网络的底层原理。
### 项目功能
读取 MNIST 数据集（idx3-ubyte / idx1-ubyte）
对图像数据进行归一化和向量化
构建全连接神经网络
使用 SGD（随机梯度下降） 进行训练
对测试集进行预测并输出结果
支持从文件加载网络结构（.cxnn）
### 技术流程
MNIST 数据集👉数据读取（idx 文件解析）👉数据预处理（归一化 / 向量化）👉神经网络模型（前向传播）👉训练（反向传播 + SGD）👉测试与预测（输出预测值与真实值）
### 注：
NN 为神经网络的对象
SGD 为训练
LoadNetworkStructure() 为读取训练模型
feedforward 为识别
#### 关于图片：
<img width="1134" height="674" alt="image" src="https://github.com/user-attachments/assets/19d48d91-8301-43bf-b659-a4ae8861b871" />

### 编译运行
1. 新建 build 文件夹，并进入
2. cmake ..
3. make
4. 拷贝 cx.cxnn t10k-images.idx3-ubyte t10k-labels.idx1-ubyte train-images.idx3-ubyte train-labels.idx1-ubyte 到 build 下
5. 运行
