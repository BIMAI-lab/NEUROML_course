# seminar-4

## Prerequisites

### Step 1.

Pull docker image from docker registry:  
``` docker pull miykael/nipype_tutorial:latest ```  
(make sure that docker daemon on your computer is working)  
In case of any troubles please read this [instruction](docker pull miykael/nipype_tutorial:latest)
### Step 2.
Clone this repository.

### Step 3.
Run this command to run docker container with mounted directory of the seminar.  

```docker run -it --rm -p 8888:8888 -v <PATH_TO_SEMINAR_4_ON_YOUR_PC>:/home/neuro/nipype_tutorial/notebooks/seminar miykael/nipype_tutorial jupyter notebook ```  
Note that ```<PATH_TO_SEMINAR_4_ON_YOUR_PC>``` is a global path to the seminar 4 directory on your computer.  
Don't forget to copy the token of your jupyter server (check the terminal). Then detach your container (```CTRL+P+Q```) just in case. If everything is okay, the jupyter server can be reached at http://localhost:8888/.  

## FAQ.
In case of any problem with datalas during datased pulling (I faced it on the machines with M1* chips) please download dataset from [here](https://disk.yandex.ru/d/Q2dZs2CoM2Sohw). Then please put the archive to the mounted directory from the previous step. Next you need to unarchive data. In order to do so please attach to you docker container ```docker exec -ti -u root <CONTAINER NAME>```. Container name can be checked by means of this command ```docker ps```. Then inside your container please run ```tar -xf <ARCHIVE_NAME>.tar```.  Make sure to specify the correct path to data inside all of your notebooks.

Also I uploaded all artifacts (preprocessed data etc.) obtained during two parts of the seminar [here](https://disk.yandex.ru/d/V5N05i337wUw_g). In case of any problem with notebook execution you can simply take it and use. The procedure of using this data is the same as for dataset% download, move, unarchive, specify correct pathes.

#### Dataset:
* A test-retest fMRI dataset for motor, language and spatial attention functions https://www.openfmri.org/dataset/ds000114/
