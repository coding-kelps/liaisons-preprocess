⚠️ This repository is a part of an academical project for the Heriot-Watt University, no third-party contributions are accepted.

# liaisons-preprocess

## Overview

This notebook outlines the preprocessing steps undertaken to generate datasets used for testing the [liaisons](https://github.com/coding-kelps/liaisons) client and [benchmarking open-source models in predicting argument relations](https://github.com/coding-kelps/liaisons-experiments).

### Dataset

For this preprocessing task, we utilized IBM's "Claim Stance Dataset" as the source. This dataset comprises 2,394 labeled claims across 55 controversial topics, collected from Wikipedia. Each claim is labeled based on its stance towards the topic, either "PRO" (supporting the topic) or "CON" (opposing the topic), making it an excellent resource for relation-based argument mining tasks.

As of now, the dataset is available on [HuggingFace](https://huggingface.co/datasets/ibm/claim_stance). Further details on the original dataset can be found in the paper *Stance Classification of Context-Dependent Claims* (Bar-Haim et al., 2017).

### Preprocessing Notes

The primary aim of this preprocessing is to create representative samples of the dataset, roughly 100 entries, enabling benchmarking with limited computing resources. Secondly, previous models in the field of relation-based argument mining have proven to give misleading benchmarks by achieving satisfactory results in specific domains (Gorur et al., 2024). To circumvent this, the preprocessing will also modify the distribution of claims to achieve a balanced plurality of stances and topics.

### Results

Processing results can be found on HuggingFace at [coding-kelps/liaisons-claim-stance-sample](https://huggingface.co/datasets/coding-kelps/liaisons-claim-stance-sample).

## About Contributions

As mentioned earlier, this work is part of an academic project for the validation of my Master's Degree at Heriot-Watt University, preventing me from accepting any contributions until the final release of my project. Thank you for your understanding.

## Associated Works

This work is part of a collection of works whose ultimate goal is to deliver a framework to automatically analyze social media content (e.g., X, Reddit) to extract their argumentative value and predict their relations, leveraging Large Language Models' (LLMs) abilities:

- [liaisons](https://github.com/coding-kelps/liaisons) (the developed client for social media content analysis)
- [liaisons-claim-stance-sample](https://huggingface.co/datasets/coding-kelps/liaisons-claim-stance-sample) (the resulting sample of this preprocess)
- [liaisons-experiments](https://github.com/coding-kelps/liaisons-experiments) (the benchmarking framework to evaluate LLMs' relation prediction abilities)
- [liaisons-experiments-results](https://huggingface.co/datasets/coding-kelps/liaisons-experiments-results) (the obtained results with this benchmarking)
- [mantis-shrimp](https://github.com/coding-kelps/mantis-shrimp) (the configuration-as-code used to set up my workstation for this project)

## About the Development Team
This project is solely conducted by me, [Guilhem Santé](https://github.com/guilhem-sante). I am a postgraduate student pursuing the MSc in Artificial Intelligence at Heriot-Watt University in Edinburgh.

## Special Thanks
I would like to credits [Andrew Ireland](http://www.macs.hw.ac.uk/~air/), my supervisor for this project.  
  
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/03/Heriot-Watt_University_logo.svg/1200px-Heriot-Watt_University_logo.svg.png" width="300">
