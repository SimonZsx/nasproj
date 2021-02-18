
Test weight inheritance (weight sharing) converge


Use pretrained model, re initialize part of the model parameters 

 nohup python3 test.py -a resnet18 --pretrained --lr 0.1 ../datasets/imagenet >wshare.log 2>&1 &




Original 

 nohup python3 imagenet.py -a resnet18 --lr 0.1 ../datasets/imagenet >original.log 2>&1 &  


Ours

python3 inherit.py -a resnet18 --pretrained --lr 0.1 ../datasets/imagenet


