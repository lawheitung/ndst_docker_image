# Text Classification

These files use the NVIDIA GPU Cloud (NGC) NeMo container to walk the learner through an introductory text classification ML workflow. Everything is deployed by Kubeflow running on K8S and uses Trident/NetApp for a persistent storage back-end.

## Use Case 1
Showcase how a user can use Kubeflow to deploy a Jupyter notebook and gain access to a GPU accelerated development environment.

This will include an introduction to the JupyterLab IDE, an overview of K8S storage integration with Trident, setup steps to monitor GPU utilization through the jupyter-nvdashboard, and a walkthrough of the Kubeflow Notebook interface.

## Use Case 2
Showcase how a user can use NeMo to quickly download and train a BERT NLP model and then checkpoint and compare results.

Checkpointing and reverting is done using NetApp and the pre-trained models and libraries come from the NeMo packages on NGC.

## Use Case 3

Development TBD

## Data

The `SST-2` data is included in this repo for reproducability, but it should not be re-distributed outside of the lab environment for licensing reasons.

# Setup, Installation, and Upgrading

See the [tools](tools/README.md) section of this repo.
