# 神經網路設定

## 簡介
此為小小的作業，且因為訓練結果太差，找了一些可以增進訓練結果的資料。

## 引用源
`隱藏神經層數(HLC)、隱藏神經元數(HNC)` 設定皆採用自下列網頁。

ver2:
> https://www.linkedin.com/pulse/choosing-number-hidden-layers-neurons-neural-networks-sachdev

ver1:
> Kasperski, Andrzej. (2016). Re: How to decide the number of hidden layers and nodes in a hidden layer?. Retrieved from: https://www.researchgate.net/post/How-to-decide-the-number-of-hidden-layers-and-nodes-in-a-hidden-layer/581ce9f5eeae397d27799324/citation/download.


## Activation function setting
* ver1中，activation function是ReLU，但在ver2中改為較好的Swish。
* 原因：可以降低像是 Vanishing Gradient Problem 的發生。

## 架構設定
* 訓練資料使用`grades.csv`，皆採用one-hot encoding。
* ver1中，測試資料占0.4；ver2中，測試資料占0.3。

`InputDim = 56`, `OutputDim = 3` 

* ver1中，HLC=5, HNC由下列函數計算
<br>
![ver1 method](https://github.com/phantom0174/ck-110-2-ml/blob/main/%E4%BD%9C%E6%A5%AD2-2/img/ver1_method.png)
<br>

* ver2中，HLC=5, HNC由下列函數計算
<br>
![ver2 method](https://github.com/phantom0174/ck-110-2-ml/blob/main/%E4%BD%9C%E6%A5%AD2-2/img/ver2_method.png)
