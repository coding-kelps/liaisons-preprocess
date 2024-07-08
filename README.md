⚠️ This repository is a part of an academical Master Project for the Heriot-Watt University, no third-party contributions are accepted.

# liaisons-preprocess

## Overview

This notebook outlines the preprocessing steps undertaken to generate datasets used for testing the [liaisons](https://github.com/coding-kelps/liaisons) client and [benchmarking open-source models in predicting argument relations](https://github.com/coding-kelps/liaisons-experiments).

### Dataset

For this preprocessing task, we utilized IBM's "Claim Stance Dataset" as the source. This dataset comprises 2,394 labeled claims across 55 controversial topics, collected from Wikipedia. Each claim is labeled based on its stance towards the topic, either "PRO" (supporting the topic) or "CON" (opposing the topic), making it an excellent resource for relation-based argument mining tasks.

As of now, the dataset is available on [HuggingFace](https://huggingface.co/datasets/ibm/claim_stance). Further details on the original dataset can be found in the paper *Stance Classification of Context-Dependent Claims* (Bar-Haim et al., 2017).

### Preprocessing Notes

The primary aim of this preprocessing is to create a representative sample of the dataset, thereby reducing computational costs for benchmarking and testing related software.

## About the Development Team
This project is solely conducted by me, [Guilhem Santé](https://github.com/guilhem-sante). I am a postgraduate student pursuing the MSc in Artificial Intelligence at Heriot-Watt University in Edinburgh.

## Special Thanks
I would like to credits [Andrew Ireland](http://www.macs.hw.ac.uk/~air/), my supervisor for this project.  
  
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/03/Heriot-Watt_University_logo.svg/1200px-Heriot-Watt_University_logo.svg.png" width="300">
