# Python sample code for fine-tuned BERT model

## Introduction
This sample code show how to run fine-tuned BERT model using OpenVINO toolkit on a simple specific task to predict whether an IMDB movie review is positive or negative.

For how to fine-tune BERT model and use OpenVINO to convert BERT model, please go to directory "bert_training_fine-tine" and follow the guide.

## Run inference using OpenVINO
After get converted fine-tuned BERT model, run below command to infer, please change the libcpu_extension.so path if needed on your machine.

  python3 bert_fine-tune_for_movie-review.py -m path_to_bert-model/bert-finetune.xml -l /opt/intel/openvino/inference_engine/lib/intel64/libcpu_extension_avx512.so -d CPU
