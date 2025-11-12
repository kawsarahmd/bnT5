### Acknowledgements
We thank the Google TPU Research Cloud (TRC) program for generously providing the cloud computing infrastructure essential to this work.


### TPU Setup for Pretraining

This repository includes shell scripts to quickly set up the environment for **T5 pretraining** on **Google Cloud TPU**.

### Files

* **`conda_setup.sh`** — Installs Miniconda, creates the Python environment, and installs required dependencies.
* **`vllm_setup_in_tpu.sh`** — Prepares TPU runtime with optimized libraries for vLLM / transformer-based pretraining.

### Usage

Run the following commands inside your TPU VM:

```bash
# Step 1: Set up Conda environment
bash ./shell_scripts/conda_setup.sh

# Step 2: Configure TPU environment
bash ./shell_scripts/vllm_setup_in_tpu.sh
```

### Note

These scripts are tested in **Google Cloud TPU v4-8** and **Ubuntu 22.04 TPU VM** images.
Modify paths or versions as needed for your setup.


