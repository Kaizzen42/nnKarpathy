# nnKarpathy


# Environment Setup

## Conda 
1. Use conda to create and environment with a specific python version.
`conda create --name "torch_nn_base" python=3.9`
Make sure you specify the python version.
This would install python in the correct directory within your environment, thus giving you a specific python path and installation for your new environment.
It will prevent mixups with other python installations. Note that these other versions could be newer, but not the ones you want. 

2. Activate env
`conda activate torch_nn_base`

3. Check which python path
`which python3`
This should return a path within your env. If it returns a path like your system default, or another env, the python is not the one you want to use. To fix this, first check if python was installed correctly in the location you wanted, and then deactivate and reactivate your env.

Correct value for `which python3`
`/opt/homebrew/Caskroom/miniforge/base/envs/torch_nn_base/bin/python3`

Incorrect value:
`/opt/homebrew/bin/python3`

4. [optional] If you see the bug in step3, fix as follows:
`conda deactivate`
Repeat if your env moves to `base`, till you reach a state where no envs are active.
`conda activate torch_nn_base` 

