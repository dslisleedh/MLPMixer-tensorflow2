<h1> MLP-Mixer: An all-MLP Architecture for Vision [arXiv](https://arxiv.org/abs/2105.01601) </h1> 

![MLP-Mixer](https://camo.githubusercontent.com/6f01197a711dee4f81441f2e6fef577f72ab8b36f1ddeea03d30ecada3e10d72/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f333339382f312a635548643647396a6a776c3946377858765f534245772e6a706567)
<h3>
요약 : 
Multi-Head Self Attention대신 단순히 Fully-Connected Layer만 사용해도 이미지에서 global/local information을  모두 가져 올 수 있음.
</h3>



<h5>
2가지 MLP로 구성함. 하나는 Token(spatial)간의 교환을 하는 token mixing MLP, 하나는 채널내의 교환을 하는 channel mixing MLP 
단순히 Feature map을 transpose하면서 각각 MLP에 넣음으로써 Self Attention보다 더 적은 hyperparameter로 유사한 성능을 이끌어냄.  
</h5>

<h4>
CNN보다 Global하게 볼 수 있고(random mixing을 했을 때 성능이 더 좋음) 계산 효율이 더 좋으며,  
Transfomer보다 더 Local하게 볼 수 있고(local information에 inductive bias가 더 들어감) 계산 효율이 더 좋음.
</h4>
