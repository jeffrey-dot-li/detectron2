```bash
wget -O model/model_final.zip https://www.dropbox.com/sh/1098ym6vhad4zi6/AABe16eSdY_34KGp52W0ruwha?dl=0
```

```bash
unzip model/model_final.zip -d model/
```

```bash
python demo/demo.py --config-file configs/DLA_mask_rcnn_X_101_32x8d_FPN_3x.yaml --input test.png --output test_output.png --confidence-threshold 0.5 --opts MODEL.WEIGHTS model/model_final_trimmed.pth MODEL.DEVICE cuda
```
