# DLproject2024_4guys
此存储库用于存放开发过程中的代码，记录开发过程，提交代码时务必写明提交原因，写明注释~

## 日志

- 🚩**News**
- 🚩(2024.11) 
  - 2024.11.18: 整理整个项目的文件框架，写明注释以及说明
  - 2024.11.19: 中期报告
- 🚩(2024.10): The repositiory was built up.


## 项目介绍

对于一些寿命相对较长（比如10年、20年）的电子原件，
我们不可能真的对其测试10年、20年， 
于是我们需要对其寿命进行预测

在本项目中，被预测的对象是一类微波电子管，
这类微波电子管需要在特定条件下，能够长期将电流保持在某个期望的数值。
随着使用时间的增加，电流会越来越小，**如果电流相对与期望的数值，
减小了10%，则此微波电子管的被视为报废**

所以，我们的任务是，预测该微波电子管的电流变化，并判断何时下降10%，**则此下降10%的时间为其寿命**。
为了让模型更好地学习到此时间序列的规律，我们需要大量的数据预处理工作
我们在自定义数据集上对Autoformer模型进行了微调和优化，同时对比了其他传统模型LSTM、GRU、TCN等的预测性能。

### 文件夹架构（等待进一步补充完整）
- baseline(数据集以及传统模型）
  -  data:数据集
  -  sourceModel:传统模型
  -  DataProcess.igynb:数据处理代码
  -   sourceModel.igynb:传统模型训练
  -   TransferModel.igynb:传统模型测试
- improved method(Autoformer模型训练及测试）
  -  autoformer.igynb:Autoformer模型训练及测试  
- author-kit-CVPR2025-v3.1-latex-: latex模板
- `.gitignore`: 对于会在运行后生成的file，不需要把他上传到github。为避免上传时自动上传、导致将此类文件包含在内，应该将其文件路径包含在`.gitignore`文件中
## 项目模型

### 模型介绍： Autoformer
- 模型代码/预训练模型：[huggingface/MRNH/autoformer-ett-hourly]([(https://huggingface.co/MRNH/autoformer-ett-hourly)])

## 使用方法
- 下载项目。
- 运行对应igynb文件夹中的代码，完成模型训练与测试（需更改数据集路径）。
