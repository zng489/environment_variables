# System variables
```
C:\Users\PC\miniconda3\Scripts for conda in cmd
or
C:\Users\PC\miniconda3\envs for a specific python version
```

# Installing python in Visual Code
```
Installing python in Visual Code
```

# Conda Remove
```
deactivate
conda remove -n ENV_NAME --all
conda env remove -n jupyter_conda_python_3.8
```

# Environment_Variables
C:\Users\Yuan\miniconda3\envs\jupyter_conda
```
Adicionar estas 3 pastas (nessa ordem):
 C:\Users\Yuan\miniconda3\Scripts
 C:\Users\Yuan\miniconda3
 C:\Users\Yuan\miniconda3\Library\bin
=================================================================================================================
python -m venv myenv
python -m venv myenv python=3.6
=================================================================================================================
conda create -n myenv
conda create -n myenv python=3.6
=================================================================================================================
```

# Miniconda 
```
=================================================================================================================

Download >> https://docs.conda.io/en/latest/miniconda.html

Step 1 >> Latest - Conda 4.10.3 Python 3.9.5 released July 21, 2021

Step 2 >> Platform	Name	SHA256 hash Windows	Miniconda3 Windows 64-bit	
b33797064593ab2229a0135dc69001bea05cb56a20c2f243b1231213642e260a

winget install -e --id Anaconda.Miniconda3

------------------------------------------------------------------------------------------------------------------
where conda
where python

conda activate base

C:\Users\Yuan>
>> conda create --name jupyter_conda_python_3.8 python=3.8 -y
>> conda install -n conda_3.9 ipykernel --update-deps --force-reinstall  # IF NEED IT
>> conda activate jupyter_conda_python_3.8

>> conda deactivate

C:\Users\Yuan>
>> conda activate jupyter_conda_python_3.8

(jupyter_conda_python_3.8) C:\Users\Yuan>
>> pip install jupyter

(jupyter_conda_python_3.8) C:\Users\Yuan>
>> jupyter notebook
>> conda env list
********************************************************************************************************************
C:\Users\Yuan>activate jupyter_v_2.7
(jupyter_v_2.7) C:\Users\Yuan>python
********************************************************************************************************************

=================================================================================================================
pip install -r /path/to/requirements.txt


```

## Pyenv
```
where python
C:\Users\Yuan> where python
C:\Users\Yuan\AppData\Local\Programs\Python\Python310\python.exe
C:\Users\Yuan\AppData\Local\Microsoft\WindowsApps\python.exe

pyenv-win-master.zip
C:\python_v0\.pyenv\pyenv-win\bin
C:\python_v0\.pyenv\pyenv-win\shims

C:\Users\Yuan>pip install pipenv

pip list
C:\Users\Yuan> pip list

cd C:\jupyter_env> pipenv shell --python C:\Users\Yuan\AppData\Local\Programs\Python\Python310\python.exe

cd C:\jupyter_env
pipenv shell --python C:\Users\Yuan\AppData\Local\Programs\Python\Python310\python.exe

C:\python_v0\.pyenv\pyenv-win\versions\3.8.0

pip list

pipenv --venv

pipenv install pandas

pipenv shell

jupyter notebook
```


## Activating Anaconda Environment in VsCode
```
Command Prompt

settings.json
{
    "python.pythonPath":"C:\\Users\\Yuan\\miniconda3\\envs\\jupyter_conda\\python.exe"
}
```

# Opening jupyter in VSC
```
=================================================================================================================
1 - Installing and download miniconda
2 - Creating the environment and pip jupyter
3 - Opening the VSC and install the extesion for ipynb file
4 - pip uninstall if necessary!!!
=================================================================================================================
```


```
Solving environment: failed

CondaHTTPError: HTTP 000 CONNECTION FAILED for url <https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/noarch/repodata.json>
Elapsed: -

An HTTP error occurred when trying to retrieve this URL.
HTTP errors are often intermittent, and a simple retry will get you on your way.
SSLError(MaxRetryError('HTTPSConnectionPool(host=\'mirrors.tuna.tsinghua.edu.cn\', port=443): Max retries exceeded with url: /anaconda/pkgs/free/noarch/repodata.json (Caused by SSLError(SSLError("bad handshake: Error([(\'SSL routines\', \'ssl3_get_server_certificate\', \'certificate verify failed\')])")))'))
尝试重新配置源

# 重置源配置
conda config --remove-key channels 
# 重新添加清华源
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/pytorch/ 
conda config --set show_channel_urls yes
# 查看效果
cat ~/.condarc
没什么用

为防火墙的问题，通过如下命令解决

conda config --set ssl_verify false
```
