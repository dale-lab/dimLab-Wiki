
**environement name**: dimlab-env

## First Steps
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
conda create -n <project-name> -c conda-forge python=3.9
conda activate <project-name>
conda install -c conda-forge pyopencl
conda install pytorch=1.8.2 cudatoolkit=10.2 -c pytorch-lts
conda install cudnn
pip install "napari[all]"
```

<!-- tabs:end -->

## After installing the correct environment
Move to the folder **dimLab**:

```bash
conda activate dimlab-env
pip install -e .
```