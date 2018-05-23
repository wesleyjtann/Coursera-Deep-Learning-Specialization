# [Coursera Deep Learning Specialization](https://www.coursera.org/specializations/deep-learning)

In these five courses, it teaches the foundations of Deep Learning, understand how to build neural networks, and learn how to lead successful machine learning projects. Topics covered include:

    *Convolutional networks 
    *RNNs 
    *LSTM 
    *Adam 
    *Dropout 
    *BatchNorm 
    *Xavier/He initialization, and more 

All topics are practiced in Python and in TensorFlow. 


### Course 1. Neural Network and Deep Learning
This course teaches the foundations of deep learning.

    * Week 1 Introduction to deep learning
    * Week 2 Neural Networks Basics
    * Week 3 Shallow neural networks
    * Week 4 Deep Neural Networks
   

### Course 2. Improving Deep Neural Networks: Hyperparameter tuning, Regularization and Optimization
This course teaches the "magic" of getting deep learning to work well. 

    * Week 1 Practical aspects of Deep Learning
    * Week 2 Optimization algorithms
    * Week 3 Hyperparameter tuning, Batch Normalization and Programming Frameworks


### Course 3. Structuring Machine Learning Projects
This course teaches the art of building successful machine learning projects. 

    * Week 1 ML Strategy (1)
    * Week 2 ML Strategy (2)


### Course 4. Convolutional Neural Networks
This course teaches the building of convolutional neural networks and applying it to image data. 

    * Week 1 Foundations of Convolutional Neural Networks
    * Week 2 Deep convolutional models: case studies
    * Week 3 Object detection
    * Week 4 Special applications: Face recognition & Neural style transfer


### Course 5. Sequence Models
This course teaches the building of models for natural language, audio, and other sequence data. 

    * Week 1 Recurrent Neural Networks
    * Week 2 Natural Language Processing & Word Embeddings
    * Week 3 Sequence models & Attention mechanism



### Instructions for downloading Jupyter Notebooks from Coursera 
From an open Jupyter Notebook homework assignment, select "Coursera" to take you to the home page in Jupyter Notebook.

Make a new notebook and fill it with the following and excute the cell with:

    %%bash
    tar cvfz hw.tar.gz .
    
This may take a little while to run depending on the packages.
Select "Coursera" again to take you to the Home directory.
Check the hw.tar.gz file and then Download.
After the file is downloaded, delete it.

If the file is too big, you may get an error and have to restart. If so, try the following instead, remembering to delete any tar files created.

    %%bash
    for dir in */
    do
      base=$(basename "$dir")
      tar -czf "${base}.tar.gz" "$dir"
    done
    find . -maxdepth 1 -type f -exec tar cvfz hw.tar.gz {} +
    
    


