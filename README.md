# UMOT: A unified framework for long- and short-term association for multi-object tracking

https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0332709

## Installation

The codebase is built on top of [Deformable DETR](https://github.com/fundamentalvision/Deformable-DETR) and [MOTR](https://github.com/megvii-research/MOTR).

### Requirements

* Python 3.9–3.11, PyTorch 2.x, CUDA 12.x (recommended)

* Create environment and install PyTorch

    ```bash
    conda create -n UMOT python=3.10
    conda activate UMOT
    # PyTorch 2.2+ with CUDA 12 — see https://pytorch.org/get-started/locally/
    pip install torch torchvision
    ```

* Install other dependencies

    ```bash
    pip install -r requirements.txt
    ```

* Build MultiScaleDeformableAttention (CUDA 12 / PyTorch 2 compatible)

    ```bash
    cd models/ops
    pip install -e .
    ```

