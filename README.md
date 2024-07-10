# whisper-large-v2-atcosim_corpus

This model is a fine-tuned version of [openai/whisper-large-v2](https://huggingface.co/openai/whisper-large-v2) on the [atcosim_corpus](https://huggingface.co/datasets/Jzuluaga/atcosim_corpus) dataset.


## Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 1e-05
- train_batch_size: 32
- eval_batch_size: 8
- seed: 42
- distributed_type: multi-GPU
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: linear
- lr_scheduler_warmup_steps: 250
- num_epochs: 50

  
## Evaluation results

See README.md under the `Evaluation` folder.


## Framework versions

- Transformers 4.42.3
- Pytorch 2.3.1+cu118
- Datasets 2.20.0
- Tokenizers 0.19.1
