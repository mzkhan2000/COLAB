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

#### use Python's pickle functionality to write the model object to a single file

```python
import pickle
pickle.dump(earthquake_embedding_model, open('earthquake_w2v_model.pkl','wb'))
# Loading model to compare the results
# model = pickle.load(open('model.pkl','rb'))
# download
from google.colab import files
files.download('earthquake_w2v_model.pkl')
# upload
from google.colab import files
uploaded = files.upload()
# load
earthquake_w2v_model = pickle.load(open('earth_w2v_model.pkl','rb'))
```


```python
text here
```


```python
text here
```
