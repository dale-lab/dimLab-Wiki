
# Installing dimLab

> [!ATTENTION|style:flat]
> A <code>GPU</code> is highly recommended to run this project. It will reduce processing times from <code>~15-20 min</code> to <code>~3-5 min</code> per run.

After installing all of the previous softwares in [Quick Start](quickstart.md "Quick Start"), you are ready to install <code>dimLab</code>

>[!Warning|style:flat]
> Make sure to select the correct setup based on your computer configuration.

## Create a virtual environment

🤖💭 Open a terminal and run the following commands:

<!-- tabs:start -->

#### **<span style="color: Blue;"><b>CPU</b></span>**

```bash
conda create -n dimlab-env -c conda-forge python=3.9 # creates a virtual environment
conda activate dimlab-env # activates the virtual environment
pip install cellpose # installs cellpose
pip install "napari[all]" # installs napari
```

#### **<span style="color: Green;"><b>GPU</b></span>**


```bash
conda create -n dimlab-env -c conda-forge python=3.9 # creates a virtual environment
conda activate dimlab-env # activates the virtual environment
conda install pytorch=1.8.2 cudatoolkit=10.2 -c pytorch-lts # installs pytorch and cudatoolkit
conda install cudnn # installs cudnn
pip install "napari[all]" # installs napari
```

<!-- tabs:end -->

## Download dimLab

Download the latest version of the dimLab:

<!-- tabs:start -->
#### **<span style="color: Black;"><b>First Option</b></span>**

Open GitHub Desktop and go to:

> <code>File</code> ➡️ <code>Clone Repository</code> ➡️ <code>Enter a name for the repository</code>

You will see that the name of the repo is link to the organization dale-lab. i.e. <code>dale-lab/dimLab</code>

This will download the latest version of the dimLab and store it in <code>~/Documents/GitHub/dimLab/</code>

> [!Note|style:flat]
> 🤖💭 Now every time you need to update the repo you just need to go to GitHub Desktop, and press <code>Fetch Origin</code> to update the repo.

#### **<span style="color: Black;"><b>Second Option</b></span>**

> [!Warning|style:flat]
> 🤖💭 In this option you are required to download the latest version of <code>dimLab</code> each time there is an update

Go to the [GitHub repository website](https://github.com/dale-lab/dimLab) and download the latest version of the dimLab.

> <code>Code</code> ➡️ <code>Download Zip</code>

It is recommended to store all your git repos in:

> <code>C:\Users\...\Documents\GitHub</code>

<!-- tabs:end -->

## Install dimLab

Go to the folder **dimLab**:

> 🤖💭 Usually you will find this folder in <code>~/Documents/GitHub/dimLab/</code>

open a terminal and type: 

```bash
conda activate dimlab-env # activate the virtual environment
pip install -e . # installs dimLab
```

> [!Note|style:flat]
> 🤖💭 If you get any errors during the installation, please let us know.
> 🤖💭 now you are ready to run your first dimLab pipeline.