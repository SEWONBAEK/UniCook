# UniCook
<br/>

<div align="center">
  <img src="./img/logo.PNG" width="80%">
  <h3>자산의 시각화를 제공하는 인터넷 전문 은행</h3>
</div>

## ⌨️ 기간

- **2026.03.24 ~ 2026.04.27(5주)**

<a name="tableContents"></a>

<br/>

## 🔎 목차

1. <a href="#subject">🎯 주제</a>
1. <a href="#mainContents">⭐️ 주요 분석</a>
1. <a href="#systemArchitecture">⚙ 시스템 아키텍쳐</a>
1. <a href="#skills">🛠️ 기술 스택</a>
1. <a href="#erd">💾 ERD</a>
1. <a href="#contents">🖥️ 화면 소개</a>
1. <a href="#developers">👥 팀원 소개</a>

<br/>

<!------- 주제 시작 -------->

## 🎯 주제

<a name="subject"></a>

**빅데이터 분석**과 **AI**를 활용한 식품 커머스 프로젝트로 개인 맞춤형 추천 상품을 보여줍니다.<br />
각 페이지마다 다른 **알고리즘**을 이용하여 데이터를 분석합니다.

<br />
**주요 기능**


- **Numpy**, **Pandas**를 이용한 전처리
- **Scikit-learn(SVD)**, **협업 필터링**의 **코사인 유사도 분석** 이용
- 분석한 내용과 시간대별 추천과 아이템 카테고리 결합
  
<div align="right"><a href="#tableContents">목차로 이동</a></div>

<br/>

<!------- 주요 기능 시작 -------->

## ⭐️ 주요 분석

<a name="mainContents"></a>

### 메인 페이지

#### 메인 페이지 상단과 하단에 상품별 분석 내용을 제공합니다.

- 상단 분석
  - 회원 : 시간대별 분석 + 사용자 구매내역(SVD) + 아이템 카테고리를 결합하여 분석합니다.
  - 비회원 : 시간대별 가장 많은 구매내역을 가진 상품 4가지를 표시합니다.

- 하단 분석
  - 회원 : 로그인한 사용자와 같은 성별, 비슷한 나이대의 유사도를 통해 도출한 가중치를 아이템으로 도출했습니다.
  - 비회원 : 전체 회원을 대상으로 구매내역에 대한 가중치를 부여하여 분석 후 화면에 표시합니다.


===


### 상세 페이지

#### 현재 상품 기준의 분석 내용을 제공합니다.

- 현재 상품과 가장 유사도가 높은 상품들을 도출하여 화면에 표시합니다.


---


### 장바구니

<h4>장바구니에 담긴 상품과 전체 사용자의 구매내역을 통해 분석합니다.</h4>

- 장바구니에 담긴 상품들을 토대로 아이템 간 코사인 유사도를 계산합니다.
- 구매내역 + 구매수량(로그화)을 합산하여 유사도를 계산합니다.


---


### 구매내역

#### 현재 사용자가 지금까지 구매한 내용을 바탕으로 상품을 추천할 수 있도록 분석합니다.

- 현재 사용자가 구매한 상품의 구매빈도와 구매수량에 대한 가중치를 계산하여 최애 상품을 분석합니다.
- 가중치 점수: (빈도 * 0.7) + (수량 * 0.3)


---


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

### 💻 FrontEnd

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![Ajax](https://img.shields.io/badge/Ajax-%23ffffff.svg?style=for-the-badge&logo=jquery&logoColor=black)
![Figma](https://img.shields.io/badge/figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white)
---

### ⚙️ BackEnd

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Mysql](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mariadb&logoColor=white)
---

### 📊 Data Analysis

![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
---

### 📈 Visualization

![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Seaborn](https://img.shields.io/badge/Seaborn-%234479A1.svg?style=for-the-badge&logo=Seaborn&logoColor=white)
---

### 🤝 Collaboration

![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
---

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
