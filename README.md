# BO-with-DiffCSP

Attempting to perform optimization of materials via ab initio generation with DiffCSP checkpoints. WIP.

Dependencies are listed in requirements.txt. I used Python version 3.9.18. Recommended to have CUDA.

You will need to manually edit matminer's fingerprint.py to include this line "from ruamel.yaml import YAML", and replace all function calls of yaml.safe_load(f) with YAML(typ='safe', pure=True).load(f) to overcome a depcreciated function.
