# WorkFlow: save effort for logging and visualization

## How does it work

WorkFlow extracts basic process of training a neural network, and handles the logging and the visualization of multiple loss variables. 
It allows you to focus on the parts that most deserve your valuable efforts, such as network structure and optimization strategy.

<!-- ## Run the sample -->

# Install dependancies
## Install all required files
### 1. Enter your own conda environment
### 2. Install dependancies
```
pip install numpy pyyaml mkl mkl-include setuptools cmake cffi typing torchvision visdom matplotlib
```

<!-- ```
$ pip install -r requirements.txt
``` -->

install Workflow

```
$ python setup.py install
```

## Install all required files (old version)

Install Pytorch 
1. Install virtualenv: https://virtualenv.pypa.io/en/stable

2. Build a new virtualenv environment (this will create a folder in your current directory).

```
$ virtualenv pytorch
```

3. Go to the new folder and activate the environment(https://virtualenv.pypa.io/en/stable/userguide/#usage)

```
$ source bin/activate
```

4. Clone pytorch and build: https://github.com/pytorch/pytorch

```
$ git clone --recursive https://github.com/pytorch/pytorch
$ cd pytorch
$ python setup.py install
```

5. Install dependencies
```
$ pip install numpy pyyaml mkl mkl-include setuptools cmake cffi typing
```

Install torchvision and visdom

```
$ pip install torchvision
$ pip install visdom
```

# Run the sample code

Run the visdom server
```
$ python -m visdom.server 
```
Open another terminal
```
$ python sample.py
```