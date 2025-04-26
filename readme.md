

## What are Tensors:-


### Understanding Tensors

A **tensor** is a mathematical object that generalizes the concepts of scalars, vectors, and matrices to higher dimensions. Tensors are fundamental in various fields, including physics, engineering, and machine learning, as they provide a concise way to represent and manipulate multi-dimensional data.

### Definition and Properties

In mathematics, a tensor is an algebraic **object** that describes a multilinear relationship between sets of algebraic objects related to a vector space. Tensors can map between different objects such as vectors, scalars, and even other tensors. They are defined independent of any basis, although they are often referred to by their components in a basis related to a particular coordinate system.

**Tensor Shape, Size, and Rank**

* **Tensor Shape:** The shape of a tensor refers to the layout or structure of the tensor, which defines the number of dimensions and the size of each dimension. For example, a tensor with shape (2, 3) has two dimensions, with the first dimension having a size of 2 and the second dimension having a size of 3.

* **Tensor Size:** The size of a tensor refers to the total number of elements in the tensor. It is the product of all the dimensions of the tensor. For instance, a tensor with shape (2, 3) has a size of 6 (2 * 3)

* **Tensor Rank:** The rank of a tensor, also known as its order, is the number of dimensions it has. A scalar is a rank-0 tensor, a vector is a rank-1 tensor, a matrix is a rank-2 tensor, and so on.

**Example in TensorFlow**

Here is an example of creating and manipulating tensors using TensorFlow:

```python
import tensorflow as tf

# Create a tensor
tensor = tf.constant([[1, 2, 3], [4, 5, 6]])

# Get the shape of the tensor
shape = tensor.shape
print("Tensor shape:", shape)

# Get the size of the tensor
size = tf.size(tensor)
print("Tensor size:", size)

# Get the rank of the tensor
rank = tf.rank(tensor)
print("Tensor rank:", rank)
```
Output:

```
Tensor shape: (2, 3)
Tensor size: tf.Tensor(6, shape=(), dtype=int32)
Tensor rank: tf.Tensor(2, shape=(), dtype=int32)
```

### Applications of Tensors

Tensors are widely used in various fields due to their ability to represent complex relationships and multi-dimensional data:

* **Physics:** Tensors are used to describe physical properties such as stress, strain, and electromagnetic fields.

* **Machine Learning:** In deep learning frameworks like TensorFlow and PyTorch, tensors are the basic building blocks used to represent data and perform computations.

* **Computer Vision:** Tensors are used to represent images and perform operations such as convolution and pooling


In summary, tensors are powerful mathematical objects that provide a unified framework for representing and manipulating multi-dimensional data. Understanding their properties and how to work with them is crucial for various scientific and engineering applications