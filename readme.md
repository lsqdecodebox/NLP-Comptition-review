# NLP-Comptition-review




### jigsaw review

1. 学习使用tpu：  

   ​	从pytorch 到TensorFlow 

   ​	从tpu配置 到 训练过程  再到内存管理

2. 通过 masked language model (MLM)   finetuning 模型

3. 迁移学习：

   ​	few shot or zero shot

   ​	资料网站  http://transferlearning.xyz/

   ​	xlm-roberta  https://arxiv.org/abs/1911.02116

   ​	跨语言评测benchmark https://github.com/facebookresearch/XNLI

4. AUC metric 的 post-processing https://www.kaggle.com/c/tweet-sentiment-extraction/discussion/159910

### tweet extraction

1. 最让人抓狂的比赛（solve 噪声）

2. 对模型、优化器、loss、文本预处理（正则、符号编码等） 、训练、调参、seed、模型输出误差等有了整体的把握，什么是重要的，什么是不重要的

3. pre-processing 和 post-processing 的重要性，math magic！

4. 在数据噪声较大的情况下，运气好的seed带来的data order可以将噪声数据很好分开，带来提升。

   seed 重要性论文：https://arxiv.org/pdf/2002.06305.pdf

5. special head  ; end logit 根据start Logit信息来判定  XLNet使用过

6. beam search ，选择最优序列

### 疫情问答助手

1. 动态规划寻找最短路径
2. beam search寻找start和end span 配对
3. bm25粗召回







