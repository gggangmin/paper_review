# Optimization of sola cell production lines using neural networks and genetic

[paper link](https://pubs.acs.org/doi/full/10.1021/acsaem.0c01207)

### 문제

온실가스 배출량을 줄이기 위해 태양광 에너지는 매우 각광받고있다. 태양광 발전시스템(PV 시스템)은 태양광을 전기로 변환하는 시스템으로 광전지를 생산한다.
태양전지는 태양광 발전과 에너지 저장시스템(ESS)가 같이 작동하며, 전기생산과 에너지관리, 잉여생산 전기 판매, 비상전력 등으로 사용한다. 
이때 PV시스템의 제조 recipe의 전력변환 효율을 높일 수록 태양광 효율이 증가한다. 따라서 PV제조 프로세스를 최적화할 필요가 있다.
생산라인을 최적화하는 문제는 절대 쉽지않으며, 비용도 매우 많이든다. 연구를 위해서는 제조 프로세스를 반복하여 실험할 필요가 있는데
경험적인 실험은 비현실적으로 많은 실험 횟수를 요구하며 이는 현실적으로 불가능하다.
따라서 본 논문에서는 PV 시스템의 생산라인 최적화를 위한 기계학습 프레임워크를 제안한다.

### 방법

<p align="center"><img src="../resource/buratti2020optimization_1.png"></p>

논문에서 제안하는 시스템은 광전지를 생산하는 recipe를 뉴럴네트워크를 통해 학습시킨다.
여기서 뉴럴네트워크는 유전 알고리즘에 의해 반복적으로 최적화 되어 가장 좋은 recipe를 선택하게 된다. 

<p align="center"><img src="../resource/buratti2020optimization_2.png"></p>

실험에서 확인할 수 있는 것처럼 유전알고리즘의 iteration이 반복될 수록 태양전지의 효율이 증가한다. 유전알고리즘 특성상 돌연변이 선택으로 인한
약간의 분산즈악는 존재한다. 

### 공헌

태양전제 제조공정의 recipe에서 뉴럴네트워크의 도입 뿐 아니라 유전 알고리즘을 도입함으로써 효율적인 recipe을 개선하였다.

### 의견

기존의 제조공정 recipe에 뉴럴네트워크를 도입하고, 단순 뉴럴네트워크만으로 문제를 해결하지 않고 유전알고리즘을 도입함으로써 성능을 향상시킨점이 참신하다.
단순 뉴럴네트워크가 아닌 적절한 깊은 네트워크를 도입하거나, 네트워크만으로도 성능을 더욱 향상시킬 수 있을 것 같다.
