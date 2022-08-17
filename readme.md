Run the below commands:

> python gen_optical_flow.py

> python create_train_test_split.py

> python build_file_list.py

> python main_single_gpu.py /datasets/gms_frames -m rgb -a rgb_resnet152 --new_length=1 --epochs 250 --lr 0.001 --lr_steps 100 200 --iter-size 2 --print-freq 2 --save-freq 25 

> python main_single_gpu.py /datasets/gms_frames -m flow -a flow_resnet152 --new_length=10 --epochs 350 --lr 0.001 --lr_steps 200 300 --iter-size 2 --print-freq 2 --save-freq 35 
