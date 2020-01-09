page_type: reference
<style>{% include "site-assets/css/style.css" %}</style>

<!-- DO NOT EDIT! Automatically generated file. -->

# tf.math.reciprocal_no_nan


<table class="tfo-notebook-buttons tfo-api" align="left">

<td>
  <a target="_blank" href="https://github.com/tensorflow/tensorflow/tree/r2.0/tensorflow/python/ops/math_ops.py#L4132-L4161">
    <img src="https://www.tensorflow.org/images/GitHub-Mark-32px.png" />
    View source on GitHub
  </a>
</td></table>



Performs a safe reciprocal operation, element wise.

### Aliases:

* `tf.compat.v1.math.reciprocal_no_nan`
* `tf.compat.v2.math.reciprocal_no_nan`


``` python
tf.math.reciprocal_no_nan(
    x,
    name=None
)
```



<!-- Placeholder for "Used in" -->

If a particular element is zero, the reciprocal for that element is
also set to zero.

#### For example:


```python
x = tf.constant([2.0, 0.5, 0, 1], dtype=tf.float32)
tf.math.reciprocal_no_nan(x)  # [ 0.5, 2, 0.0, 1.0 ]
```

#### Args:


* <b>`x`</b>: A `Tensor` of type `float16`, `float32`, `float64` `complex64` or
  `complex128`.
* <b>`name`</b>: A name for the operation (optional).


#### Returns:

A `Tensor` of same shape and type as `x`.



#### Raises:


* <b>`TypeError`</b>: x must be of a valid dtype.