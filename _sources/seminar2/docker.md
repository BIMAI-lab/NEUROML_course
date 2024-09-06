# Preparation to the seminar 2

```{contents}
```
## SEMINAR 2 MRI data analysis 
**Note**: To Follow seminar you will need [docker](https://docs.docker.com/get-docker/) installed and supplementary data downloaded
  1) [Install Docker](https://docs.docker.com/engine/install/);
  2) Download `NEUROML-data.zip` from [YaDisk](https://disk.yandex.ru/d/xxnRbLetEh07YQ) and unzip it to local directory;
  3) Clone repository to your local machine;
  4) Run docker locally and ensure it working with command `docker run hello-world`;
  5) In terminal: `cd NEUROML_course/seminar2`
  6) Type command `docker build -t neuroml/seminar2:0.0.1 .` and wait for successfull build (the dot . is importaint)
  7) Run `docker run --rm -it -v /directory/to/downloaded/data/on/step/2:/workspace/data -p 8080:8080 neuroml/seminar2:0.0.1`;\
     **Note**: If you have *Windows*, pay attention to paths, type paths in conventional powershell script `C:\directory\to\downloaded\data\on\step\2`
  8) Open browser (preferebly Chrome) -> localhost:8080
     

Docker tutorials:
- [Installation](https://docs.docker.com/engine/install/)
- [Introduction to neurodocker](https://miykael.github.io/nipype_tutorial/notebooks/introduction_neurodocker.html)
- [Introduction to docker](https://miykael.github.io/nipype_tutorial/notebooks/introduction_docker.html)


## References

```{bibliography}
:style: plain
:filter: docname in docnames
```
