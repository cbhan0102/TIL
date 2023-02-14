글꼴(폰트)를 적용해보자
Web Fonts(프리텐다드 = 고딕체)


        구글 검색창에 [ prependard github ] 검색 ->
        github.com 의 ' orioncactus/pretendard: ,,,  ' 라고 적혀있는 링크페이지 이동

        <title>밑에
        <link rel="stylesheet" as="style" crossorigin href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard@v1.3.6/dist/web/variable/pretendardvariable-dynamic-subset.css" />
페이지에 폰트를 적용해본다.

그 다음에 css파일을 만들어주고, common(공통적인).css 파일을 만들어준다.
각각의 페이지에서 모두 사용될때 쓴다.(하나하나 해줄 필요 없음)

        body {
        font-family: "Pretendard Variable", sans-serif;
        }

다 적었으면 html에 연결해줘야한다.
        
        <link rel="stylesheet" href="./css/common.css">


주의: 우리가 폰트를 쓸 때엔 저작권에 매우 조심해야한다.
프리텐다드는 안심해서 써도 된다. 웹 폰트는 우리가 쓸 수 있는 일반적인 폰트랑 다른점이 있다.
폰트같은 경우 용량이 꽤 큰편이라 시간이 걸릴 수 있다. 가지고 오기 전까진 예쁜 폰트를 보일 수 없으니
때문에 대부분의 웹폰트는 '경량화'되어있다.

