# BERT
Kaggle比赛获奖要求，Megatron框架，RAG,Agent技术框架，SFT,RAG
为什么BERT成功了？
在所有其他条件相同的情况下，掩蔽语言模型比从左到右的语言模型需要更多或更少的预训练步骤来收敛吗？为什么？
在BERT的原始实现中，BERTEncoder中的位置前馈网络（通过d2l.EncoderBlock）和MaskLM中的全连接层都使用高斯误差线性单元（Gaussian error linear unit，GELU） :cite:Hendrycks.Gimpel.2016作为激活函数。研究GELU与ReLU之间的差异。
在实验中，我们可以看到遮蔽语言模型损失明显高于下一句预测损失。为什么？
将BERT输入序列的最大长度设置为512（与原始BERT模型相同）。使用原始BERT模型的配置，如
。运行此部分时是否遇到错误？为什么？
为简单起见，句号用作拆分句子的唯一分隔符。尝试其他的句子拆分技术，比如Spacy和NLTK。以NLTK为例，需要先安装NLTK：pip install nltk。在代码中先import nltk。然后下载Punkt语句词元分析器：nltk.download('punkt')。要拆分句子，比如sentences = 'This is great ! Why not ?'，调用nltk.tokenize.sent_tokenize(sentences)将返回两个句子字符串的列表：['This is great !', 'Why not ?']。
如果我们不过滤出一些不常见的词元，词量会有多大？
huggging face相关书籍
