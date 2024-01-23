[How to run Merlin on Google Colab](https://medium.com/nvidia-merlin/how-to-run-merlin-on-google-colab-83b5805c63e0)

```
# This get the RAPIDS-Colab install files and test check your GPU.  Run this and the next cell only.
# Please read the output of this cell.  If your Colab Instance is not RAPIDS compatible, it will warn you and give you remediation steps.
!git clone https://github.com/rapidsai/rapidsai-csp-utils.git
%cd rapidsai-csp-utils
!git checkout patch-22.12
%cd ..
!python rapidsai-csp-utils/colab/env-check.py
!python rapidsai-csp-utils/colab/pip-install.py

# Install the Merlin Framework
!pip install -U git+https://github.com/NVIDIA-Merlin/models.git@release-23.04
!pip install -U git+https://github.com/NVIDIA-Merlin/nvtabular.git@release-23.04
!pip install -U git+https://github.com/NVIDIA-Merlin/core.git@release-23.04
!pip install -U git+https://github.com/NVIDIA-Merlin/system.git@release-23.04
!pip install -U git+https://github.com/NVIDIA-Merlin/dataloader.git@release-23.04
!pip install -U git+https://github.com/NVIDIA-Merlin/Transformers4Rec.git@release-23.04
!pip install -U xgboost lightfm implicit
```
```
!pip install nvtabular=="1.5.0"
!pip install merlin=="1.9.1"
!pip install merlin-models=="0.10.0"
!pip install merlin-systems
!pip install tritonclient
!pip install pyarrow=="10.0.1"
!pip install torch
!pip install tensorflow=="2.11.0"
!pip install protobuf
```

