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

5. special head ： end logit 根据start Logit信息来判定， XLNet for QA使用过改方式

6. beam search ，选择最优序列

7. jaccard分数提高 https://www.kaggle.com/c/tweet-sentiment-extraction/discussion/158613

8. 用候选答案文本和jaccard分数 再训练模型，maybe为了信息完整性吧

9. SequenceBucketing释义： 要对`sequence`的长度聚类，确保将相近长度文本分配到同一个`bucket`

### 疫情问答助手

1. 动态规划寻找最短路径，用于将长文本縮减为 相交且最短的序列
2. beam search 寻找start和end span 最优配对
3. bm25粗召回



### Google QUEST Q&A 

1. KL散度 vs 交叉熵，交叉熵胜利
2. spearman 评估，及调优策略
3. 可靠的 cv 验证方法
4. 截取过长文本首尾部分，保证最大有效数据输入
5. Pseudo-label
6. multi-sample dropout
7. 模型内的超参 给 自适应调节



### TODO

ai研习社-耶鲁大学文本转SQL 

NL2SQL

GNN on 知识图谱



