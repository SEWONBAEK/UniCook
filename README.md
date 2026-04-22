# UniCook
<br/>

<div align="center">
  <img src="./img/logo.PNG" width="80%">
  <h3>자산의 시각화를 제공하는 인터넷 전문 은행</h3>
</div>

## ⌨️ 기간

- **2023.08.21 ~ 2023.10.06(7주)**

<a name="tableContents"></a>

<br/>

## 🔎 목차

1. <a href="#subject">🎯 주제</a>
1. <a href="#mainContents">⭐️ 주요 기능</a>
1. <a href="#systemArchitecture">⚙ 시스템 아키텍쳐</a>
1. <a href="#skills">🛠️ 기술 스택</a>
1. <a href="#erd">💾 ERD</a>
1. <a href="#contents">🖥️ 화면 소개</a>
1. <a href="#developers">👥 팀원 소개</a>

<br/>

<!------- 주제 시작 -------->

## 🎯 주제

<a name="subject"></a>

**finBall**은 돈을 시각적으로 보여주기 위해 공을 사용합니다. 

공을 통해 자신의 계좌 잔액을 볼 수 있으며, 공을 통한 재미있는 정산 방식인 **핀볼 정산**을 제공합니다.

**주요 기능**

- 모임 통장
- 가계부
- 금융 학습

<div align="right"><a href="#tableContents">목차로 이동</a></div>

<br/>

<!------- 주요 기능 시작 -------->

## ⭐️ 주요 기능

<a name="mainContents"></a>

### 모임 통장

<h4> 모임 통장을 만들 수 있으며, 핀볼 정산 서비스를 제공합니다.</h4>

- 상대방에게 문자 메시지를 통해, 모임 통장초대 링크를 보냅니다.
- 모임통장의 핀볼 정산은 정산 시 게임이 진행되며, 게임 결과에 따라 개인의 정산 금액이 결정됩니다.

---

### 가계부

<h4>finBall 계좌를 만들면 가계부를 생성할 수 있습니다.</h4>

- 목표 금액과 가계부로 관리할 항목을 입력하면 가계부 기능을 사용할 수 있습니다.
- 가계부는 핀볼 거래 내역에서 쉽게 작성 가능합니다.

---

### 금융 학습

<h4>ChatGPT를 이용하여 금융 학습 서비스를 제공합니다.</h4>

- 생성형 AI인 ChatGPT와 대화할 수 있는 공간을 제공합니다.
- ChatGPT에 금융 전문가의 역할을 부여했으며, 금융 지식을 전문적으로 답변을 제공합니다.

<div align="right"><a href="#tableContents">목차로 이동</a></div>

<br/>


<!------- 시스템 아키텍쳐 시작 -------->

## ⚙ 시스템 아키텍쳐

<a name="systemArchitecture"></a>

<img src="./img/architecture.png">

- FinBall 서버 : 핀볼 서비스 
- Mydata 서버 : 은행 공동망(대외계)

은행 업무를 위해 타행 관련 서비스를 위해 금융 시스템의 대외계 채널의 아키텍처를 활용했습니다. FinBall서버와 Mydata 서버간 통신을 통해 데이터 공유 및 결제 처리를 했습니다.

<div align="right"><a href="#tableContents">목차로 이동</a></div>

<br/>

<!------- 기술 스택 시작 -------->

## 🛠️ 기술 스택

<a name="skills"></a>

