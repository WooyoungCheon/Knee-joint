
**연구 목적**

Whole body bone scan image로부터 무릎 퇴행성관절염 환자의 중증도를 판단하는 convolutional neural network를 구현하여 환자의 병기를 예측하고,
관절염의 진행 정도에 따른 적절한 치료계획을 수립하는데 용이하게 하고자 한다.


**Data Set**

205명의 Bone scan data (강남세브란스 전태주 핵의학과 교수님, 용인세브란스 병원의 정용휴 핵의학과 교수님
Y, info, diaginfo로 구성
 - Y: 환자의 whole body bone scan data가 1024*256, uint16 type로 저장
 - info: file format, patient ID, data size, color type, 주입한 방사성 동위원소 등
 - Diaginfo: 무릎 관절에 발생한 퇴행성관절염의 중증도 6단계(Normal, minimal, mildDJD, modDJD, sevDJD, unspect)로 기술. 각 단계는 2~6 사이의 정수 및 -1로 표기

