---
tags:
  - Y2018
  - "#CVPR"
  - "#Quantization"
link: https://arxiv.org/pdf/1712.05877.pdf
Main Author:
  - Bita Rouhani
Organization:
  - Microsoft
  - Meta
---


# Introduction

다양한 목적의 많은 인공지능 관련 연구는 효율성을 위해서 연산 속도를 개선하기 위한 여러 노력들을 해 왔다. 그 중 한 방향성은 [[MobileNet]], [[SqueezeNet]], [[ShuffleNet]], [[DenseNet]]과 같이 새로운 네트워크 구조를 제안해서 성능을 개선하려는 것이고, 다른 방향성은 [[TWN]], [[BNN]], [[XNOR-net]]과 같이 낮은 bit width을 사용해서 성능을 확보하려는 방식이다.

이전 연구들은 두 가지 점에서 부족한 부분이 있다.
1. 첫 번째는 적당한 모델을 사용하지 않았다는 점으로, [[AlexNet]], [[VGG]], [[GoogleNet]]의 경우 이미 네트워크 파라미터가 너무 많아서 압축을 많이 진행하더라도 성능 손해를 많이 안 볼 가능성이 크다. 따라서 [[MobileNet]]과 같이 이미 속도를 위해서 어느 정도 정확도를 손해 보고 있는 네트워크를 대상으로 실험하는 것이 바람직하다.
2. 두 번째는, 
