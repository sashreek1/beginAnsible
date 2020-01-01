# Begin Ansible
An ansible playbook to help install tensorflow  
  
## What is TensorFlow ?  
![Alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/1/11/TensorFlowLogo.svg/420px-TensorFlowLogo.svg.png?raw=true "Title")

TensorFlow is a free and open-source software library for dataflow and differentiable programming across a range of tasks. It is a symbolic math library, and is also used for machine learning applications such as neural networks.  
  
It was built to run on multiple CPUs or GPUs and even mobile operating systems, and it has several wrappers in several languages like Python, C++ or Java. 
  
## How does it work ?  
TensorFlow allows developers to create dataflow graphs—structures that describe how data moves through a graph, or a series of processing nodes. Each node in the graph represents a mathematical operation, and each connection or edge between nodes is a multidimensional data array, or tensor.
  
## A simple TensorFlow script 
  
This is a simple python script using TensorFlow to multiply 2 tensorflow constan
```python
import tensorflow as tf

x1 = tf.constant([1,2,3,4])
x2 = tf.constant([5,6,7,8])

result = tf.multiply(x1, x2)

sess = tf.Session()

print(sess.run(result))

sess.close()
```
Note : We must use TensorFlow sessions here because without starting a session we will not be able to see any output.
