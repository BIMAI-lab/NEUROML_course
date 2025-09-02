# Introduction to neuroscience and neuroimaging

```{contents}
```
## Artificial Intelligence in Medical Imaging


```{figure} figs/AI_in_neuro.png
:name: ai_neuro
Artificial Intelligence tasks in Medical Imaging.
```


## Datasets 

Datasets used (please get a personal account and complete data use agreement):
- [Human Connectome Project](https://db.humanconnectome.org/data/projects/HCP_1200)
- [UCLA Consortium for Neuropsychiatric Phenomics LA5c Study](https://openneuro.org/datasets/ds000030/versions/1.0.0)
- [Autism Brain Imaging Data Exchange](http://fcon_1000.projects.nitrc.org/indi/abide/)
- [EEG Motor Movement/Imagery Dataset](https://www.physionet.org/content/eegmmidb/1.0.0/)
- [ADNI Alzheimer Disease Neuoroimaging Initiative](https://ida.loni.usc.edu/services/NewUser.jsp)

## Software 

Software used (please get a personal account and complete usage agreement):
- [FreeSurfer](https://surfer.nmr.mgh.harvard.edu/)
- [FmriPrep](https://fmriprep.org/en/stable/)
- [Docker](https://www.docker.com/)
- [MNE python library](https://mne.tools/stable/index.html)

## MRI Machine Learning and Deep Learning Tools

Python libraries for the analysis of neuroimaging data (see more in the [nipy.org](https://nipy.org/)):
- [Nibabel](https://nipy.org/nibabel/)
- [Nilearn](https://nilearn.github.io/stable/)

Deep Learning:
- [Monai](https://github.com/Project-MONAI/MONAI)
- [TorchIO](https://github.com/fepegar/torchio)
- [PyTorch Lightning](https://github.com/Lightning-AI/pytorch-lightning)
- [Weights&Bias](https://docs.wandb.ai/?_gl=1*1nqe5p*_ga*MTU1NTY2MDQwNS4xNjYyMzY5NTg4*_ga_JH1SJHJQXJ*MTY2MjM2OTU4OC4xLjEuMTY2MjM2OTY3NS41OC4wLjA.)

More Deep Learning tools for MRI you can find in [GitHub Repository](https://github.com/kondratevakate/mri-deep-learning-tools) (last update in 2022).

## Docker

Top docker commands:
- docker run hello-world #test
- docker pull miykael/nipype_tutorial:latest # pulling images
- docker images # to check available images on your system
- docker run -it --rm -v /path/to/nipype_tutorial/:/home/neuro/nipype_tutorial -v /path/to/data/:/data -v /path/to/output/:/output -p
8888:8888 miykael/nipype_tutorial jupyter notebook
- docker run --rm kaczmarj/neurodocker:v0.4.0 generate [docker|singularity] --base neurodebian:stretch --pkg-manager apt --install afni ants git vim
- docker rmi -f IMAGE_ID # To delete a specific docker image
- docker exec -it IMAGE_ID /bin/bash # runs a new command in a running container.
- docker save -o nipype_tutorial.tar miykael/nipype_tutorial # Export docker image miykael/nipype_tutorial
- docker load --input nipype_tutorial.tar # Import docker image on another PC

Docker tutorials:
- [Installation](https://docs.docker.com/engine/install/)
- [Introduction to neurodocker](https://miykael.github.io/nipype_tutorial/notebooks/introduction_neurodocker.html)
- [Introduction to docker](https://miykael.github.io/nipype_tutorial/notebooks/introduction_docker.html)

## Python intro

If you haven't worked with Python before and don't understand what's going on, see other parts of Introduction.

## Survey

Please, take a [survey](https://forms.gle/zLpkUA2VTYtEmHZm9). It will help us to adjust course to your skills.  


## Credits
This text prepared by Polina Druzhinina and Nadezhda Alsahanova.

## References

```{bibliography}
:style: plain
:filter: docname in docnames
```
