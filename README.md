# Blockchain Integration for in-Vehicle CAN Bus Intrusion Detection Systems with ISO/SAE 21434 Compliant Reporting
This repository contains the datasets that we collected and used for the experimental part of our paper, "Blockchain Integration for in-Vehicle CAN Bus Intrusion Detection Systems with ISO/SAE 21434 Compliant Reporting."

# Folder structure
|------ Datasets \
|&nbsp;&nbsp;&nbsp;|------ Original datasets (no attacks) \
|&nbsp;&nbsp;&nbsp;|------ Datasets containing attacks \
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|------ Fuzzing \
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|------ Vehicle A \
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|------ Vehicle B \
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|------ Vehicle C \
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|------ Replay \
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|------ Vehicle A \
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|------ Vehicle B \
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|------ Vehicle C \
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|------ Combined \
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|------ Vehicle A \
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|------ Vehicle B \
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|------ Vehicle C 

## File structure ##
**The CAN datasets** are stored as ASCII Logging Files (.asc), with data structured according to Vector's format (for more information, see [Vector's webpage](https://support.vector.com/kb?id=kb_article_view&sysparm_article=KB0011536&sys_kb_id=b6d21110870d4550b9f233770cbb3523&spa=1)).
The final datasets, resulting after feature extraction, are stored as CSV files. Each row (used in the classification of the current CAN frame) contains the following information: the ID of the CAN frame, the IDs of the previous 4 CAN frames, and the data field of the current CAN frame. In addition, the last byte on each row indicates if the current frame is legitim (value 0) or attack (value 1).

## Data links ##
File | Download | Notes
--- | :---------: | :----
**datasets_no_attacks.zip** | [link1 (University website)](https://www.aut.upt.ro/~bgroza/projects/cloud-ids/datasets_no_attacks.zip) <br /> [link2 (OneDrive)](https://1drv.ms/u/s!AgEIEIfZbk8C1FfpfHfDyE1EK8Ch?e=w8admT) | Original datasets collected from three Duster vehicles
**datasets_with_attacks.zip** | [link1 (University website)](https://www.aut.upt.ro/~bgroza/projects/cloud-ids/datasets_with_attacks.zip) <br /> [link2 (OneDrive)](https://1drv.ms/u/s!AgEIEIfZbk8C1FgBV973Sth-0g5G?e=Xeie7j) | Datasets augmented with attacks
