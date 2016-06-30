Brainstorm
==========

> This repository contains the version of brainstorm that was developed and used for all the experiments within the NASCENCE project.


Brainstorm makes working with neural networks fast, flexible and fun.

Combining lessons from previous projects with new design elements, and written entirely in Python, Brainstorm has been designed to work on multiple platforms with multiple computing backends.


Getting Started
---------------
A good point to start is the brief [walkthrough](https://brainstorm.readthedocs.org/en/latest/walkthrough.html) of the ``cifar10_cnn.py`` example.  
More documentation is in progress, and hosted on [ReadTheDocs](https://brainstorm.readthedocs.org/en/latest/).
If you wish, you can also run the data preparation scripts (``data`` directory) and look at some basic examples (``examples`` directory).


Installation
------------
Here are some quick instructions for installing the latest master branch on Ubuntu.

```bash
# Install pre-requisites
sudo apt-get update
sudo apt-get install python-dev libhdf5-dev git python-pip
# Get brainstorm
git clone https://github.com/NASCENCE/brainstorm
# Install
cd brainstorm
[sudo] pip install -r requirements.txt
[sudo] python setup.py install
# Build local documentation (optional)
sudo apt-get install python-sphinx
make docs
# Install visualization dependencies (optional)
sudo apt-get install graphviz libgraphviz-dev pkg-config
[sudo] pip install pygraphviz --install-option="--include-path=/usr/include/graphviz" --install-option="--library-path=/usr/lib/graphviz/"
```
To use your CUDA installation with brainstorm:
```bash
$ [sudo] pip install -r pycuda_requirements.txt
```
Set location for storing datasets:
```bash
echo "export BRAINSTORM_DATA_DIR=/home/my_data_dir/" >> ~/.bashrc
```

License
-------

MIT License. Please see the LICENSE file.

Acknowledgements and Citation
-----------------------------

Klaus Greff and Rupesh Srivastava would like to thank Jürgen Schmidhuber for his continuous supervision and encouragement.
Funding from EU projects NASCENCE (FP7-ICT-317662) and WAY (FP7-ICT-288551) was instrumental during the development of this project.
We also thank Nvidia Corporation for their donation of GPUs.
