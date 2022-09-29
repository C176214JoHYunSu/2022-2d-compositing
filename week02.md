
Week 02
=============

Colorspace
-------------
 R/G/B/A
>컴퓨터 그래픽의 풀컬러 이미지의 구성요소 


왜 하필 R(red), G(green), B(blue) 일까?
>사람 눈의 신경요소가 RGB에 반응하기 때문


 A(alpha)란?
>RGB만으로는 투명도 표현 X, A(alpha)를 통해 투명도라는 개념을 넣어준 것

Linear Workflow 
-------------
Gamma
> (화면 이미지의) 밝기의 곡선


>><그림1*>![image](https://user-images.githubusercontent.com/113420816/192740945-a14ade35-b597-4710-86bf-69382c055ce9.png)


 CRT 모니터에서는 실제 Linaer을 표준으로 작업한 이미지의 감마가 나오지 않음
> 따라서, Gamma를 더 높게 잡아 작업해(역함수) linear를 맞춤


>>(ex) <그림2**>![image](https://user-images.githubusercontent.com/113420816/192751345-412c4447-45ef-4a70-bd20-9855017b4057.png)



> 눈이 인식할 수 있는 함수 곡선과 디지털 기기를 통해 보이는 이미지의 함수 곡선에 차이가 남, 따라서 이를 맞춰주는 작업이 필수로 필요함
>> <그림3>![image](https://user-images.githubusercontent.com/113420816/192751030-3c58fb7b-3447-4ea6-8608-874f1813c28b.png)


Color Management
-------------
모두가, 어디에서, 어떤 디바이스를 이용해 이미지를 보더라도 다 같은 이미지를 보게하는 것


> OCIO (Open Color Input Output) = 컴퓨터 이미지와 비주얼 이펙트에 초점이 맞춰진 통일된 컬러 매니지먼트 공간 (*** a complete color management solution geared towards motion picture production with an emphasis on visual effects and computer animation)

> 요즘에는 촬영할 수 있는 기기도, 송출할 수 있는 디스플레이의 종류도 다양해졌음으로, 그에 맞춰서 Gamma 작업을 해줘야 할 필요가 있음 > 통일된 컬러 스페이스와 통일된 작업 공간이 필요하기 시작

> ACES
>> 기준이 되는 컬러 스페이스
>> 디스플레이가 표현할 수 있는 컬러 스페이스와 촬영본이 표현할 수 있는 컬러 스페이스가 다름 > ACES 라는 공통된 컬러 스페이스로 작업 후, ACES CG로 합성 작업


>>> AP0 = 미래 디바이스까지 고려한 가장 넓은 범위의 ACES 컬러 스페이스
>>> AP1 = 현재 가장 많이 사용하는 원본 소실의 최소화된 컬러 스페이스

Transfer fuction
-------------
이미지 캡쳐 장치 (촬영장치)의 RGB값과 카메라 노출도 색공간 속의 전자 신호값의 매핑값

><그림3****> ![image](https://user-images.githubusercontent.com/113420816/192979775-57f45940-e122-4546-838e-e220bd2cfef2.png)

>> 



LUT (Look Up Table)
-------------
 광도에 따라 신호값을 리매핑하는 작업, 색상 변환 과정의 일부
> 두가지 유형으로 나뉜다 
> 1. 1D LUT 2. 3D LUT


>1D LUT
>> 루미너스 (밝기의 x,y 값만 조절)


>3D LUT
>> 3가지 채널 (RGB)를 각각 조절


-------------
<참고 자료>  
*,** https://www.japanistry.com/understanding-gamma-in-photography/  
*** https://opencolorio.readthedocs.io/en/latest/concepts/overview/overview.html 
**** https://learn.foundry.com/course/5515/play/color-management-fundamentals-aces-workflows-in-nuke  

