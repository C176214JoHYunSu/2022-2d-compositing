
Week 11
=============

멈춰있는 소스 + 움직이는 영상 소스 > motion blur  

같은 색의 노드들을 함께 붙여둘 것 - 비슷한 연산>원본 손실이 적어짐 (특히 transform_필터有, 같이 묶어두고 작업)  

shuffle>원본 바로 아래 둘 것  
 

bounding box   
merge - union>b box   

alt + e - 연결된 초록색 선 정리  

postage stamp - 선 정리 노드  



2.5D
-------------
포토샵에서 레이어 분할 - 


conerpin
--------
> connerpin - set to input - from head - set to input - copy 'from' - 사이즈 맞춰짐   
> 맞춰진 후 connerpin 하나 더 사용 - 수동으로 위치 맞추기  
> 빠져나간 부분은 직접 트래킹  
> stablize>transform - invert   
> 작업한 노드의 역방향, 원본과 합치면 가만히 있는 것처럼 보임    

project 3d3
----------
> 2.5d, 이미지를 3d화 시키는 것  
> 투사할 2D 이미지를 projectioncam에 연결   
> card 로 정육면체 공간을 만들어주기 (3d 공간에서 확인하고 위치, 크기 조절, z값만 조절할 것)   
> card와 scene 연결 - cam - scanline render  
