# ORDERED-NEURONS-INTEGRATING-TREE-STRUCTURES-INTO-RECURRENT-NEURAL-NETWORKS--tensorflow
tensorflow实现的ordered_neurons_Lstm,原始论文：https://arxiv.org/pdf/1810.09536.pdf。
根据tensorflow中LSTM源代码的实现，修改而成的。

使用方式和一般的LstmCell一样,把tf.nn.rnn_cell.BasicLSTMCell换成文件中的ON_LSTM类就行,然后 tf.nn.bidirectional_dynamic_rnn或 tf.nn.dynamic_rnn
就可以了。
这个论文介绍了神经元排序的问题，通过神经元排序，能更好的学习到句子之中的层次结构。
