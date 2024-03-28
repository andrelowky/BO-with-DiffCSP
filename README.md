# BO-with-DiffCSP

Attempting to perform optimization of materials via ab initio generation with DiffCSP checkpoints. WIP.

Make sure your environment is running Python==3.9.18 (may need to change kernels). Afterwards, install these packages first: PyTorch (with CUDA if available), then pymatgen. Then install the dependencies I listed.

You will need to manually edit matminer's fingerprint.py to include this line "from ruamel.yaml import YAML", and replace all function calls of yaml.safe_load(f) with YAML(typ='safe', pure=True).load(f) to overcome a depcreciated function.
