
Week 02
=============

Colorspace
-------------
> R/G/B/A
>>컴퓨터 그래픽의 풀컬러 이미지의 구성요소 


>왜 하필 R(red), G(green), B(blue) 일까?
>>사람 눈의 신경요소가 RGB에 반응하기 때문


> A(alpha)란?
>>RGB만으로는 투명도 표현 X, A(alpha)를 통해 투명도라는 개념을 넣어준 것

Linear Workflow 
-------------
>Gamma
>> (화면 이미지의) 밝기의 곡선


>><그림1>![image](https://user-images.githubusercontent.com/113420816/192740945-a14ade35-b597-4710-86bf-69382c055ce9.png)


> CRT 모니터에서는 실제 Linaer을 표준으로 작업한 이미지의 감마가 나오지 않음
>> 따라서, Gamma를 더 높게 잡아 작업해(역함수) linear를 맞춤


>>(ex) <그림2>![image](https://user-images.githubusercontent.com/113420816/192751345-412c4447-45ef-4a70-bd20-9855017b4057.png)



> 눈이 인식할 수 있는 함수 곡선과 디지털 기기를 통해 보이는 이미지의 함수 곡선에 차이가 남, 따라서 이를 맞춰주는 작업이 필수로 필요함
>> <그림3>![image](https://user-images.githubusercontent.com/113420816/192751030-3c58fb7b-3447-4ea6-8608-874f1813c28b.png)


Color Management
-------------
> 
