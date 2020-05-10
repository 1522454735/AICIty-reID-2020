## AICity-reID 2020 (track2)

![](https://github.com/layumi/AICIty-reID-2020/blob/master/heatmap2020.jpg)

In this repo, we include the 1st Place submission to [AICity Challenge](https://www.aicitychallenge.org/) 2020 re-id track (Baidu-UTS submission) [[Paper]](https://github.com/layumi/AICIty-reID-2020/blob/master/paper.pdf)

We fuse the models trained on Paddlepaddle and Pytorch. To illustrate them, we provide the two training parts seperatively as following. 

- We include the [Paddlepaddle](https://github.com/PaddlePaddle/Paddle) training code at [Here](https://github.com/miraclebiu/PaddleReid) (will update soon).
- We include the [Pytorch](https://pytorch.org/) training code at [Here](https://github.com/layumi/AICIty-reID-2020/tree/master/pytorch).

### Performance：
 AICITY2020 Challange Track2 Leaderboard
 
 |TeamName|mAP|Link|
 |--------|----|-------|
 |**Baidu-UTS(Ours)**|84.1%|[code](https://github.com/layumi/AICIty-reID-2020)|
 |RuiYanAI|78.1%|[code](https://github.com/Xiangyu-CAS/AICity2020-VOC-ReID)|
 |DMT|73.1%|[code](https://github.com/heshuting555/AICITY2020_DMT_VehicleReID)|

### Extracted Features & Camera Prediction & Direction Prediction:
You may dowanload from [GoogleDrive](https://drive.google.com/file/d/1RAQFT9umi6kTehFRiISu0g9xKI3PScbc/view?usp=sharing)
```
├── final_features/
│   ├── features/                  /* extracted pytorch feature
│   ├── pkl_feas/                   /* extracted paddle feature (include direction similarity)
│       ├── real_query_fea_ResNeXt101_32x8d_wsl_416_416_final.pkl 
|           ...
│       ├── query_fea_Res2Net101_vd_final2.pkl                 
│   ├── gallery_cam_preds_baidu      /*  gallery camera prediction
│   ├── query_cam_preds_baidu      /*  query camera prediction
|   ├── submit_cam.mat             /*  camera feature for camera similarity calculation
```

### Related Repos：

 :helicopter:  Drone-based building re-id [[code]](https://github.com/layumi/University1652-Baseline)  [[paper]](https://arxiv.org/abs/2002.12186)
 
[Vehicle re-ID Paper Collection] https://github.com/layumi/Vehicle_reID-Collection

[Person re-ID Baseline] https://github.com/layumi/Person_reID_baseline_pytorch

[Person/Vehicle Generation] https://github.com/NVlabs/DG-Net
