# SF-crime-Pytorch

Fight crime with Pytorch!

## 下载数据

https://www.kaggle.com/c/sf-crime/data

数据应当存放于/input/sf-crime中

## 输出的模型

/working/net(v4).pkl，是PyTorch的CUDA的模型，CPU玩家自行转换，另载入模型需要声明类Residual和build-model。

另外，在 https://www.kaggle.com/doublepoi/a-nn-with-residual-v4 有notebook。

/working/gbm(v1).pkl，是LightGBM的模型，v2由于大小原因，未上传。

另外，在 https://www.kaggle.com/doublepoi/lightgbm-test-4 有v2的notebook。

## 目录

[一、项目搭建](https://gitee.com/Double-POI/SF-crime-Pytorch/blob/master/%E6%97%A7%E9%87%91%E5%B1%B1%E7%8A%AF%E7%BD%AA%E5%88%86%E7%B1%BB%E9%A2%84%E6%B5%8B%E6%A8%A1%E5%9E%8B%E7%A0%94%E7%A9%B6/1%E3%80%81%E9%A1%B9%E7%9B%AE%E6%90%AD%E5%BB%BA/1%E3%80%81%E9%A1%B9%E7%9B%AE%E6%90%AD%E5%BB%BA.md)

[二、数据的可视化分析](https://gitee.com/Double-POI/SF-crime-Pytorch/blob/master/%E6%97%A7%E9%87%91%E5%B1%B1%E7%8A%AF%E7%BD%AA%E5%88%86%E7%B1%BB%E9%A2%84%E6%B5%8B%E6%A8%A1%E5%9E%8B%E7%A0%94%E7%A9%B6/2%E3%80%81%E6%95%B0%E6%8D%AE%E7%9A%84%E5%8F%AF%E8%A7%86%E5%8C%96%E5%88%86%E6%9E%90/2%E3%80%81%E6%95%B0%E6%8D%AE%E7%9A%84%E5%8F%AF%E8%A7%86%E5%8C%96%E5%88%86%E6%9E%90.md)

[三、数据的清洗及格式化](https://gitee.com/Double-POI/SF-crime-Pytorch/blob/master/%E6%97%A7%E9%87%91%E5%B1%B1%E7%8A%AF%E7%BD%AA%E5%88%86%E7%B1%BB%E9%A2%84%E6%B5%8B%E6%A8%A1%E5%9E%8B%E7%A0%94%E7%A9%B6/3%E3%80%81%E6%95%B0%E6%8D%AE%E7%9A%84%E6%B8%85%E6%B4%97%E5%8F%8A%E6%A0%BC%E5%BC%8F%E5%8C%96/3%E3%80%81%E6%95%B0%E6%8D%AE%E7%9A%84%E6%B8%85%E6%B4%97%E5%8F%8A%E6%A0%BC%E5%BC%8F%E5%8C%96.md)

[四、传统机器学习（其一）](https://gitee.com/Double-POI/SF-crime-Pytorch/blob/master/%E6%97%A7%E9%87%91%E5%B1%B1%E7%8A%AF%E7%BD%AA%E5%88%86%E7%B1%BB%E9%A2%84%E6%B5%8B%E6%A8%A1%E5%9E%8B%E7%A0%94%E7%A9%B6/4%E3%80%81%E4%BC%A0%E7%BB%9F%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%EF%BC%88%E5%85%B6%E4%B8%80%EF%BC%89/4%E3%80%81%E4%BC%A0%E7%BB%9F%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%EF%BC%88%E5%85%B6%E4%B8%80%EF%BC%89.md)

[五、单层神经网络](https://gitee.com/Double-POI/SF-crime-Pytorch/blob/master/%E6%97%A7%E9%87%91%E5%B1%B1%E7%8A%AF%E7%BD%AA%E5%88%86%E7%B1%BB%E9%A2%84%E6%B5%8B%E6%A8%A1%E5%9E%8B%E7%A0%94%E7%A9%B6/5%E3%80%81%E5%8D%95%E5%B1%82%E7%A5%9E%E7%BB%8F%E7%BD%91%E7%BB%9C/5%E3%80%81%E5%8D%95%E5%B1%82%E7%A5%9E%E7%BB%8F%E7%BD%91%E7%BB%9C.md)

[六、多层神经网络（其一）](https://gitee.com/Double-POI/SF-crime-Pytorch/blob/master/%E6%97%A7%E9%87%91%E5%B1%B1%E7%8A%AF%E7%BD%AA%E5%88%86%E7%B1%BB%E9%A2%84%E6%B5%8B%E6%A8%A1%E5%9E%8B%E7%A0%94%E7%A9%B6/6%E3%80%81%E5%A4%9A%E5%B1%82%E7%A5%9E%E7%BB%8F%E7%BD%91%E7%BB%9C%EF%BC%88%E5%85%B6%E4%B8%80%EF%BC%89/6%E3%80%81%E5%A4%9A%E5%B1%82%E7%A5%9E%E7%BB%8F%E7%BD%91%E7%BB%9C%EF%BC%88%E5%85%B6%E4%B8%80%EF%BC%89.md)

[七、Kernels计算资源的使用](https://gitee.com/Double-POI/SF-crime-Pytorch/blob/master/%E6%97%A7%E9%87%91%E5%B1%B1%E7%8A%AF%E7%BD%AA%E5%88%86%E7%B1%BB%E9%A2%84%E6%B5%8B%E6%A8%A1%E5%9E%8B%E7%A0%94%E7%A9%B6/7%E3%80%81Kernels%E8%AE%A1%E7%AE%97%E8%B5%84%E6%BA%90%E7%9A%84%E4%BD%BF%E7%94%A8/7%E3%80%81Kernels%E8%AE%A1%E7%AE%97%E8%B5%84%E6%BA%90%E7%9A%84%E4%BD%BF%E7%94%A8.md)

[八、多层神经网络（其二）](https://gitee.com/Double-POI/SF-crime-Pytorch/blob/master/%E6%97%A7%E9%87%91%E5%B1%B1%E7%8A%AF%E7%BD%AA%E5%88%86%E7%B1%BB%E9%A2%84%E6%B5%8B%E6%A8%A1%E5%9E%8B%E7%A0%94%E7%A9%B6/8%E3%80%81%E5%A4%9A%E5%B1%82%E7%A5%9E%E7%BB%8F%E7%BD%91%E7%BB%9C%EF%BC%88%E5%85%B6%E4%BA%8C%EF%BC%89/8%E3%80%81%E5%A4%9A%E5%B1%82%E7%A5%9E%E7%BB%8F%E7%BD%91%E7%BB%9C%EF%BC%88%E5%85%B6%E4%BA%8C%EF%BC%89.md)

[九、传统机器学习（其二）](https://gitee.com/Double-POI/SF-crime-Pytorch/blob/master/%E6%97%A7%E9%87%91%E5%B1%B1%E7%8A%AF%E7%BD%AA%E5%88%86%E7%B1%BB%E9%A2%84%E6%B5%8B%E6%A8%A1%E5%9E%8B%E7%A0%94%E7%A9%B6/9%E3%80%81%E4%BC%A0%E7%BB%9F%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%EF%BC%88%E5%85%B6%E4%BA%8C%EF%BC%89/9%E3%80%81%E4%BC%A0%E7%BB%9F%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%EF%BC%88%E5%85%B6%E4%BA%8C%EF%BC%89.md)

## 源代码

位于/src目录下。

## 总结

此程序还存在改进空间，但是家中计算资源有限，调参有很大困难，见谅。