# Active Semantic Decoy Polling (ASDP)

### A Machine Learning Framework for Detecting Progressive Semantic Data Exfiltration in Shadow AI Environments

![Research](https://img.shields.io/badge/Project-ASDP-blue)
![Python](https://img.shields.io/badge/Language-Python-blue)
![Jupyter](https://img.shields.io/badge/Notebooks-Jupyter-orange)

## 1. Overview

Active Semantic Decoy Polling (ASDP) is a research framework designed to investigate the detection of progressive semantic data exfiltration in Shadow AI environments. The project explores machine learning, conversational context and semantic indicators to identify potentially suspicious interactions that may be difficult to recognize when individual messages are examined in isolation.

This repository provides the implementation packages, experimental code and supporting notebooks associated with the ASDP research project. It is intended to support scientific transparency, experimental reproducibility and further cybersecurity research.

## 2. Research Objectives

- Investigate progressive semantic data exfiltration in Shadow AI environments.
- Examine the contribution of conversation history to detection.
- Assess the influence of conversation-history length through ablation experiments.
- Investigate the contribution of individual feature groups.
- Explore model evaluation and explainability through the supplied proxy experiment.
- Support supplementary testing involving HESD and LLaMA-related workflows.

## 3. Repository Contents

| File or filename prefix | Description |
| --- | --- |
| `ASDP_Experiment_01_Conversation_History_Co...` | Experiment 01: conversation-history investigation. |
| `ASDP_Experiment_02_History_Length_Ablation...` | Experiment 02: history-length ablation study. |
| `ASDP_Experiment_03_Feature_Group_Ablation...` | Experiment 03: feature-group ablation study. |
| `ASDP_Experiment_04_Completed_Proxy.zip` | Experiment 04: supplied proxy evaluation package. |
| `ASDP_Implementation_v1_2.zip` | ASDP implementation, version 1.2. |
| `ASDP_Implementation_v1_2_with_ablation.zip` | Version 1.2 implementation with ablation-related materials. |
| `HESD Testing.ipynb` | Supplementary HESD testing notebook. |
| `asdp-llama-g-3-hesd.ipynb` | Supplementary ASDP/LLaMA/HESD-related notebook. |

The first three filenames are shown as prefixes because their full names are not available in the repository screenshot. Use the corresponding complete filenames when downloading them.

## 4. Experimental Design

### Experiment 01 — Conversation History

Investigates the role of conversational context in detecting progressive semantic data exfiltration. Consult the experiment package for its exact comparison settings, dataset and evaluation procedure.

### Experiment 02 — History-Length Ablation

Examines the influence of different conversation-history lengths on detection performance. The original history-window settings and evaluation protocol should be retained when reproducing this experiment.

### Experiment 03 — Feature-Group Ablation

Investigates the contribution of feature groups to the detection framework. The feature definitions, configurations and comparison methodology are provided by the original experimental implementation where available.

### Experiment 04 — Proxy Evaluation

Provides the supplied proxy experiment associated with the ASDP evaluation and explainability workflow. Proxy-based findings should be interpreted within the limitations of the proxy setup and should not be represented as full real-world validation. Refer to the package and manuscript for the exact model, protocol and scope of the reported results.

## 5. Implementation Packages

The repository includes two ASDP version 1.2 archives: the base implementation and an implementation containing ablation-related materials. Extract these archives into separate directories to avoid overwriting files. Use the implementation and configuration corresponding to the experiment being reproduced.

## 6. Supplementary HESD Testing

The two Jupyter notebooks provide supplementary HESD-related testing and an ASDP/LLaMA-related workflow. These notebooks should be treated separately from the four numbered experiments unless the manuscript explicitly incorporates their results. Any external dataset, model weights, credentials or computing resources required by the notebooks must be obtained separately where they are not bundled.

## 7. Software Requirements and Installation

A Python environment with Jupyter Notebook or Google Colab is recommended. Exact Python versions and package dependencies should be determined from the original experiment files and notebook imports.

To create an isolated local environment:

```bash
python -m venv .venv
```

Activate it on Windows:

```powershell
.venv\Scripts\Activate.ps1
```

Or on Linux/macOS:

```bash
source .venv/bin/activate
```

Install Jupyter if needed:

```bash
python -m pip install jupyter
```

If an extracted experiment contains a `requirements.txt` file, install its dependencies from that experiment directory:

```bash
python -m pip install -r requirements.txt
```

Otherwise, inspect the experiment's documentation and imports before installing the required libraries. Separate environments may be needed for incompatible dependencies.

## 8. Running the Experiments

1. Download the required archive using GitHub, or download the repository through **Code > Download ZIP**.
2. Extract the repository archive, then extract each required experiment ZIP into its own directory.
3. Read any documentation included in the selected experiment package.
4. Install the experiment-specific dependencies.
5. Obtain the required dataset and configure local file paths as specified by the code.
6. Open the experiment notebook or execute its documented Python entry point.
7. Run preprocessing, training and evaluation in the order specified by the original implementation.
8. Save generated metrics, tables and figures and compare them with the corresponding manuscript results.

### Running in Google Colab

Open [Google Colab](https://colab.research.google.com/), upload the relevant `.ipynb` notebook, provide its required data and dependencies, and execute the cells in order. Select a GPU runtime only if the notebook requires one. Review the code before running it and never embed private credentials in a public notebook.

## 9. Dataset Availability

Use the datasets and preprocessing procedures specified by each experiment. Dataset availability, access conditions and redistribution permissions depend on the original data sources. If a required dataset is not included in the repository, obtain it from its authorized source before executing the corresponding experiment. Do not publish confidential conversations, personal information or restricted data.

## 10. Reproducibility and Evaluation

For meaningful comparisons, retain the original dataset version, preprocessing steps, feature definitions, training and testing splits, random seeds, model hyperparameters, history-window settings and evaluation metrics wherever specified. Record software versions and hardware details when repeating experiments. Avoid tuning on the held-out test set.

The associated manuscript and original experiment outputs should be consulted for numerical findings. This README does not introduce new performance claims or certify that all packages have been independently reproduced. Proxy and supplementary results should be distinguished from the main experimental results.

## 11. Citation

If you use this implementation or experimental material in academic work, please cite the associated ASDP research manuscript and acknowledge this repository. Use the verified author list, final manuscript title, publication year and DOI when available. Until formal publication details are available, cite the repository URL and the version or commit used in your research.

## 12. License and Research Use

Consult the repository's LICENSE file, if provided, for applicable code-use permissions. In the absence of an explicit license, do not assume permission to redistribute or modify the materials. Third-party datasets, models and dependencies remain subject to their respective licenses.

The framework is intended for authorized cybersecurity research, defensive evaluation and academic experimentation. It should not be used to access, disclose or exfiltrate information without authorization.

## 13. Issues and Feedback

Questions regarding implementation, experimental reproduction or technical issues may be submitted through the repository's GitHub Issues section, if enabled. Include the relevant experiment number, environment details and error message, without disclosing confidential information.

---

**ASDP Research Project | Semantic Data Exfiltration Detection | Shadow AI Security | Machine Learning**
