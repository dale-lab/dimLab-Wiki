
# Installing dimLab

After installing all of the previous softwares in [Quick Start](quickstart.md "Quick Start"), proceed to open a terminal and run the following commands:

>[!Warning|style:flat]
> Make sure to select the correct setup based on your computer configuration.

## In the Terminal
<!-- tabs:start -->

#### **<span style="color: Blue;"><b>CPU</b></span>**

```bash
conda create -n dimlab-env -c conda-forge python=3.9
conda activate dimlab-env
pip install cellpose
pip install "napari[all]"
```

#### **<span style="color: Green;"><b>GPU</b></span>**


```bash
conda create -n dimlab-env -c conda-forge python=3.9
conda activate dimlab-env
conda install pytorch=1.8.2 cudatoolkit=10.2 -c pytorch-lts
conda install cudnn
pip install "napari[all]"
```

<!-- tabs:end -->

## After installing the correct environment
Go to the folder **dimLab**:

> 🤖💭 Usually you will find this folder in <code>~/Documents/GitHub/dimLab/</code>

```bash
conda activate dimlab-env
pip install -e .
```