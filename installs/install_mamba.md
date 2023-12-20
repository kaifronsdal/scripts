```
wget -O $HOME/miniforge3.sh "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-$(uname)-$(uname -m).sh"
bash $HOME/miniforge3.sh -b -p "$HOME/conda"
rm $HOME/miniforge3.sh

source $HOME/conda/bin/activate

source "${HOME}/conda/etc/profile.d/conda.sh"
# For mamba support also run the following command
source "${HOME}/conda/etc/profile.d/mamba.sh"

conda activate

conda init
mamba init
```