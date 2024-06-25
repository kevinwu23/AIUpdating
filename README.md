# Regulating AI Adaptation: An Analysis of AI Medical Device Updates

## Overview

This repository contains the data and code used for the analysis presented in the paper "Regulating AI Adaptation: An Analysis of AI Medical Device Updates". The paper was presented at the Conference on Health, Inference, and Learning (CHIL) 2024.

### Authors
- Kevin Wu, Stanford University, USA (kevinywu@stanford.edu)
- Eric Wu, Stanford University, USA (wue@stanford.edu)
- Kit Rodolfa, Stanford Law School, USA (krodolfa@law.stanford.edu)
- Daniel E. Ho, Stanford Law School, USA (dho@law.stanford.edu)
- James Zou, Stanford University, USA (jamesz@stanford.edu)

## Abstract
While the pace of development of AI has rapidly progressed in recent years, the implementation of safe and effective regulatory frameworks has lagged behind. In particular, the adaptive nature of AI models presents unique challenges to regulators as updating a model can improve its performance but also introduce safety risks. This study systematically analyzes the frequency and nature of updates in FDA-approved AI medical devices, providing insights for future regulatory policies toward model updating and adaptive AI.

## Contents
- `analysis.ipynb`: The main figures can be run through this notebook.
- `fda_ai_devices_2023.csv`: Our table of medical devices that have been classified by the FDA as AI.
| **Column**             | **Description**                                                                                             |
|------------------------|-------------------------------------------------------------------------------------------------------------|
| Date of Final Decision | The date when the final decision was made regarding the approval of the AI medical device.                  |
| Submission Number      | The unique identification number assigned to each submission for FDA approval.                              |
| Device                 | The name of the AI medical device submitted for approval.                                                   |
| Company                | The name of the company that developed and submitted the AI medical device for approval.                    |
| Panel (Lead)           | The FDA panel responsible for reviewing and approving the medical device.                                   |
| Primary Product Code   | The primary product code assigned to the device, indicating its category and intended use. 
- `update_annotations_2023.csv`:

| **Column**              | **Description**                                                                                         |
|-------------------------|---------------------------------------------------------------------------------------------------------|
| Subject                 | The submission number of the subject AI medical device being analyzed.                                  |
| Predicate               | The submission number of the predicate AI medical device to which the subject device is compared.       |
| Input signal            | Indicates if there has been an update to the input signal for the AI medical device.                    |
| Model architecture      | Indicates if there has been an update to the model architecture for the AI medical device.              |
| Training data           | Indicates if there has been an update to the training data used for the AI medical device.              |
| Target population       | Indicates if there has been an update to the target population for the AI medical device.               |
| Unspecified Improvement | Indicates if there has been an unspecified improvement to the AI medical device.                        |
| Outcome variable        | Indicates if there has been an update to the outcome variable for the AI medical device.                |


## Data and Code Availability
The primary data used in this study are publicly available through the FDA website. The analysis of the data and the code used are available in this repository.

## Citation
If you use this code or data in your work, please cite the paper:

```bibtex
@inproceedings{wu2024regulating,
  title={Regulating AI Adaptation: An Analysis of AI Medical Device Updates},
  author={Wu, Kevin and Wu, Eric and Zou, James},
  booktitle={Conference on Health, Inference, and Learning (CHIL)},
  year={2024},
  organization={Proceedings of Machine Learning Research}
}
