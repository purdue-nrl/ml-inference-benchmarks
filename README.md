# Running the workloads

### Steps to set up dependancies
#### Rerun torch just to make sure your version's the latest one
1. `git clone git@github.com:Aayush-Ankit/isca_workloads.git
2. `luarocks install torch`
3. `luarocks install nn`
4. `luarocks install dpnn`
5. `luarocks install torchx`
#### To use with CUDA
1. `luarocks install cutorch`
2. `luarocks install cunn`
3. `luarocks install cunnx`
#### Install RNN dependancy (allows using sequencers)
1. `cd rnn`
2. `luarocks make rocks/rnn-scm-1.rockspec`
#### Yay! Setup's Done!!!

#### Running a benchmark on CPU/GPU
`th <.lua> -gpu <0/1> -threads <non-zero> -batch <non-zero>`

### cmdline options: 
1. 'gpu 0 for CPU run, 1 for GPU run'
2. 'threads -used for CPU runs, can increase to evaluate CPU performance'



