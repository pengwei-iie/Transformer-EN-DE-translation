## A Pytorch Implementation of the Transformer Network
This repository includes pytorch implementations of ["Attention is All You Need"](https://papers.nips.cc/paper/7181-attention-is-all-you-need.pdf) (Vaswani et al., NIPS 2017) and 
["Weighted Transformer Network for Machine Translation"](https://arxiv.org/pdf/1711.02132.pdf) (Ahmed et al., arXiv 2017)

## Run
1. python preprocess.py -train_src ./data/newstest2013.en -train_tgt ./data/newstest2013.de
获得训练的文件copus-train.t7 和 copus.dict
2. python train.py -data_path data/copus-train.t7 -model_path model_name
进行训练
3. predict python translate.py -vocab data/copus.dict -model_path model_name -decode_input ./data/source_file -decode_output ./data/out_file

## Reference
**Paper**
- Vaswani et al., "Attention is All You Need", NIPS 2017
- Ahmed et al., "Weighted Transformer Network for Machine Translation", Arxiv 2017

