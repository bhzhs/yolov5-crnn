train.py

```
 # construct face related neural networks
    #cfg =[8,8,16,16,'M',32,32,'M',48,48,'M',64,128] #small model
    # cfg =[16,16,32,32,'M',64,64,'M',96,96,'M',128,256]#medium model
    cfg =[32,32,64,64,'M',128,128,'M',196,196,'M',256,256] #big model
    model = myNet_ocr(num_classes=len(plate_chr),cfg=cfg)
```

## 环境配置

1. WIN 10 or Ubuntu 16.04
2. **PyTorch > 1.2.0 (may fix ctc loss)**
3. yaml
4. easydict
5. tensorboardX

## Train

```angular2html
python train.py --cfg lib/config/360CC_config.yaml
```

结果保存再output文件夹中
