# pytorch-ddp
code for the Distributed Data Parallel using Pytorch


# 1 gpu
Accuracy of the network on the 10000 test images: 27 %
Total elapsed time: 69.03 seconds,      Train 1 epoch 13.08 seconds


# DDP 
```
python -m torch.distributed.launch --nproc_per_node=4 train_ddp.py
```
## ddp 4gpus
Accuracy of the network on the 10000 test images: 14 %
Total elapsed time: 70.23 seconds,      Train 1 epoch 6.11 seconds

## ddp 2gpus
Accuracy of the network on the 10000 test images: 19 %
Total elapsed time: 97.03 seconds,      Train 1 epoch 9.79 seconds


## mixed precision ddp 4gpus
Accuracy of the network on the 10000 test images: 15 %
Total elapsed time: 70.61 seconds,      Train 1 epoch 6.52 seconds
