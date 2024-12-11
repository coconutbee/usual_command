# conda
conda remove -n ENV_NAME --all  
conda create -n ENV_NAME python=3.10

# python venv
python3 -s -m venv <env_name>  
source .sd3.5/bin/activate  # linux activate  
.sd3.5\Scripts\activate  # window activate  
deactivate  

# nvidia
watch -n 1 nvidia-smi  # watch GPU status

# git clone lfs  
git lfs install  
git clone <https....>

# git 上傳工作區檔案  
git init  # 在本地建立git工作區  
git add "folder" # 將工作區資料夾上傳到暫存區    
git commit -m "folder name"  # 將暫存區檔案上傳到本地repo  
git remote add origin <https....>  
git push -u origin main    
  
git push origin -d <branch...>  # delete remote branch  
git branch -D <branch...> # Force-delete un-merged local branches  

# Download sd3.5 model by ssh way  
1. if you don't have a ssh key on hugging face:  
   1.  ssh-keygen -t rsa -b 4096 -C "your_email@example.com" # generate a key  
   2.  cat ~/.ssh/id_rsa.pub # copy the content starting with "ssh-rsa" till the end  
   3.  paste your key on "SSH & GPG Keys" -> "Add SSH Key"  
2. git lfs install  
3. git clone git@hf.co:stabilityai/stable-diffusion-3.5-large  


