

page_type: reference


<!-- DO NOT EDIT! Automatically generated file. -->
# tf.gfile.Remove

### `tf.gfile.Remove`

``` python
Remove(filename)
```



Defined in [`tensorflow/python/lib/io/file_io.py`](https://www.github.com/tensorflow/tensorflow/blob/r1.1/tensorflow/python/lib/io/file_io.py).

Deletes the file located at 'filename'.

#### Args:

* <b>`filename`</b>: string, a filename


#### Raises:

  errors.OpError: Propagates any errors reported by the FileSystem API.  E.g.,
  NotFoundError if the file does not exist.