# Quantum-Enhanced-Default-Detection

Utilizes FT Transformer architecture to detect high risk default potential. Quantum models use QuFeX parametrized circuits detailed in:
https://arxiv.org/pdf/2501.13165

Classical Implementation: Uses GPU accelerated PyTorch interface to establish baseline performance for quantum comparison

Quantum CLS Implementation: Adds one QuFeX layer after the self-attention layers on only the CLS token.

Quantum MLP Implementation: Adds QuFeX layer on every token in MLP layers in between attention layers.

## Installation

Clone the repository and install the required dependencies:

```bash
git clone https://github.com/benjaminhagan/Quantum-Enhanced-Default-Detection
cd Quantum-Enhanced-Default-Detection
pip install -r requirements.txt
pip install -e .