### 프론트

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![TypeScript](https://img.shields.io/badge/Typescript-3178C6?style=for-the-badge&logo=Typescript&logoColor=white)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)

![ChatGPT](https://img.shields.io/badge/chatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white)
![Redux](https://img.shields.io/badge/redux-%23593d88.svg?style=for-the-badge&logo=redux&logoColor=white)

![Figma](https://img.shields.io/badge/figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white)

---

### 백엔드

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![SpringBoot](https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)

![SpringBoot](https://img.shields.io/badge/springsecurity-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)

![Mysql](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mariadb&logoColor=white)
![MongoDB](https://img.shields.io/badge/mongoDB-47A248?style=for-the-badge&logo=MongoDB&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)

---

### 협업

![GitLab](https://img.shields.io/badge/gitlab-FC6D26.svg?style=for-the-badge&logo=gitlab&logoColor=white)
![Jira](https://img.shields.io/badge/jira-%230A0FFF.svg?style=for-the-badge&logo=jira&logoColor=white)
![Mattermost](https://img.shields.io/badge/mattermost-0058CC.svg?style=for-the-badge&logo=mattermost&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000.svg?style=for-the-badge&logo=notion&logoColor=white)

<div align="right"><a href="#tableContents">목차로 이동</a></div>

<br/>

<!------- ERD 시작 -------->

## 💾 ERD
### 핀볼 ERD
<img src="./img/erdFinball.png">

---
### 마이데이터 ERD
<img src="./img/erdMydata.png">

<a name="erd"></a>

<div align="right"><a href="#tableContents">목차로 이동</a></div>

<br/>

<!------- 화면 소개 시작 -------->

<a name="contents"></a>

<br/>

## 🖥️ 화면 소개

### 1. 핀볼 계좌

<table>
    <tr>
        <td align="center" width="200">
            <h5>핀볼 계좌 채우기</h5>
            <img src="./img/gifs/핀볼채우기.gif" alt="핀볼채우기" width="100%" />  
        </td>
        <td align="center" width="200">
            <h5>핀볼 계좌 이체</h5>
            <img src="./img/gifs/핀볼보내기.gif" alt="핀볼보내기" width="100%" />  
        </td> 
        <td align="center" width="200">
            <h5>가계부</h5>
            <img src="./img/gifs/가계부.gif" alt="가계부" width="100%" />
        </td>
    </tr>
    <tr>
      <td align="center">
        <div>✔ 핀볼 서비스에 등록된 계좌에서 입금</div>
      </td>
      <td align="center">
        <div>✔ 핀볼 계좌에서 다른 계좌로의 이체</div>
      </td>
      <td align="center">
        <div>✔ 가계부 생성 및 항목 지정</div>
        <div>✔ 거래 내역에서 항목 선택 시 가계부 반영</div>
      </td>
    </tr>
</table>

### 2. 모임 통장

<table>
    <tr>
        <td align="center" width="200">
            <h5>모임 계좌 생성</h5>
            <img src="./img/gifs/모임계좌생성.gif" alt="모임계좌생성" width="200" />  
        </td>
        <td align="center" width="200">
            <h5>모임 계좌 채우기</h5>
            <img src="./img/gifs/모임계좌채우기.gif" alt="모임계좌채우기" width="200" />  
        </td> 
        <td align="center" width="200">
            <h5>모임 계좌로 결제</h5>
            <img src="./img/gifs/모임계좌로결제.gif" alt="모임계좌로결제" width="200" />
        </td>
        <td align="center" width="200">
            <h5>간편 정산</h5>
            <img src="./img/gifs/간편정산.gif" alt="간편정산" width="200" />
        </td>
    </tr>
    <tr>
      <td align="center">
        <div>✔ 모임 계좌 생성 시 계좌 이름과 정산 방식 설정</div>
      </td>
      <td align="center">
        <div>✔ 모임 계좌의 채우기 버튼을 통해 채우기</div>
      </td>
      <td align="center">
        <div>✔ 핀볼 정산을 선택했을 시, 게임을 통해 정산 진행</div>
      </td>
      <td align="center">
        <div>✔ 모임 계좌가 없거나, 간편하게 정산을 하기 위한 서비스</div>
      </td>
    </tr>
</table>

### 3. 타행

<table>
    <tr>
        <td align="center" width="200">
            <h5>카드 연결</h5>
            <img src="./img/gifs/카드연결.gif" alt="카드연결" width="200" />  
        </td>
        <td align="center" width="200">
            <h5>카드 결제</h5>
            <img src="./img/gifs/카드결제.gif" alt="카드결제" width="200" />  
        </td> 
        <td align="center" width="200">
            <h5>계좌 연결</h5>
            <img src="./img/gifs/계좌연결.gif" alt="계좌연결" width="200" />
        </td>
        <td align="center" width="200">
            <h5>계좌 결제</h5>
            <img src="./img/gifs/계좌결제.gif" alt="계좌결제" width="200" />
        </td>
    </tr>
    <tr>
      <td align="center">
        <div>✔ 대외계 접근을 위해 주민번호 인증</div>
        <div>✔ 대외계 서버에 존재하는 카드 정보 조회 및 등록</div>  
      </td>
      <td align="center">
        <div>✔ 카드상세 페이지에서 카드 결제</div>
      </td>
      <td align="center">
        <div>✔ 대외계 접근을 위해 주민번호 인증</div>
        <div>✔ 대외계 서버에 존재하는 계좌 정보 조회 및 등록</div>
      </td>
      <td align="center">
        <div>✔ 대외계 서버에 있는 계좌로 결제</div>
      </td>
    </tr>
</table>

### 4. 금융 학습

<table>
    <tr>
        <td align="center" width="200">
            <h5>GPT 학습</h5>
            <img src="./img/gifs/GPT학습.gif" alt="GPT학습" width="200" />  
        </td>
        <td align="center" width="200">
            <h5>금융 퀴즈</h5>
            <img src="./img/gifs/금융퀴즈.gif" alt="금융퀴즈" width="200" />  
        </td> 
        <td align="center" width="200">
            <h5>계좌 연결</h5>
            <img src="./img/gifs/커스텀볼.gif" alt="커스텀볼" width="200" />
        </td>
    </tr>
    <tr>
      <td align="center">
        <div>✔ ChatGPT를 활용한 금융 학습</div>  
      </td>
      <td align="center">
        <div>✔ 금융 퀴즈로 포인트 획득</div>  
      </td>
      <td align="center">
        <div>✔ 획득한 포인트로 공 구매</div>
        <div>✔ 구매한 공 선택으로 스킨 적용</div>
      </td>
    </tr>
</table>

<div align="right"><a href="#tableContents">목차로 이동</a></div>

<br/>

### ✔ 프로젝트 결과물

---

<!-- - [포팅메뉴얼] -->

- [중간발표자료](./ppt/핀볼_중간발표.pptx)
- [최종발표자료](./ppt/핀볼_최종발표.pptx)
<!-- - [최종발표자료] -->

<!------- 팀원 소개 시작 -------->

## 👥 팀원 소개

<a name="developers"></a>

|  **Name**   |                                                  박윤희                                                   |                                                  박세연                                                   |                                                  박정희                                                   |                                                  백세원                                                   |                                                  진선용                                                   |                                                  정정원                                                   |
| :---------: | :-------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------: |
|  **역할**   |                                                  풀스택                                                   |                                                프론트엔드                                                 |                                                  프론트엔드                                                   |                                                풀스택                                                 |                                                  풀스택                                                   |                                                  프론트엔드                                                   |
<div align="right"><a href="#tableContents">목차로 이동</a></div>
