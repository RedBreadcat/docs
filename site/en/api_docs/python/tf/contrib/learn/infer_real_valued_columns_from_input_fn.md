

page_type: reference
<style> table img { max-width: 100%; } </style>


<!-- DO NOT EDIT! Automatically generated file. -->


# tf.contrib.learn.infer_real_valued_columns_from_input_fn

``` python
tf.contrib.learn.infer_real_valued_columns_from_input_fn(input_fn)
```



Defined in [`tensorflow/contrib/learn/python/learn/estimators/estimator.py`](https://www.github.com/tensorflow/tensorflow/blob/r1.7/tensorflow/contrib/learn/python/learn/estimators/estimator.py).

See the guide: [Learn (contrib) > Input processing](../../../../../api_guides/python/contrib.learn#Input_processing)

Creates `FeatureColumn` objects for inputs defined by `input_fn`. (deprecated)

THIS FUNCTION IS DEPRECATED. It will be removed in a future version.
Instructions for updating:
Please specify feature columns explicitly.

This interprets all inputs as dense, fixed-length float values. This creates
a local graph in which it calls `input_fn` to build the tensors, then discards
it.

#### Args:

* <b>`input_fn`</b>: Input function returning a tuple of:
      features - Dictionary of string feature name to `Tensor` or `Tensor`.
      labels - `Tensor` of label values.


#### Returns:

List of `FeatureColumn` objects.