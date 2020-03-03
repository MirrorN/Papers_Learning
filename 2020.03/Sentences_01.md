## Sentences 01

[toc]

#### 1. Tree-LSTM

However, natural language exhibits syntactic properties that would naturally combine words to phrases.(表述句法结构信息更自然地将单词组合成短语)

Order-insensitive models are insufficient to fully capture the semantics of natural language due to their inability to account for differences in structures. (表述XXXX的模型无法很好的捕捉语言的语义信息，这是因为他们无法解释不同的结构)

In this paper, we work towards addressing this question by directly  comparing a type of XXX. (我们的模型通过直接XXXX解决了这一问题)

#### 2. NMT of Rare Words with Subword units

We note that such techniques make assumptions that often do not hold true in practice.(表述我们发现这些技术在实际中并不总是正确的)

This paper has two main contributions:(表述本文的主要贡献有：(列表))

The main motivation behind this paper is that the translation of some words is transparent in that they are translatable by a competent translator even if they novel to him or her.(阐述论文观点的灵感来源)

####  3.Revisiting Low-Resource Neural Machine Translation: A Case Study

It has been shown that the performance of neural machine translation (NMT) drops starkly in  low-resource conditions, underperforming phrase-based statistical machine translation (PBSMT) and requiring large amounts of auxiliary data to achieve competitive results. (表述 NMT 在低资源的条件下效果下降很快，效果不如基于短语的 SMT，为了达到很好的效果，必须要使用很多额外的数据)

While the trend in high-resource settings is towards using larger and deeper models, XXX use smaller and fewer layers for smaller datasets. (在 high-resource 的数据处理中使用的是 larger的)

While seim-supervised and unsupervised dapproaches have been shown to be very effectivev for some language pairs, their effectiveness depends on the availability of large amounts of suitable auxiliary data, and other conditions being met.(表述尽管半监督学习以及无监督学习在一些语言非常有效，但是这些效果的提升依然是依赖于大量的、辅助的合适数据以及其他条件)

To simulate different amounts of training resources, we randomly subsmaple the IWSLT training corpus 5 times, discarding half of the data at each step.(表述 为了估计XXXX， 我们随机的在数据集中进行采样，并且每次都数量减半)

In the ultra-low data conditiion, reducing the BPE vocabulary size is effectivev.(表述在XXX的条件下，是非常有效的)

For simplicity (为了简单起见)

For comparison to previous work.

Our results far outperform the RNN-based results reported by XXX， and are on par with the bast reported results on this dataset.(我们的结果远远超出了XXX， 并且与这个数据集最好的结果等同 (be on par with 与...同等水平)) 



#### 3.Improving Neural Machine Translation Models with Monolingual Data

Neural Machine Translation (NMT) has obtained state-of-art performance for several language pairs, while only using parallel data for training. (经典开头，表述NMT的发展现状以及注意很多时候都会使用 language pair 表示语言之间的翻译)

In contrast to previous work,  which combines NMT models with separately trained language models, we note that encoder-decoder NMT architectures already have the capactiy to learn the same information as a language model, and we explore strategies to train with monolingual data without changing the neural network architecture.

We obtain substantial improvements on XXX dataset. (表述在某个数据集上获得了很大的提升)

We follow the neural machine translation architecture by Bahdanau et at.(2015) , which we will briefly summarize here.(表述将要使用的主体结构，接下来我们将会简要的介绍)

C(i) is computed as a weighted sum of the annotations h(j). (表述 注意力机制的向量计算，作为加权和)

Including syntactic data during training is very effective, and yields an improvement over out baseline by 2.8-3.4 BLEU.(表述加入了XXX的信息之后效果非常明显，并且带来了相较于 baseline 的XXX的BLEU提升)

We also subtaintially outperform NMT results reported by Jean et al.(2015a) and Luong et at.(2015),who previously reported SOTA result.(表述我们的结果超过了之前XXX提出的XXX的模型的结果)

#### 4.Semi-Supervised Learning for Neural Machine Translation

While end-to-end neural machine translation (NMT) has made remarkable progress recently, NMT systems only rely on parallel corpora for parameter estimation.

We propose a semi-supervised approach for training NMT models on the concatenation of labeled (parallel corpora)  and unlabeled (monolingual corpora) data (表述基于XXXX数据提出了XXX方法)

Our approach can not only exploit the monolingual corpora of the target language,but also of the source language. (表述本文的方法的提升之处：不仅XXX还XXX)

However, most existing NMT approaches suffer from a major drwback: they heavily rely on parallel corpora for training translation model.(表述NMT的问题所在)

It is appealing to explore the more reradily available abundant monolingual corpora to improve NMT.(用于从NMT到增加使用monolingual data 的改进模型)





#### 5.Using Target-side Monolingual Data for Neural Machine Translation through Multi-task Learning

The performance of Neural Machine Translation(NMT) models relies on the availability of sufficient amounts of parallel data, and an efficient and effective way of leveraging the vastly available amounts of monolingual data has yet to be found.(表述 NMT 目前的优秀表现得益于数量庞大的平行语料，并且对于单语语料的有效使用方法仍然在一直探索)

The decoder predicts the next target word through two channels, a target-side language model on the lowest layer, and an attentional recurrent model which is conditioned on the source representation.(表述 模型的主要结构，  注意XXX是取决于XXX的表述)

Initial results in the news domain for three language pairs show moderate but consistent improvements over a baseline trained on bilingual data only.(表述初步的载新闻领域的结果显示有少量但是稳定的提升)

In recent years, neural encoder-decoder models have signigicantly advanced the state of the art in NMT, and now consistently outperform Statistical Machine Translation(SMT).（表述NMT相较于SMT的进步，可以用在 Introduction 部分的开头）

We propose a modified neural sequence-to-sequence model with attention that uses multi-task learning on the decoder side to jointly learn two strongly related tasks: target-side language modeling and translation.(我们提出一种改进的ANMT，这个模型使用了 multi-task 的方式在 decoder 部分联合学习两个非常关联的任务：LM 和 translation)

Our approach aims to exploit the siganals from target-side monolingual data to learn a strong language model that supports the decoder in making translation decisions for the next word. (我们的方法探究了使用 target-side 的 monolingual data 去学习一个 strong 的 LM 来支持 decoder 更好的预测下一个单词)

Figure 1 illustrates this separation graphically. (Figure 1 用图解释)

We  view this approach as an instance of multi-task learning rather than transfer learning, where optimization is typically carried out sequentialy. (我们将这种方法看作 multi-task learning 而不是 transfer learning)

While initial results show only moderate improvements over the baseline and fall short against using synthetic parallel data, we believe there is value in pursuing this line of research further to simplify training procedures.(尽管初步的结果显示只有很少量的提高而且没有超过 synthetic parallel data 的结果，但是这依然有它的意义)





