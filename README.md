viswsl
======

Weakly supervised learning to solve multiple vision tasks together.


Install Dependencies
--------------------

For these steps to install through Anaconda / Miniconda.

1. Install Anaconda or Miniconda distribution based on Python3+ from their [downloads site](https://conda.io/docs/user-guide/install/download.html).


2. Clone the repository first.

```
git clone https://www.github.com/kdexd/viswsl
```

3. Create a conda environment and install all the dependencies.

```
cd viswsl
conda create -n viswsl python=3.7
conda activate viswsl
pip install -r requirements.txt
```

<!-- Mention apt dependency: ZeroMQ (libzmq3-dev) -->

4. **[Optional]** Install NVIDIA Apex for Half-precision training. (Requires GCC 5+)

```
pip install -v --no-cache-dir --global-option="--cpp_ext" \
    --global-option="--cuda_ext" git+https://github.com/nvidia/apex.git
```


5. Install this codebase as a package in development version.

```
python setup.py develop
```