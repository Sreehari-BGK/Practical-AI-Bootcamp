# Tasks for the bootcamp

## Day 3

You learnt [data augumentation in tf.data](https://github.com/tinkerhub/Practical-AI-Bootcamp/blob/main/Resources/Day%203/README.md#tfdata) and data augumentation on input pipelines. Click [here](https://www.tensorflow.org/text) to find a tool for applying preprocessing to text data. Apply `text.normalize_utf8` to the below loaded dataset

```python
import tensorflow as tf

directory_url = 'https://storage.googleapis.com/download.tensorflow.org/data/illiad/'
file_names = ['cowper.txt', 'derby.txt', 'butler.txt']

file_paths = [
    tf.keras.utils.get_file(file_name, directory_url + file_name)
    for file_name in file_names
]

dataset = tf.data.TextLineDataset(file_paths)
```
