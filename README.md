# conda env command MEMO
### conda create env
```python
conda env create --name [myENV] python=[version]
```

### activate env 
```python
conda activate [myENV]
```

### deactivate env
```python
conda deactivate
```

### conda remove env
```python
conda remove --name [myENV] --all
```

### conda store env config (freeze.yml)
```python
conda env export --no-builds > freeze.yml
```
### conda create env with yml file (freeze.yml)
```python
conda env create -f freeze.yml
```

# Python Virtual Environment
## python venv
```bash
python3 -s -m venv "env_name"  
source .sd3.5/bin/activate  # linux activate  
.sd3.5\Scripts\activate  # window activate  
deactivate  
```
# nvidia
### nvidia
```bash
watch -n 1 nvidia-smi  # watch GPU status
```

# Git commands
### git clone lfs  
```bash
git lfs install  
git clone <https....>
```

### git 創建/上傳工作區檔案  
```bash
git init  # 在本地建立git工作區  
git add README.md  
git add "folder" # 將工作區資料夾上傳到暫存區    
git commit -m "folder name"  # 將暫存區檔案上傳到本地repo  
git remote add origin "https...."  #添加organize的遠端repo
git push -u origin main     
```
### git 抓資料下來
```bash
git fetch "branch name" # 將最新進度加到本地端
git fetch [遠端節點名稱] [branch name]
git branch -r # 檢查remote branch
git push [遠端節點名稱] [branch name] # 將本地版本上傳到遠端合併
```

### git remove branch  
```bash
git push origin -d <branch...>  # delete remote branch  
git branch -D <branch...> # Force-delete un-merged local branches  
```

### git usual command  
```bash
git status  
git log  
git rm "file"
git checkout "Branch name"
git branch # check all branch
```

# Stable Diffusion
### Download sd3.5 model by ssh way  
1. if you don't have a ssh key on hugging face:  
   1.  ssh-keygen -t rsa -b 4096 -C "your_email@example.com" # generate a key  
   2.  cat ~/.ssh/id_rsa.pub # copy the content starting with "ssh-rsa" till the end  
   3.  paste your key on "SSH & GPG Keys" -> "Add SSH Key"  
2. git lfs install  
3. git clone git@hf.co:stabilityai/stable-diffusion-3.5-large  


