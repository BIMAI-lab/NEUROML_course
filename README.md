# NEUROML2024



## Neuroimaging and Machine Learning for Biomedicine
This is a repository containing seminars and lecture materials for the Skoltech course on Machine Learning in Neuroimaging data, Fall 2024.

## Main links

- [Cite](https://bimai-lab.github.io/NEUROML_course/intro.html)
- [:cupid: Lab Page](http://adase.group/neuro/)
- [✈️ Telegram Channel](https://t.me/+oI9K02ZDD1NiMGQy)


## Course description:
This course is specifically aimed at MSc and PhD students with basic knowledge of Machine Learning techniques pursuing further growth in neuroimaging data analysis, either in clinical practice or in neuroscience research. The course will provide you with training in the aspects of human neuroimaging methods, data properties and applied Machine Learning techniques. The course is focused on brain biophysics, scanning techniques and methods of data analysis. Students will develop a broad set of skills that are essential to study brain function, brain pathology and solve biomedical tasks with state-of-the-art Machine Learning and Computer Vision techniques.​


### The list of the current seminars published (will be updated with time):

* SEMINAR 0 Intro
 
* SEMINAR 1  EEG analysis, Machine Learning in EEG

* SEMINAR 2 MRI data analysis, sources, databases, tools \
  **Note**: To Follow seminar you will need [docker](https://docs.docker.com/get-docker/) installed and supplementary data downloaded
  1) Install Docker;
  2) Download `NEUROML-data.zip` from [YaDisk](https://disk.yandex.ru/d/xxnRbLetEh07YQ) and unzip it to local directory;
  3) Clone [the repository](https://github.com/BIMAI-lab/NEUROML_course) to your local machine;
  4) Run docker locally and ensure it working with command `docker run hello-world`;
  5) In terminal: `cd NEUROML2022/seminar2`
  6) Type command `docker build -t neuroml/seminar2:0.0.1 .` and wait for successfull build (the dot . is importaint)
  7) Run `docker run --rm -it -v /directory/to/downloaded/data/on/step/2:/workspace/data -p 8080:8080 neuroml/seminar2:0.0.1`;\
     **Note**: If you have *Windows*, pay attention to paths, type paths in conventional powershell script `C:\directory\to\downloaded\data\on\step\2`
  8) Open browser (preferebly Chrome) -> localhost:8080
     
* SEMINAR 3 Machine Learning for structural MRI data analysis 

* SEMINAR 4 fMRI data preprocessing, analysis, GLM

  1) First follow the instruction for geting the docker image: https://miykael.github.io/nipype_tutorial/notebooks/introduction_docker.html.
  2) Clone the seminar4 repository
  3) Run the container and mount the folder: docker run -it --rm -p 8888:8888 -v /path_to_seminar-4:/home/neuro/nipype_tutorial/notebooks/seminar miykael/nipype_tutorial jupyter notebook
  4) Dowload the data from: https://www.openfmri.org/dataset/ds000114/
  
* SEMINAR 5 Functional connectivity analysis and Machine Learning modelling

* SEMINAR 6 Interpretation of ML models

* SEMINAR 7 Generative models

#### Datasets used (please get a personal account and complete data use agreement):
* Human Connectome Project https://db.humanconnectome.org/data/projects/HCP_1200
* UCLA Consortium for Neuropsychiatric Phenomics LA5c Study https://openneuro.org/datasets/ds000030/versions/1.0.0
* Autism Brain Imaging Data Exchange http://fcon_1000.projects.nitrc.org/indi/abide/
* EEG Motor Movement/Imagery Dataset https://www.physionet.org/content/eegmmidb/1.0.0/
* ADNI Alzheimer Disease Neuoroimaging Initiative https://ida.loni.usc.edu/services/NewUser.jsp

#### Software used (please get a personal account and complete usage agreement):
* FreeSurfer https://surfer.nmr.mgh.harvard.edu/
* FmriPrep https://fmriprep.org/en/stable/
* Docker https://www.docker.com/
* MNE python library https://mne.tools/stable/index.html
