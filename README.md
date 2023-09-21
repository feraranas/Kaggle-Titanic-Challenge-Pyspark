# Kaggle Titanic Challenge con Pyspark

<img src="./assets/apache-spark.png" height=80 width=300 alt="spark-logo">

## **Equipo 4**:
| <h4>Alumn</h4> | <h4>Matricula</h4> |
| ---|---|
| <h5>Mauricio Juárez Sánchez</h5> | <h5>A01660336</h5> |
| <h5>Alfredo Jeong Hyun Park</h5> | <h5>A01658259</h5> |
| <h5>Fernando Alfonso Arana Salas</h5> | <h5>A01272933</h5> |
| <h5>Miguel Ángel Bustamante Pérez</h5> | <h5>A01781583</h5> |

# Challenge Kaggle – Titanic classification

The objective of this project is to solve the Titanic - Machine Learning from Disaster problem from the Kaggle Competition using classification algorithms. Specifically, we will be using the Pyspark library in contrast to Pandas.

## Pandas vs Pyspark:
### 1. In-memory Computation
| <h4>Pandas</h4> | <h4>Pyspark</h4> |
| ---|---|
| <h5>Pandas operates primarily in-memory, which means it loads the entire dataset into memory for processing. This can be limiting when working with very large datasets that don't fit in memory.</h5> | <h5> PySpark also performs in-memory computation, but it can efficiently handle large datasets by distributing the data across a cluster's memory.</h5> |

### 2. Distributed Processing using Parallelize
| <h4>Pandas</h4> | <h4>Pyspark</h4> |
| ---|---|
| <h5>Pandas does not have native support for distributed processing or parallelization. It's designed for single-machine data analysis.</h5> | <h5>PySpark is designed for distributed processing and can parallelize computations across a cluster of machines, making it suitable for big data processing.</h5> |

### 3. Cluster Managers
| <h4>Pandas</h4> | <h4>Pyspark</h4> |
| ---|---|
| <h5>Pandas does not integrate with cluster managers like Spark, Yarn, or Mesos.</h5> | <h5>PySpark is designed to work with various cluster managers, such as Spark's built-in cluster manager, YARN, and Mesos, allowing it to leverage cluster resources efficiently.</h5> |

### 4. Fault-Tolerant
| <h4>Pandas</h4> | <h4>Pyspark</h4> |
| ---|---|
| <h5>Pandas does not have built-in fault tolerance features.</h5> | <h5>PySpark is designed for fault tolerance. It can recover from node failures in a cluster and continue processing.</h5> |

### 5. Immutable
| <h4>Pandas</h4> | <h4>Pyspark</h4> |
| ---|---|
| <h5>Pandas DataFrames are mutable, meaning you can modify them in place.</h5> | <h5>PySpark DataFrames are immutable, which means any transformation on a DataFrame creates a new DataFrame. This immutability simplifies parallel processing and fault tolerance.</h5> |

### 6. Lazy-evaluation
| <h4>Pandas</h4> | <h4>Pyspark</h4> |
| ---|---|
| <h5>Pandas does not support lazy evaluation.</h5> | <h5>PySpark supports lazy evaluation, which means transformations on DataFrames are not executed immediately but are deferred until an action is performed. This optimizes query execution.</h5> |

### 7. Cache & Persistence
| <h4>Pandas</h4> | <h4>Pyspark</h4> |
| ---|---|
| <h5>Pandas does not provide built-in mechanisms for caching or persisting data.</h5> | <h5>PySpark allows you to cache intermediate DataFrames in memory for faster access during iterative computations, improving performance.</h5> |

### 7. Inbuilt Optimization with DataFrames
| <h4>Pandas</h4> | <h4>Pyspark</h4> |
| ---|---|
| <h5>Pandas does not provide built-in optimization for distributed computing.</h5> | <h5>PySpark's DataFrames are designed for optimized distributed computing. The Catalyst query optimizer and Tungsten execution engine help improve query performance.</h5> |

### 9. Supports ANSI SQL
| <h4>Pandas</h4> | <h4>Pyspark</h4> |
| ---|---|
| <h5>Pandas does not directly support ANSI SQL, but you can use SQL-like syntax with the pandasql library.</h5> | <h5>PySpark has built-in support for ANSI SQL through its Spark SQL module, allowing you to run SQL queries on DataFrames.</h5> |
