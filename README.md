**연구 동기**

퇴행성 관절염(Osteoarthritis)은 뼈의 과증식, 윤활액 염증, 연골하 경화증, 관절 사이 좁아짐 등을 동반하는, 관절연골에서 발생하는 모든 퇴행성 질환을 일컫는다.
퇴행성 관절염은 전 세계 약 3억 명이 앓고 있는 흔한 노인성 질병 중 하나이며, 기대수명이 증가함에 따라 유병률과 발생률이 크게 늘고 있다.
이에 대한 진단은 병력 청취와 X-ray 검진을 통해 이루어지지만, 초기 관절염을 진단하기 어렵다는 단점이 있다.
뼈와 같이 큰 조직의 구조만을 감별할 수 있는 X-ray의 특성상 cartilage나 meniscus와 같은 연부조직의 구조를 파악하는 데는 기술적 한계가 있다.
그러나 PET이나 Bone scan과 같은 핵의학 영상은 다른 영상의학 기기보다 민감도가 훨씬 뛰어난데,
병변의 생리학적 변화로 인한 방사성 표지자의 흡수 변화를 통해 병변의 위치를 알아내기 때문에 이러한 문제를 극복할 수 있다.


**연구 목적**

Whole body bone scan image로부터 무릎 퇴행성 관절염 환자의 중증도를 판단하는 convolutional neural network를 구현하여 환자의 병기를 예측(Image Classification)하고,
관절염의 진행 정도에 따른 적절한 치료계획을 수립하는데 용이하게 하고자 한다.


**Data Set**

205명의 Bone scan data (강남세브란스 전태주 핵의학과 교수님, 용인세브란스 병원 정용휴 핵의학과 교수님)

Y, info, diaginfo로 구성
 - Y: 환자의 whole body bone scan data가 1024*256, uint16 type로 저장
 - info: file format, patient ID, data size, color type, 주입한 방사성 동위원소 등
 - Diaginfo: 무릎 관절에 발생한 퇴행성관절염의 중증도 6단계(Normal, minimal, mildDJD, modDJD, sevDJD, unspect)로 기술. 각 단계는 2~6 사이의 정수 및 -1로 표기

**연구 기간**

2022.03 - 2022.06
