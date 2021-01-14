# EyeGotIt
Hansung Univ. Computer engineering Graduation Project
- 김상민 [Sangmeebee의 공간](https://github.com/Sangmeebee)
- 임찬호 [Lim-chano의 공간](https://github.com/Lim-chano)
- 마효리 [hyori100의 공간](https://github.com/hyori100)
- 최찬미 [cksalchl0102의 공간](https://github.com/cksalchl0102)
## 작품 개요
### <당신의 눈이 되어드립니다!> 시각장애인을 위한 길 안내 모바일 어플리케이션

## 작품 기능
* 회원가입과 로그인
```
회원가입 시 보호자와 사용자를 연동한 후 로그인 과정을 거칩니다. 
```
* 경로설정 (보호자)
```
보호자가 사용자가 자주 가는 몇 가지 경로를 클릭만으로 PIN point와 안내 텍스트를 이용하여 미리 설정합니다. 
```
* 음성으로 경로안내 (사용자) 
```
보호자가 미리 설정해 둔 경로를 사용자는 음성을 통해서 “선택” 하고 음성을 통하여 “안내” 받습니다. 
```
* 위험알림 전송
```
위험 상황 발생 시 사용자가 화면을 오른쪽으로 drag 함으로써 보호자에게 위험 알림을 전송 할 수 있습니다. 
또한, 사용자의 기기의 심각한 충돌 발생 시 보호자에게 자동으로 위험 알림이 전송됩니다. 
```
* 현재위치 전송
```
위험 상황을 대비하여 사용자가 화면을 왼쪽으로 drag 함으로써 보호자에게 현재 위치를 전송 할 수 있습니다. 
```
* [**신호등 인식과 사물 거리 인식**](https://github.com/Sangmeebee/Tensorflow-ObjectDetectionApi)
```
카메라가 장착된 안경을 사용하여 신호등의 적색신호와 녹색신호를 판별할 수 있습니다. 
또한, 물체(장애물)의 위치와 사용자 사이의 거리를 측정 할 수 있습니다. 
```

## 주요 적용 기술 및 구조

* 데이터베이스
```
HashMap 알고리즘을 이용하여 Firebase 환경 구축
```
* 지도
```
NaverColudPlatform의 Maps Api를 사용하여 Map 구축 , GPS Provider, NetworkProvider과 Maps Api의 Passive Provider로 GPS값 추출
```
* 음성인식
```
Naver Clova Speech Recognition와 Android의 Text To Speech를 통한 사용자와 앱의 상호작용
```
* [**사물인식**](https://github.com/Sangmeebee/Tensorflow-ObjectDetectionApi)
```
Tensorflow Object Detection Api를 사용하여 사물인식
```
* MQTT
```
MQTT Broker(HiveMQ)를 통하여 사용자와 보호자 연결한 뒤, Token의 Topic값으로 회원가입시 Firebase에 저장되는 topic값을 지정 
```



## 기대효과

* 위험감소
```
길찾기 기능 사용 중 신호등을 사물인식 기능으로 신호 확인 
길찾기 기능 사용 중 스스로 해결하지 못할 상황 발생 시 보호자에게 즉시 위험 알림 전송
```
* 맞춤조작
```
일반 사용자가 아닌 시각, 발달 장애인을 위한 Drag조작과 음성 인식 기술 적용
```
* 발전방향
```
많은 위험요소 사물들을 학습하여, 길찾기 기능 사용 중 위험요소를 감지하여 해결
카메라가 부착된 안경을 사용하여 사물인식 과정을 일반인의 시야와 같은 위치에서 판별
사용자가 위험알림 버튼을 누를 시 MQTT를 사용하여 보호자 뿐 아니라 근처의 경찰서로도 알림 전송
```
