# Installations_and_environment_setups
This repository contains information about how to install and setup various environments in linux/ubuntu
## Contents
1. Julia on linux (using anaconda virtual_env)
2. Tensorflow-gpu setup on anaconda
## Julia on linux (using anaconda virtual env)
- First create a new environment
    ```
    conda create -n <name_of_env> -c conda-forge julia
    ```
- Creating a new env is optional, if you want to install julia into an existing env then execute the following commands
    ```
    conda activate <env_name>
    conda install -c conda-forge julia
    ```
- Test julia installation by running ```julia``` in the terminal to open julia REPL. Then type 
    ```
    println("Hello world")
    ```
    You should be able to see the output "Hello world" indicating that the installation is successful
- Next, install jupyter notebook if it is not already installed
    ```
    conda install jupyter
    ```
- Now, connect julia to jupyter notebook by running the following commands in julia REPL (to open julia REPL, just run 'julia' in the terminal)
    ```
    using Pkg
    Pkg.add("IJulia")
    ```
    Now this should start the installation
- Once the installation is complete, you will be able to see julia option in the jupyter notebooks

Some usefull links:
- https://www.youtube.com/watch?v=oyx8M1yoboY
- https://anaconda.org/conda-forge/julia
- https://docs.julialang.org/en/v1/stdlib/REPL/
## Tensorflow-gpu setup in anaconda environment
- Refer https://www.thehardwareguy.co.uk/install-tensorflow-gpu 



