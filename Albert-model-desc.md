# Description

[ALBERT](https://arxiv.org/abs/1909.11942) (single model)



### implementation

Each case in Commonsense QA contain a question stem, a question concept and 5 choices.

1.  **Input features**

    We made **input text** for each choice using the following format  `[CLS] question [SEP] question_concept [SEP] choice_i [SEP]`.

    The **token_type_ids** of choice tokens are set to 1, other tokens are set to 0.

2.  **Model**

    Our model are similar to [huggingface's AlbertForMultipleChoice](https://huggingface.co/transformers/_modules/transformers/models/albert/modeling_albert.html#AlbertForMultipleChoice.forward) to the task.

    input_feature =**albert**=> pooled_output =**classifier**=> score

    [CODE](https://github.com/Zaaachary/CSQA)

### Experiment Details

The accuracies of 5 different runs are 80.18%, 80.10%, 80.50%, 79.93%, 80.09% respectively on the dev set.

Parameters for training are listed as below:

-   max sequence length: 128
-   train batch size: 2
-   gradient accumulation step: 8
-   warmup step: 0.1
-   weight decay: 0.1
-   learning rate: 2e-5
-   train epoch: 10



### Affiliation

[Soochow University](https://www.suda.edu.cn/) & [I2R](https://www.a-star.edu.sg/i2r)
