# computer7

# CRA로 프로젝트 시작하기

- **Nods.js, npm install**
    
    [Download | Node.js](https://nodejs.org/en/download/)
    
    - **Node.js :** JavaScript로 네트워크 애플리케이션을 개발할 수 있게 해주는 환경
    - **npm(node package manager) :** Node.js를 위한 패키지 매니저
    - **패키지 매니저** : 프로젝트에서 필요로 하는 다양한 외부 패키지들의 버전과 의존성을 관리하고 편하게 설치 및 삭제를 도와주는 역할
    - Node.js를 설치하면 npm은 자동으로 함께 설치된다.
    
    - Node.js 버전 확인
    
    ```jsx
    node --version
    ```
    
    - npm 버전 확인
    
    ```jsx
    npm --version
    ```
    
- **Create-react-app**
    
    **CRA(Create-react-app)** 
    
    - 리액트로 웹 사이트를 개발할 때 create-react-app을 사용한다 ⇒  리액트로 웹 애플리케이션을 개발하는데 필요한 상태로 프로젝트를 생성해 주는 도구
    - CRA를 실행하기 위해서는 node.js, npm이 필요함!
    
    ```jsx
    npx create-react-app 프로젝트명
    ```
    
    - 리액트 기반 웹 애플리케이션을 생성하는 명령어
    - npx는 npm패키지를 설치하고 바로 실행 시켜준다.
        
         ⇒ 패키지를 정해진 위치에 설치하고 찾아서 실행하려면 번거롭기 때문에 한 번에 처리하기 위해서 npx 사용
        
    
    ***프로젝트 생성시 주의사항***
    
    1. 프로젝트명에 npm명령어를 사용하면 안 된다.
    2. 대소문자, 특수기호 사용 X
    
    ![화면 캡처 2023-02-20 094018.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b6190691-95f0-432f-89f3-a96e71310ab6/%ED%99%94%EB%A9%B4_%EC%BA%A1%EC%B2%98_2023-02-20_094018.png)
    
    설치완료시 화면
    
    ```jsx
    cd 해당폴더
    npm start
    ```
    
     Change Directory `cd`
    
    : 현재 커맨드 라인 도구가 위치한 경로를 변경하는 명령어 (폴더를 더블클릭해서 안으로 들어가는 것과 동일)
    
    ![화면 캡처 2023-02-20 094211.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/972f3049-e53b-42ee-b112-750a79a6834d/%ED%99%94%EB%A9%B4_%EC%BA%A1%EC%B2%98_2023-02-20_094211.png)
    
    리액트 애플리케이션 로컬 개발 환경에서 실행!
    
    ### 생성된 폴더 설명
    
    1. **node_modules**
        
        **: 프로젝트 생성에 필요한 모든 라이브러리 코드 보관함 /** 리액트 프로젝트를 위해 필요한 자바스크립트 라이브러리(모듈)이 자동 설치된 폴더 / node-package를 통해 설치된 모든 것들이 이 경로로 들어간다고 보면 된다.
        
    2. **public**
        
        **: html, img 파일 등을 보관하는 static 파일 보관함 /** 리액트로 개발한 모든 코드는 자바스크립트로 만들어진다. 
        
        manifest(file) : Favicon에 관련된 정보
        
    3. **src** 
        
        **: 소스 코드 보관함 /** 실제 리액트 코드를 개발하는 곳
        
        package.json : **프로젝트 정보 기입하는 파일** / 리액트 프로젝트 구동에 필요한 여러가지 라이브러리 정보들이 기입되어 있음(자동 생성되는 파일) - 평소에 건들 필요 없음
        

- 리액트라고 엄청나게 어렵고 복잡한게 아님! 기존 html,  css처럼 코드 짜서 웹 페이지 제작하면 되는데, html 대신 **JSX**라는 걸 사용한다. 처음엔 html과 다른 부분들 때문에 어색하게 느껴지는데, 사용하다보면 금방 익숙해지니까 걱정 노노!

- App.js가 메인페이지

**mac**

```jsx
sudo npx create-react-app 프로젝트명
```

맥북 비밀번호 입력

작업 폴더 오픈 → src → app.js에 코드 작성(메인 페이지)

미리 보기 띄우기 : terminal open → npm start

- **브라우저 설정 방법**
    
    **제어판 > 프로그램 > 기본 프로그램 > 기본 프로그램 설정**에 들어가서 Chrome 선택
    

html파일에 직접 리액트를 설치해도 되지만, 복잡하고 오래 걸려서 Create React App이라는 라이브러리 도움을 받아 프로젝트를 생성한다.

- **React에서 Emmet 설정**
    1. include Languages검색
    2. Item : javascript / value : javascriptreact 추가
        
        ![화면 캡처 2023-02-15 151848.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ca20157d-eb5f-42a9-ae37-b3996a1fdfcf/%ED%99%94%EB%A9%B4_%EC%BA%A1%EC%B2%98_2023-02-15_151848.png)
        
        ![화면 캡처 2023-02-15 152040.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c88d8d58-3c06-4902-a077-1ea878d84549/%ED%99%94%EB%A9%B4_%EC%BA%A1%EC%B2%98_2023-02-15_152040.png)
