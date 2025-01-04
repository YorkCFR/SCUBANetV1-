# SCUBANetV1+

This is a dataset that contains images of SCUBA divers interacting with an underwater unmanned vehicle in both Warm and Cold water environments. Object annotations for body, head and hands were produced through manual labelling.

The original work is described in R. Codd-Downey and M. Jenkin, "Finding divers with SCUBANet," 2019 International Conference on Robotics and Automation (ICRA), Montreal, QC, Canada, 2019, pp. 5746-5751, doi: 10.1109/ICRA.2019.8793655. The work described in the original work has been augmented with additional data and has been re-structured so as to be structured for Yolo. See the references below for a full set of references for this work.

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

## References
R. Codd-Downey and M. Jenkin, "Finding divers with SCUBANet," 2019 International Conference on Robotics and Automation (ICRA), Montreal, QC, Canada, 2019, pp. 5746-5751, doi: 10.1109/ICRA.2019.8793655. 

R. Codd-Downey. Underwater gesture-based human-to-robot communication. PhD Thesis. Computer Science. York University, 2024.


