# Tensorflow
TensorFlow is an open-source, high-performance library for numerical computation that uses directed graphs.
It is a scalable and multi-platform programming interface for implementing and running machine learning algorithms, including convenience wrappers for deep learning.
- supports GPU and CPU processing and is compatible with Tensor Processing Units (TPUs)
- The directed graph is a language independent representation of the code in your model. You can build a DAG in Python, store it in a saved model, restore it in C++ program for low latency prediction. Or you can use this same Python code and execute it both on CPUs, GPUs, and TPUs.

*This provides language and hardware portability**

*Language portability:*As a developer, you write your code in a high-level language like Python and have it executed in different platforms by the TensorFlow execution engine.

*Portability between devices*: enables a lot of power and flexibility. F.e. you train a TensorFlow model on the cloud on lots of powerful hardwaren. Then you take the train model and put it on a device out on the edge (mobile phone or embedded chip). Then you can do predictions with the model right on the device itself offline. --> faster response during predictions

TensorFlow has 2 main components that we will try to understand.
- Graphs
- Sessions

TensorFlow works by building a graph of defined computations. Nothing is computed or stored in this grapgh. It is simply a way of defining the operations that have been written in code.
A TensorFlow session allows parts of the graph to be executed. It allocates memory and resources and handles the execution of the operations and computations we've defined.
