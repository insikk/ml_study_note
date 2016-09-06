# Neural Networks Tips and Tricks, Recurrent Neural Networks


## 스터디 자료

[1] [cs224d lecture slide lec06](http://cs224d.stanford.edu/lectures/CS224d-Lecture6.pdf)

[2] 

## NOTE

### General Strategy for Implementing Model

1. Select appropriate Network Structure
  
  1.1 Structure: Single words, fixed windows vs Recursive Sentence Based vs Bag of words
  
  1.2. Nonlinearity

2. Check for implementation bugs with gradient check 
3. Parameter initialization

  For the very first propagation make sure the activation occurs around linear region of the activation function.

4. Optimization tricks

  * Never use full batch method.
  * mini batch SGD
  * momentum
  * decrease learning rate once validation error stops decreasing.
  * AdaGrad
  
5. Check if the model is powerful enough to overfit
  
  5.1. If not, change model structure or make model "larger"
  
  5.2. If you can overfit: Regularize
  

## 키워드

### Neural Networks Tips and Tricks

Gradient Check, Stochastic Gradient Descent (SGD), Mini batches (size 20 to 1000), momentum, AdaGrad, Dropout, Random hyperparameter search
  

### Recurrent Neural Networks


## 질문과 답변
