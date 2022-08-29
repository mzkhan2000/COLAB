# COLAB
My colab working repo


#### Uploading files from your local file system:

```python
from google.colab import files
uploaded = files.upload()

for fn in uploaded.keys():
  print('User uploaded file "{name}" with length {length} bytes'.format(
      name=fn, length=len(uploaded[fn])))

```

#### Downloading files to your local file system

```python
from google.colab import files
files.download('example.txt')
```


```python
text here
```


```python
text here
```


```python
text here
```
