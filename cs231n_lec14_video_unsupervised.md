# ConvNets for videos, Unsupervised learning


## 스터디 자료

[1] [cs231n lecture slide lec14](http://cs231n.stanford.edu/slides/winter1516_lecture14.pdf)

[2] [Machine Learning 스터디 (19) Deep Learning - RBM, DBN, CNN](http://sanghyukchun.github.io/75/)

## 키워드

### Videos

Optical Flow, Spatio-Temporal ConvNets, 3D ConvNets, GRU-RCN

### Unsupervised Learning

Autoencoder, Variational Autoencoder, Generative Adversarial Networks


## 질문과 답변

Autoencoder가 요즈음(2016년) 들어서 많이 안쓰이는 이유는?
> 두 가지 이유가 존재하는데 다음과 같다.
>
> 1. 2016년 현 시점 기준으로 deep learning network를 훈련시키기에 충분한 양의 labeled data를 확보하기 쉬워졌다. 
> 2. ReLU, proper initialization, batch norm, adam 등의 고급 기법으로 인해 pre-training 과정없이 end-to-end로 모델을 훈련시키는 것이 가능해짐. 
>

> Autoencoder가 나온 배경을 보면 2006년경에 deep nueral network (4 layer 이상)을 훈련시키는 것이 힘든 것을 해결하고자 나왔다.
> Autoencoder를 이용하면 unlabeled data에 대해서 스스로 의미있는 feature를 찾아내는 미리 훈련된 네트워크를 가지고 시작 할 수 있다. (weight initialization 문제 해결)
> 이후에 fine-tuning 과정을 거쳐 완성된 classifier를 만든다. 
> 현재도 labeled된 데이터가 부족하다면 pre-training의 아이디어를 시도해 볼 수 있겠다. 
>
>> 자료 [2]에 따르면 "NIPS 2006에 발표된 Bengio 교수 연구팀의 Greedy layer-wise training of deep networks 연구와 NIPS 2007에 발표된 Hinton 교수 연구팀의 A fast learning algorithm for deep belief nets 두 논문을 통해 제안되었던 unsupervised pretraining method"가 있으며, "이 부분은 더 이상 practical usage로 사용되지는 않지만, deep learning의 거의 첫 번째 연구결과라고 해도 좋을 정도로 의미있는 연구결과" 이므로 알아둘만한 방법이라고 한다.
 
