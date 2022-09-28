Week 01
=============

2D
-------------
> What is 2D?
>>2D = 2차원 (two-dimensional space) , 2차원 컴퓨터 그래픽스 (2D computer graphic)
>>점과 점을 이은 선의 세계, X와 Y값으로 이루어진 세계
>>>1D, 3D, 4D란?
>>> 점, 점선면, 점선면도형. XYZ, XYZ에 시간선을 넣은 차원
>What is Dimension?
>> 차원..
>Then why we use 2D?
>> 결국 우리가 보는 영상물은 2D로 이루어져 있기 때문에

Digital
-------------
>Digit
>>숫자
>>> 이미지를 숫자화 할 수 있다. 컴퓨터는 0과 1로 이루어진 세계, 명도에 따라 0~255까지 분류가능
>>>

<그림1*>
![Image](https://user-images.githubusercontent.com/113420816/191705939-f829587a-d089-48d5-9269-291b70d495c5.png)
>>> 세가지 단계를 통해 이미지로 변화된다
>>>1. 공간 샘플링 2. 시간 샘플링 3. 픽셀 값의 양자화 - 이때 두 샘플링은 디지털 이미지를 제공하는 데이터가 되고, 이 저장한 데이터를 정수 값 범위로 변환하면 마지막과 같은 그림이 나타난다.


>>> 컬러 이미지도 같은 원리로 돌아간다.
>>>

<그림2**>
![Image](https://user-images.githubusercontent.com/113420816/191707073-abbff974-60be-410e-9c05-0b43718289be.png)

>>>RGB라는 세가지 색상 채널을 사용해 표현하는데, 세가지 채널들은 각 빨간, 녹색, 파랑의 강도에 따라 0~255의 단계를 가진다. 한 픽셀당 세가지의 채널 데이터를 가지고 색을 만들어 내는 것.

Compositing
-------------
>

Color
-------------
>Hue + Value + Saturation (색조+명도+채도)
>빛은 바깥에 존재하지만, 색은 인식하는 뇌 속에서만 이루어지는 것

>RGB
>>컴퓨터상으로 표현해낼 수 있는 컬러
>> 레드, 그린, 블루

>CMYK
>>인쇄 가능한 컬러
>>시안, 마젠타, 옐로, 블랙을 섞어 인쇄를 함

Alpha
-------------
>어도비에서는 투명도의 개념으로 사용
>우리가 흔히 아는 체커보드=알파

Colorspace
-------------
>Why does it matter?
>>표현할 수 있는 컬러 스페이스가 커질 수록 다양한 색감을 잡아냄, 표현하고자 하는 색감에 가까워질 수 있음

>요즈음은 Rec.2020을 사용해 영상물 제작후, 원하는 배포 기종..? (텔레비젼, 스크린, 유튜브 영상 등등)에 따라 컬러스페이스를 달리 해서 제공


<출처>
*, ** Mathanraj Sharma, "Understanding Images with skimage-Python", Medium, <https://towardsdatascience.com/understanding-images-with-skimage-python-b94d210afd23>

