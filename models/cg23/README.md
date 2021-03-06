### CNN for SRC steering
This model was able to drive in the simulator at ~50mph. The video is below. A writeup on the similar approach that I used for P3 is here: https://medium.com/towards-data-science/cnn-model-comparison-in-udacitys-driving-simulator-9261de09b45#.zii457ypz

The differences for the SRC model are:
- Top-down images used to train and test
- NVIDIA model layers modified for 320X160 images
- Left/right images usage commented out

#### Once your dataset folder is setup, Model is trained using
```
python SRC_model.py --dataset data/ --model cnn --nb-epoch 10 --resized-image-height 160 --resized-image-width 320
```

#### Then save the .json
```
python print_json.py
```
#### Then test in the simulator
```
python drive_new.py model.json
```

### Video is here
https://drive.google.com/drive/folders/0B2jsfsxBoDxZdXFsdktuX0gxaFU

