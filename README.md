# SCUBANetV1+

This is a dataset that contains images of SCUBA divers interacting with
an underwater unmanned vehicle in both Warm and Cold water environments.
Object annotations for body, head and hands were produced through manual labelling.

```
usage: train.py [-h] [--yolo_model YOLO_MODEL] [--cfg_file CFG_FILE] yaml_file

positional arguments:
  yaml_file			ultralytics dataset description file

optional arguments:
  -h, --help			show this help message and exit
  --yolo_model YOLO_MODEL	YOLO version to train
  --cfg_file CFG_FILE		YOLO hyperparameters configuration 
```

## Output

This will train the chosen ultralytics model on the selected dataset (cold, warm, both). The script
will run and output training and validation metrics as well as a number of checkpoint models. You will need
the model name **best.pt**

