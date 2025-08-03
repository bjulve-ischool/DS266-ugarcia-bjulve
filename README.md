# DS266-ugarcia-bjulve

## Files

- **analysis/**
  - **data/**
    - [hallucination_study_test_samples-2025-08-02_171427.pkl](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/analysis/data/hallucination_study_test_samples-2025-08-02_171427.pkl)
      - Saved short story/question pairs from the SQuALITY test set. There are 5 in total.
  - [Prepare_Samples.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/analysis/Prepare_Samples.ipynb)
    - Randomly sample 5 short stories from the SQuALITY test set and pair them with 5 questions generated from the [MixQG](https://huggingface.co/Salesforce/mixqg-base) model.
  - [SocraticPretrained_Augmented_FT_Analysis.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/analysis/SocraticPretrained_Augmented_FT_Analysis.ipynb)
    - Generate output text for the Socratic Pretrained model FT on augmented data.
    - Use the 5 prepared short story/question pairs.
  - [SocraticPretrained_Augmented_FT_Analysis_Markup.pdf](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/analysis/SocraticPretrained_Augmented_FT_Analysis_Markup.pdf)
    - Highlight hallucination sentences in the output from the accompanying analysis notebook.
  - [SocraticPretrained_No_FT_Analysis.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/analysis/SocraticPretrained_No_FT_Analysis.ipynb)
    - Generate output text for the Socratic Pretrained model with no FT.
    - Use the 5 prepared short story/question pairs
  - [SocraticPretrained_No_FT_Analysis_Markup.pdf](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/analysis/SocraticPretrained_No_FT_Analysis_Markup.pdf)
    - Highlight hallucination sentences in the output from the accompanying analysis notebook.
  - [SocraticPretrained_Regular_FT_Analysis.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/analysis/SocraticPretrained_Regular_FT_Analysis.ipynb)
    - Generate output text for the Socratic Pretrained model FT on the original SQuALITY training set.
    - Use the 5 prepared short story/question pairs
  - [SocraticPretrained_Regular_FT_Analysis_Markup.pdf](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/analysis/SocraticPretrained_Regular_FT_Analysis_Markup.pdf)
    - Highlight hallucination sentences in the output from the accompanying analysis notebook.
  - [T5Gemma_Augmented_FT_Analysis.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/analysis/T5Gemma_Augmented_FT_Analysis.ipynb)
    - Generate output text for the T5Gemma model FT on augmented data.
    - Use the 5 prepared short story/question pairs
  - [T5Gemma_Augmented_FT_Analysis_Markup.pdf](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/analysis/T5Gemma_Augmented_FT_Analysis_Markup.pdf)
    - Highlight hallucination sentences in the output from the accompanying analysis notebook.
  - [T5Gemma_No_FT_Analysis.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/analysis/T5Gemma_No_FT_Analysis.ipynb)
    - Generate output text for the T5Gemma model with no FT.
    - Use the 5 prepared short story/question pairs
  - [T5Gemma_No_FT_Analysis_Markup.pdf](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/analysis/T5Gemma_No_FT_Analysis_Markup.pdf)
    - Highlight hallucination sentences in the output from the accompanying analysis notebook.
  - [T5Gemma_Regular_FT_Analysis.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/analysis/T5Gemma_Regular_FT_Analysis.ipynb)
    - Generate output text for the T5Gemma model FT on the original SQuALITY training set.
    - Use the 5 prepared short story/question pairs
  - [T5Gemma_Regular_FT_Analysis_Markup.pdf](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/analysis/T5Gemma_Regular_FT_Analysis_Markup.pdf)
    - Highlight hallucination sentences in the output from the accompanying analysis notebook.
- [Models_SocraticPretrained_Augmented.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/Models_SocraticPretrained_Augmented.ipynb)
  - Use QLoRA to fine tune the Socratric Pretrained (Pagnoni) BARTLarge model on the augmented data set with 25% Socratic question/summary masked inputs added.
  - 750 non-augmented samples, 250 augmented samples.
  - 1000 total training samples.
- **data/**
  - **v1-3/**
    - [dev.jsonl](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/data/v1-3/dev.jsonl)
      - SQuALITY validation set.
      - 500 total samples after forming every possible response, question, and document triplet.
    - [test.jsonl](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/data/v1-3/test.jsonl)
      - SQuALITY test set.
      - 1040 total samples after forming every possible response, question, and document triplet.
    - [train.jsonl](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/data/v1-3/train.jsonl)
      - SQuALITY training set.
      - 1000 total samples after forming every possible response, question, and document triplet.
- **datasets/**
  - [models_socraticpretraining_augmented_train-2025-07-28_092936.json](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/datasets/models_socraticpretraining_augmented_train-2025-07-28_092936.json)
    - Saved the 250 augmented samples (Socratic question/summary masked inputs).
    - This took 20 minutes to generate on Colab.
- **initial_attempts/**
  - Various notebooks we created early on in the project.
  - These are for historical purposes only.
- **outputs/**
  - These are the predictions (summary text) generated from each of the 6 models when run against the SQuALITY test data set.
- [Models_SocraticPretrained_Augmented_Evaluation.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/Models_SocraticPretrained_Augmented_Evaluation.ipynb)
  - Run the test SQuALITY samples on the Socratic Pretrained model FT on augmented data. Metrics are also computed.
  - 1040 total test samples.
- [Models_SocraticPretrained_Baseline.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/Models_SocraticPretrained_Baseline.ipynb)
  - Use QLoRA to fine tune the Socratric Pretrained model on the original SQuALITY training data set.
  - No augmented samples.
  - 1000 total training samples.
- [Models_SocraticPretrained_Baseline_Evaluation.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/Models_SocraticPretrained_Baseline_Evaluation.ipynb)
  - Run the test SQuALITY samples on the Socratic Pretrained model FT on non-augmented data. Metrics are also computed.
  - 1040 total test samples.
- [Models_SocraticPretrained_No_FT_Evaluation.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/Models_SocraticPretrained_No_FT_Evaluation.ipynb)
  - Run the test SQuALITY samples on the Socratic Pretrained model with no FT. Metrics are also computed.
  - 1040 total test samples.
- [Models_T5Gemma_Augmented.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/Models_T5Gemma_Augmented.ipynb)
  - Use QLoRA to fine tune the T5Gemma model on the augmented data set with 25% Socratic question/summary masked inputs added.
  - 750 non-augmented samples, 250 augmented samples.
  - 1000 total training samples.
  - The [T5Gemma](https://developers.googleblog.com/en/t5gemma/) model is based on the Gemma 2B LLM adapted to fit an encoder-decoder T5-like architecture. We used the T5Gemma 2B instruction tuned variant. The model card on HuggingFace can be found [here](https://huggingface.co/google/t5gemma-2b-2b-ul2-it). 
- [Models_T5Gemma_Augmented_Evaluation.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/Models_T5Gemma_Augmented_Evaluation.ipynb)
  - Run the test SQuALITY samples on the T5Gemma model FT on the augmented data set. Metrics are also computed.
  - 1040 total test samples.
- [Models_T5Gemma_Baseline_4_layers.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/Models_T5Gemma_Baseline_4_layers.ipynb)
  - Use QLoRA to fine tune the T5Gemma model on the original SQuALITY training data set.
  - No augmented samples.
  - 1000 total training samples.
- [Models_T5Gemma_Baseline_Evaluation.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/Models_T5Gemma_Baseline_Evaluation.ipynb)
  - Run the test SQuALITY samples on the T5Gemma model FT on non-augmented data. Metrics are also computed.
  - 1040 total test samples.
- [Models_T5Gemma_No_FT_Evaluation.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/Models_T5Gemma_No_FT_Evaluation.ipynb)
  - Run the test SQuALITY samples on the T5Gemma model with no FT. Metrics are also computed.
  - 1040 total test samples.
- [QFS_Datasets.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/QFS_Datasets.ipynb)
  - EDA notebook for QMSum and SQuALITY data sets.
- [Socratic_Pretrained_Sampler.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/Socratic_Pretrained_Sampler.ipynb)
  - Generate output text from the Socratic Pretrained model with no FT.
- [T5Gemma_Sampler.ipynb](https://github.com/bjulve-ischool/DS266-ugarcia-bjulve/blob/main/T5Gemma_Sampler.ipynb)
  - Generate output text from the T5Gemma model with no FT.

## External Storage

Here is a link to Bernard Julve's Google Drive folder with saved HuggingFace models:

https://drive.google.com/drive/folders/1OuFnXXQjodm4zuDqNgUFvnEFfSDediR7?usp=sharing

These 4 trained models were the result of the Models_*.ipynb fine tuning notebooks that utilized the SQuALITY data set.
