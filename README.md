# conda
conda remove -n ENV_NAME --all  
conda create --name myenv python=3.10

# git clone lfs  
git lfs install  
git clone <https....>

# git 上傳工作區檔案  
git init  # 在本地建立git工作區  
git add "folder" # 將工作區資料夾上傳到暫存區    
git commit -m "folder name"  # 將暫存區檔案上傳到repo  
git remote add origin <https....>  
git push -u origin master  
  
git push origin -d <branch...>  # delete remote branch  
git branch -D <branch...> # Force-delete un-merged local branches  
