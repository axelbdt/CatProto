# Zero to Catlab with Julia

## Install Julia

https://julialang.org/downloads/

or via package manager :
```
sudo apt install julia
```

## Generate Catlab.jl notebooks

### Get the Catlab.jl code

```shell
git clone https://github.com/AlgebraicJulia/Catlab.jl.git
cd Catlab.jl/docs
# open julia repl
julia
```

### Install the dependencies

From the repl, switch to pkg mode by typing `]`. The prompt should change to `pkg>`.
```
activate .
instantiate
```
Backspace to exit pkg mode. Prompt changes back to `julia>`.

### Build the docs project to generate the notebooks

Switch to shell mode by typing `;`. Prompt changes to `shell`.
```shell
julia --project=. main.jl
```
Build can take a while, but should generate Jupyter notebooks into a directory `generated`. 

Open the Catlab.jl project with VSCode, open the notebooks.

Enjoy :)