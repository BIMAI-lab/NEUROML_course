# Preparation to the seminar 4

```{contents}
```
## SEMINAR 4 (20.09) fMRI data preprocessing, analysis, GLM
**Note**: To Follow seminar you will need [docker](https://docs.docker.com/get-docker/) installed and supplementary data downloaded
 
1) First follow the [instruction for getting the docker image](https://miykael.github.io/nipype_tutorial/notebooks/introduction_docker.html).
2) Clone the seminar4 repository
3) Run the container and mount the folder: `docker run -it --rm -p 8888:8888 -v /path_to_seminar-4:/home/neuro/nipype_tutorial/notebooks/seminar miykael/nipype_tutorial jupyter notebook`
4) Dowload the data from: [https://www.openfmri.org/dataset/ds000114/](https://www.openfmri.org/dataset/ds000114/)
5) Open browser (preferebly Chrome) -> localhost:8888
     

Docker tutorials:
- [Installation](https://docs.docker.com/engine/install/)
- [Introduction to neurodocker](https://miykael.github.io/nipype_tutorial/notebooks/introduction_neurodocker.html)

## References

```{bibliography}
:style: plain
:filter: docname in docnames
```
