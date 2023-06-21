# Audio-visual quality assessment
The data set used in the experiment is LIVE-SJTU
## 1.Obtain the features extracted by Vision Transformer
get the pretrained ViT model by rwightman\,save them at ./pretrained_models.link:\
https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-vitjx/jx_vit_base_patch16_224_in21k-e5005f0a.pth \
https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-vitjx/jx_vit_large_patch16_224_in21k-606da67d.pth
````
python feature_extractor/feature_extractor.py --input (path) --output (path)
````
## 2.Train the AVQA model
````
python train.py --epoch (epoch) --learning_rate (learning_rate) --batch_size (batch_size) --data_path (data_path)
````
## Results
trainlog : ./log/avqa.log\
plot : ./log/avqa.png
