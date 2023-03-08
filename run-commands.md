# Training
## command
1. Generate the training partitions for each submodule: ```python create_cluster_masks.py --config configs/mega-nerf/building.yaml --dataset_path dataset/building-pixsfm  --output mask-path --grid_dim 2 4```
2. Train each submodule: ``````
3. Merge the trained submodules into a unified Mega-NeRF model: ``````
# Evaluation
## command
        python eval.py --config_file configs/mega-nerf/building.yaml  --exp_name logs/building-pixsfm-8 --dataset_path dataset/building-pixsfm --container_path pretrain/building-pixsfm-8.pt
## file_structure
![1](https://user-images.githubusercontent.com/57701854/223612905-4fb25b7e-162c-45a3-a0ee-01c164af115a.png)
![2](https://user-images.githubusercontent.com/57701854/223612995-de339c1c-080e-4498-b90e-1a5d0de9f092.png)
![3](https://user-images.githubusercontent.com/57701854/223613014-704c6fb0-aaeb-4432-ab47-340ffe317355.png)

