# autoencoder

### 오토인코더의 모든 것 : 이활석(Naver) 님 강의 영상
> https://youtu.be/o_peo6U7IRM

### VAE (Variantional AutoEncoder)
> Steve Lee 님 블로그 : https://deepinsight.tistory.com/127

## REFERENCE

---

- CODESTATES | lecture note N433_AutoEncoder
- [https://deepinsight.tistory.com/124](https://deepinsight.tistory.com/124)

## AutoEncoder

---

[https://camo.githubusercontent.com/d393cc862a94453672ca7acbd91acf831fc5c36b6ae0f45cd007413ce9e788a3/68747470733a2f2f692e696d6775722e636f6d2f396a625442324f2e706e67](https://camo.githubusercontent.com/d393cc862a94453672ca7acbd91acf831fc5c36b6ae0f45cd007413ce9e788a3/68747470733a2f2f692e696d6775722e636f6d2f396a625442324f2e706e67)

> AutoEncoder의 기본적인 구조는 위 그림처럼 모래시계 형태를 띠고 있습니다.
위에 Code 라고 표시된 가장 저차원의 벡터는 **Latent(잠재) 벡터**라고도 하는데요.
AutoEncoder 에서 중요한 의미를 갖는 Latent 벡터란 무엇일까요?.
> 
- Latent(잠재) 벡터란 원본 데이터보다 차원이 작으면서도, 원본 데이터의 특징을 잘 보존하고 있는 벡터를 말하는데요.
AutoEncoder는 궁극적으로 이 Latent 벡터를 잘 얻기 위한 방법이라고 할 수 있겠습니다.
    
    ### Manifold Learning
    
    *우선 Manifold Learning에 대해 직관적으로 알아보도록 하겠습니다.*
    
    Manifold란 고차원 데이터(e.g Image의 경우 (256, 256, 3) or...)가 있을 때 고차원 데이터를 데이터 공간에 뿌리면 sample들을 잘 아우르는 subspace가 있을 것이라는 가정에서 학습을 진행하는 방법입니다.
    
    이렇게 찾은 manifold는 데이터의 차원을 축소시킬 수 있습니다.
    
    > *출처:*
    > 
    > 
    > [https://deepinsight.tistory.com/124](https://deepinsight.tistory.com/124)
    > 
    > [Steve-Lee's Deep Insight]
    > 

## **AutoEncoder 활용하기**

---

AutoEncoder의 대표적인 쓰임새는 다음과 같습니다.

- **차원 축소(Dimensionality Reduction)와 데이터 압축**
- **데이터 노이즈 제거(Denoising)**
- **이상치 탐지(Anomaly Detection)**
