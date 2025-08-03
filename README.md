# DS266-ugarcia-bjulve

## Files

- Models_SocraticPretrained_Augmented.ipynb
  - Use QLoRA to fine tune the Socratric Pretrained (Pagnoni) BARTLarge model on the augmented data set with 25% Socratic question/summary masked inputs added.
  - 750 non-augmented samples, 250 augmented samples.
  - 1000 total training samples.
- Models_SocraticPretrained_Augmented_Evaluation.ipynb
  - Run the test SQuALITY samples on the Socratic Pretrained model FT on augmented data. Metrics are also computed.
  - 1040 total test samples.
- Models_SocraticPretrained_Baseline.ipynb
  - Use QLoRA to fine tune the Socratric Pretrained model on the original SQuALITY training data set.
  - No augmented samples.
  - 1000 total training samples.
- Models_SocraticPretrained_Baseline_Evaluation.ipynb
  - Run the test SQuALITY samples on the Socratic Pretrained model FT on non-augmented data. Metrics are also computed.
  - 1040 total test samples.
- Models_SocraticPretrained_No_FT_Evaluation.ipynb
  - Run the test SQuALITY samples on the Socratic Pretrained model with no FT. Metrics are also computed.
  - 1040 total test samples.
- Models_T5Gemma_Augmented.ipynb
  - Use QLoRA to fine tune the T5Gemma model on the augmented data set with 25% Socratic question/summary masked inputs added.
  - 750 non-augmented samples, 250 augmented samples.
  - 1000 total training samples.
  - The [T5Gemma](https://developers.googleblog.com/en/t5gemma/) model is based on the Gemma 2B LLM adapted to fit an encoder-decoder T5-like architecture. We used the T5Gemma 2B instruction tuned variant. The model card on HuggingFace can be found [here](https://huggingface.co/google/t5gemma-2b-2b-ul2-it). 
- Models_T5Gemma_Augmented_Evaluation.ipynb
  - Run the test SQuALITY samples on the T5Gemma model FT on the augmented data set. Metrics are also computed.
  - 1040 total test samples.
- Models_T5Gemma_Baseline_4_layers.ipynb
  - Use QLoRA to fine tune the T5Gemma model on the original SQuALITY training data set.
  - No augmented samples.
  - 1000 total training samples.
- Models_T5Gemma_Baseline_Evaluation.ipynb
  - Run the test SQuALITY samples on the T5Gemma model FT on non-augmented data. Metrics are also computed.
  - 1040 total test samples.
- Models_T5Gemma_No_FT_Evaluation.ipynb
  - Run the test SQuALITY samples on the T5Gemma model with no FT. Metrics are also computed.
  - 1040 total test samples.
- QFS_Datasets.ipynb
  - EDA notebook for QMSum and SQuALITY data sets.
- Socratic_Pretrained_Sampler.ipynb
  - Generate output text from the Socratic Pretrained model with no FT.
- T5Gemma_Sampler.ipynb
  - Generate output text from the T5Gemma model with no FT.

## External Storage

Here is a link to Bernard Julve's Google Drive folder with saved HuggingFace models:

https://drive.google.com/drive/folders/1OuFnXXQjodm4zuDqNgUFvnEFfSDediR7?usp=sharing

These 4 trained models were the result of the Models_*.ipynb fine tuning notebooks that utilized the SQuALITY data set.
