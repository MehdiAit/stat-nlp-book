# The Stat-NLP-Book Project

## Installation 

We assume you have a command line interface in your OS 
(bash, zsh, cygwin etc.). 

### Install Git

Go to the [git installation instructions](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) 
and follow platform specific instructions. 

### Get Stat-NLP-Book Repository

Clone this repository, and enter it:
    
    git clone https://github.com/uclmr/stat-nlp-book.git
    cd stat-nlp-book

Let us assume the full stat-nlp-book path is `SNLPHOME`. 

### Install Docker

Go to the [docker webpage](https://www.docker.com/) and follow the instruction for your platform.

### Download Stat-NLP-Book Image

    docker pull riedelcastro/stat-nlp-book

### Run Notebook

    docker run -p 8888:8888 -v SNLPHOME:/home/jovyan/work riedelcastro/stat-nlp-book 

Go to the [introduction page](http://localhost:8888/notebooks/overview.ipynb). 

## Code Outside the Notebook
Assume you have a local code directory with absolute path `CODE`. 

### Running
When running code outside notebooks you can still use the 
docker image like so:

    docker run -v CODE:/home/jovyan/work riedelcastro/stat-nlp-book python3 mycode/main.py
    
### Editing 
You can edit your code in `CODE` with any editor or IDE of your choice. 
Good options are:

* PyCharm (...)
* Atom (...)
* vim etc.

