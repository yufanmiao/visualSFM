# visualSFM
use pmvs/cmvs from pmoulon on github https://github.com/pmoulon/CMVS-PMVS.git
follow the instructions there to compile
should notice that outputlinux folder should be created in program/ rather than program/main when doing cmake
otherwise tinycthread won't be included and thus leads to compiling errors

siftGPU might be compiled but CUDA may not function correctly because if the path sepcified in the makefile of siftGPU (called "simple_find_cuda") fails, then it sets no CUDA support as defaults. This can be fixed by simply changing line 14 to "siftgpu_enable_cuda = 1" (change 0 to 1)

the other third party programs can be compiled correctly by following Scott Sawyer's tutorial http://www.10flow.com/2012/08/15/building-visualsfm-on-ubuntu-12-04-precise-pangolin-desktop-64-bit/
