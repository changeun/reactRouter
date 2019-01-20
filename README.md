이 프로젝트는 react-router로 SPA 개발하는 방법을 기록한 것입니다.(/w. [Create React App](https://github.com/facebook/create-react-app))

### `SPA란?`

Single Page Application, 즉 싱글 페이지 애플리케이션 약어.<br>


### `NODE_PATH 설정`

컴포넌트나 모듈을 import할 때 보통 상대 경로로 불러옴.<br>
디렉토리 구조가 깊어질 수록 '../../../../components/MyComponent' 식으로 불러오는 단점을 보완하여<br>
프로젝트의 루트 경로를 지정하여 절대 경로로 불러오는 방법 설정함.<br>

=> package.js 안에 있는 start와 bulid 부분 수정<br>
=> "start": "NODE_PATH=src (...)",<br>
   "bulid": "NODE_PATH=src (...)",<br>
   
   windows는 yarn add cross-env 따로 설치해주어야함. <br>
   "start": "cross-env NODE_PATH=src (...)",<br>
   "bulid": "cross-env NODE_PATH=src (...)",
