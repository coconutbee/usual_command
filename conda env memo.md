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
