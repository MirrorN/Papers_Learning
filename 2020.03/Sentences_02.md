## Sentences 02

[toc]

#### 1. Revisiting Low-Resource Neural Machine Translation: A Case Study

It has been shown that the performance of neural machine translation (NMT) drops starkly in low-resource conditions, underperforming phrase-based statistical machine translation (PBSMT) and requiring large amounts of auxiliary data to achieve competitive results. (可用作开头，表述NMT效果依赖于大量的额外数据，并且在 low-resource 的情况下比 PBSMT 的结果要差)

We discuss some pitfalls to be aware of when training low-resource NMT systems, and recent techniques that have shown to be especially helpful in low-resource settings, resulting in a set of best practices for low-resource NMT. (表述分析了一些 Low-Resource NMT 的问题所在以及一些有用的设置)

Our main contributions are as follows:

We explore best practices for low-resource NMT, evaluating their importance with ablation studies. (我们探讨了一些 low-resource NMT 的实践，评估了 ablation study 的重要性)

We reproduce a comparison of NMT and  PBSMT in different data conditions, showing that when following our best practices, NMT outperforms PBSMT with as little as 100 000 words of parallel training data. (我们重新比较了在不同的 data condition下的 NMT 和 PBSMT 的结果，XXX)

The bulk of research on low-resource NMT has focused on exploiting monolingual data, or parallel data involving other language pairs. (大量的XXX显示)

We expect that such a threshold reduces the need to carefully tune the vocabulary size to the dataset, leading to more aggressive segmentation on smaller datasets. (我们希望可以通过这样的阈值)

For comparison to previous work

Our results demonstrate that NMT is in fact a suitable choice in low-data settings, and can outperform PBSMT with far less parallel training data than previously claimed. (我们的结果证明XXX)

#### 2. Copied Monolingual Data Improves Low-Resource Neural Machine Translation

Specifically, we create a bitext from the monolingual text in the target language so that each source language is identical to the target sentence. (具体地，我们根据 target language 的 monolingual data 创建了bitext， XXXX)

Our proposed method proves to be an effective way of incorporating monolingual data into low-resource NMT. (我们的方法证明了将 monolingual data 加入到 low-resource NMT 中很有效)

In this paper, we introduce a straightforward method for adding target-side monolingual training data to an NMT system without changing its architecture or training algorithm. (我们引入了一种更直接的方式来将 monolingual data 加入到 NMT 中，而不需要改变原有的结构或者训练算法)

We focus on language pairs with small amounts of parallel data where monolingual data has the most impact. (我们关注的是那些只有很少 paralle data ，monolingual data 占较大影响的 language pairs)

This implies that back-translation does not make full use of monolingual data in low-resource settings which makes sense because it relies on low-resource translation in the reverse diection. (这意味着 back-translation 并没有充分利用 monolingual data)

Our method is similar, although instead of using a null source sentence, we use a copy of the target sentence and train the encoder parameters on the copied sentece. (表述自己的模型与之前的模型的区别)

We propose a method for incorporating target-side monolingual data into low-resource NMT that does not rely heavily on the amount or quality of the parallel data. (简述论文模型+最重要的功能/特点)



