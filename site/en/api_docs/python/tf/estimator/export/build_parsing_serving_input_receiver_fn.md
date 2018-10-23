

page_type: reference


<!-- DO NOT EDIT! Automatically generated file. -->
# tf.estimator.export.build_parsing_serving_input_receiver_fn

### `tf.estimator.export.build_parsing_serving_input_receiver_fn`

``` python
build_parsing_serving_input_receiver_fn(
    feature_spec,
    default_batch_size=None
)
```



Defined in [`tensorflow/python/estimator/export/export.py`](https://www.github.com/tensorflow/tensorflow/blob/r1.1/tensorflow/python/estimator/export/export.py).

Build a serving_input_receiver_fn expecting fed tf.Examples.

Creates an input_fn that expects a serialized tf.Example fed into a string
placeholder.  The function parses the tf.Example according to the provided
feature_spec, and returns all parsed Tensors as features.  This input_fn is
for use at serving time, so the labels return value is always None.

#### Args:

* <b>`feature_spec`</b>: a dict of string to `VarLenFeature`/`FixedLenFeature`.
* <b>`default_batch_size`</b>: the number of query examples expected per batch.
      Leave unset for variable batch size (recommended).


#### Returns:

  A serving_input_receiver_fn suitable for use in serving.