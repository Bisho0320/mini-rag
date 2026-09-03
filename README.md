# mini-rag
this is a minimal implementation of the rag model for question answering

## Requirements

python 3.10 or later

### Install Python using MiniConda

1. Download and install MiniConda from here
2. Create a new environment using the following command:

$ conda create -n mini-rag-app1 python=3.10 

3. Activate the environment:

$ conda activate mini-rag-app1

### (optional) setup your commandline interface for better readability

​```bash
export PS1="\[\033[01;32m\]\u@\h:\w\n[\033[00m]\$"
​```
## installation

### install the required pakages

```bash
$ pip install -r requirements.txt
```

### srtup the environment variables
 
 ```bash
 $ cp .env.example .env
 ```

 set your enviroment variables in the `.env` file. `OPENAI_API_KEY` value .

 ```bash
 $ uvicorn main:app --reload --host 0.0.0.0 --port 5000
 ```