# transform_practice

패스트 캠퍼스 front-end 강의 중 transform 속성에 대한 공부

### ⭐️ translate() 의 소괄호 () 은 인자, 인수라고 부른다.

### transform 변화 효과의 확인을 명확히 하기 위해 body에 padding을 주었다.

### 불투명도 opercity : 0~1 ;


    원래의 형태
   ![스크린샷 2021-11-11 오후 12 08 04](https://user-images.githubusercontent.com/88579497/141236866-2b30d097-d2ed-43bd-8aba-798a642854a5.png)
    transform: rotate(45deg)를 준 값
  ![스크린샷 2021-11-11 오후 12 08 20](https://user-images.githubusercontent.com/88579497/141236891-a089179e-cf37-49c3-9b6b-a1864979a363.png)
  
    transform: rotate(45deg) scale(1.3), scale로 요소의 크기가 1.3배 늘어남
  ![스크린샷 2021-11-11 오후 12 16 09](https://user-images.githubusercontent.com/88579497/141236914-99d3fa87-bcc2-475c-9fdf-cac688ddf02e.png)


### transform에 함수를 넣으면 변환 효과를 줄수 있다.

    요소의 변환 효과
      - transform: 변환함수1 변환함수2 변환함수3 ...;
    변환 함수의 종류
      - transform: 원근법 이동 크기 회전 기울임;

### 2D 변환 함수

    px
    	- translate(x,y) : x,y축으로 이동
    	- translateX(x)	: x축으로 이동
    	- translateY(y) : y축으로 이동
    	- scale(x,y) : x,y축으로 이동
    deg
    	- rotate(degree) : 회전(각도)
    	- skewX(x) : x축으로 기울임
    	- skewY(y) : y축으로 기울임

### 3D 변환 함수

    px
    	- perspective(n) : 원근법(거리)
    deg
    	- rotateX(x) : 회전(x축)
    	- rotateY(y) : 회전(y축)

### translate(40px,40px);

    원본을 기준으로 x축으로 40, y축으로 40
  ![스크린샷 2021-11-11 오후 12 35 49](https://user-images.githubusercontent.com/88579497/141236970-6114b6a0-79b0-46f0-b35f-5cafdfa5ea30.png)
  	

### trnaslateX(40px);

    원본을 기준으로 x축으로 40
 ![스크린샷 2021-11-11 오후 12 37 10](https://user-images.githubusercontent.com/88579497/141236992-0f82d6f0-d941-472e-ae3a-3e877a47b0a9.png)


### translateY(40px);

    원본을 기준으로 y축으로 40
  ![스크린샷 2021-11-11 오후 12 38 46](https://user-images.githubusercontent.com/88579497/141237010-09a57414-dbf3-428f-9a9d-0d5dc861cc7b.png)
  	

### scale(1.5);
    AB 네모의 크기를 1.5배 키운다
 ![스크린샷 2021-11-11 오후 12 42 50](https://user-images.githubusercontent.com/88579497/141237052-3c01802c-1f60-43b7-9f58-73e0bb6e5ad8.png)


### scale(0.7);

    기본값이 1이다.
    AB 네모의 크기를 0.7배 약 70%의 크기로 줄인다
  ![스크린샷 2021-11-11 오후 12 46 51](https://user-images.githubusercontent.com/88579497/141237088-86bebd92-4113-46e1-b16e-7bbd74357215.png)
  
    

### scaleX(2)

  ![스크린샷 2021-11-11 오후 12 47 05](https://user-images.githubusercontent.com/88579497/141237100-c261ca27-cce3-4e44-b81e-ebf67869c97a.png)
 

### rotate(180deg);

    요소의 정 가운데 기준으로 180도 회전 시킨다.

![스크린샷 2021-11-11 오후 1 00 18](https://user-images.githubusercontent.com/88579497/141237144-ca32bce2-c16f-447d-a576-cfeb7e530050.png)
    	

### rotateX(45deg) : 3D 변환 함수 ;

    원근법을 사용해야 3d 같이 보이게 된다
    x 축을 기준으로 3차원으로 회전
    
![스크린샷 2021-11-11 오후 1 05 53](https://user-images.githubusercontent.com/88579497/141237176-deffb40c-1a38-46d2-8c2b-40d195d70a56.png)
  

### rotateY(45deg) : 3D 변환 함수 ;

    원근법을 사용해야 3d 같이 보이게 된다.
    y 축을 기준으로 3차원으로 회전
    
![스크린샷 2021-11-11 오후 1 34 53](https://user-images.githubusercontent.com/88579497/141237773-73ab54c4-7149-41ec-9583-9b6873f9f9f1.png)

  

### 원근법을 사용하여 3D같이 보이게 해보자 (원근법 함수는 제일 앞에 작성해야 한다)

    - perspective(500px) rotateX(70deg);
    
  ![스크린샷 2021-11-11 오후 1 09 36](https://user-images.githubusercontent.com/88579497/141237183-ca2e088f-bab7-4ede-8802-f7ec3b474124.png)

    - perspective(500px) rotateY(70deg);
    
  ![스크린샷 2021-11-11 오후 1 10 36](https://user-images.githubusercontent.com/88579497/141237192-28e41a8a-c543-422c-afdb-e1edff36e3d4.png)
 

    - perspective(500px) rotateX(30deg) rotateY(70deg);
  ![스크린샷 2021-11-11 오후 1 11 42](https://user-images.githubusercontent.com/88579497/141237443-8f48aee5-51df-486a-a523-3e4add249483.png)


   

### skewX, skewY;
![스크린샷 2021-11-11 오후 1 18 59](https://user-images.githubusercontent.com/88579497/141237376-2edda1ad-eb66-46c2-b7c4-6b0d8c24bbb8.png)

![스크린샷 2021-11-11 오후 1 19 08](https://user-images.githubusercontent.com/88579497/141237234-96e97891-a5e1-445d-ab5d-3a56b118751b.png)

![스크린샷 2021-11-11 오후 1 19 37](https://user-images.githubusercontent.com/88579497/141237240-e02cdd6b-698b-4f20-aa5e-84d78c7f5e61.png)




