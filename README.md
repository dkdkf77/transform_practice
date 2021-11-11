# transform_practice

패스트 캠퍼스 front-end 강의 중 transform 속성에 대한 공부

### ⭐️ translate() 의 소괄호 () 은 인자, 인수라고 부른다.

### transform 변화 효과의 확인을 명확히 하기 위해 body에 padding을 주었다.

    원래의 형태
    스크린샷
    transform: rotate(45deg)를 준 값
    스크린샷
    transform: rotate(45deg) scale(1.3), scale로 요소의 크기가 1.3배 늘어남
    스크린샷

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
    	스크린샷

### trnaslateX(40px);

    원본을 기준으로 x축으로 40
    	스크린샷

### translateY(40px);

    원본을 기준으로 y축으로 40
    	스크린샷

### scale(1.5);

    AB 네모의 크기를 1.5배 키운다

### scale(0.7);

    기본값이 1이다.
    AB 네모의 크기를 0.7배 약 70%의 크기로 줄인다

### scaleX(2)

    	스크린샷

### rotate(180deg);

    요소의 정 가운데 기준으로 180도 회전 시킨다.

    	스크린샷

### rotateX(45deg) : 3D 변환 함수 ;

    원근법을 사용해야 3d 같이 보이게 된다
    x 축을 기준으로 3차원으로 회전

### rotateY(45deg) : 3D 변환 함수 ;

    원근법을 사용해야 3d 같이 보이게 된다.
    y 축을 기준으로 3차원으로 회전

### 원근법을 사용하여 3D같이 보이게 해보자 (원근법 함수는 제일 앞에 작성해야 한다)

    - perspective(500px) rotateX(70deg);

    - perspective(500px) rotateY(70deg);

    - perspective(500px) rotateX(30deg) rotateY(70deg);

### skewX, skewY;
