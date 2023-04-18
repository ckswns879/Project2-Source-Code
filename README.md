# 선용품 최적 구매발주 예측 분석 웹서비스

### Project
- 2023.02.09 ~ 2023.03.09
- [Github](https://github.com/K-Digital-4Wheel)
- url : http://3.37.27.133:3000/


### :art:개요
-  부산항에 입항 예정인 선박의 기자재들의 lead time을 예측하여 사전 발주 최적 Scheduling에 의한 선박 정비 관리의 비용 시간 절감하는 프로젝트이다.

### 기획 배경(프로젝트가 해결하려고 하는 문제)
- 선박에 사용되는 기자재 수는 선박 종류의 차이를 감안하더라도 약 900여종으로 추진기를 포함 할 경우 선박 가격의 50% 내외를 차지한다. 이러한 기자재가 발주된 시점부터 입고된 시점까지의 리드타임은 해당 기자재의 제조기간과 물류 운송기간 등의 변수에 영향을 받는다. 
- 선박 기자재의 기존 발주 내용과 입고 시간을 분석하여 기자재별 lead time을 예측하는 서비스를 개발하여 최적의 발주 scheduling으로 선박 관리의 비용과 시간을 단축하는 것을 목표로 한다.

### 프로젝트 목표(프로젝트가 미칠 영향)
-  선박의 수만가지 기자재들을 범주(category)로 자동 분류하여 해당 발주처에 발주하기 위한 범주 분류 학습 모델을 개발한다. 선박 기자재들의 범주를 자동 분류하는 서비스를 웹서비스로 구현한다.
- 선박 기자재별로 lead time을 과거 기자재의 발주 및 입고 데이터를 학습하여 예측한다. 선박으로부터 접수된 기자재 주문 품목별로 lead time을 예측하여 웹서비스로 제공하며 최적 발주 스케쥴링에 활용한다.

### 서비스 특징
- 선용품을 검색하고 발주할 수 있다.
- 여러 품목을 묶음 발주할 수 있다.
- 과거 리드타임 변화와 예측 리드타임을 볼 수 있다.
- 

--- 
</br>

## :memo:차례  
1. [팀원 소개]
2. [주요 기술 스택] :hammer:
3. [ERD] :wrench:
4. [서비스 소개] :package:
5. [규칙] :bulb:
6. [시작하기] :tada:

</br></br>
### 1. [팀원 소개]
--- 

- **박경관**  - Data_Analysis - https://github.com/kyunggwan  
- **금민경** - Data_Analysis - https://github.com/min0312  
- **강정효** - Front_end - https://github.com/slows14tem  
- **김찬준** - back_end - https://github.com/ckswns879  

</br></br>
### 2. [주요 기술 스택]:hammer:

--- 
- FrontEnd
<img src="https://img.shields.io/badge/ Figma-F24E1E?style=flat-square&logo=Figma&logoColor=ffffff" /> <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=React&logoColor=ffffff"/> 

- BackEnd
<img src="https://img.shields.io/badge/Spring Boot-6DB33F?style=flat-square&logo=SpringBoot&logoColor=ffffff" /> <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=MySQL&logoColor=ffffff" /> <img src="https://img.shields.io/badge/Amazon S3-569A31?style=flat-square&logo=Amazon S3&logoColor=ffffff" /> <img src="https://img.shields.io/badge/Amazon RDS-527FFF?style=flat-square&logo=Amazon RDS&logoColor=ffffff" /> <img src="https://img.shields.io/badge/Amazon EC2-FF9900?style=flat-square&logo=Amazon EC2&logoColor=ffffff" />

- Collaboration Tools
 <img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=GitHub" />  <img src="https://img.shields.io/badge/Miro-yellow?style=flat-square&logo=Miro&logoColor=000000" /> <img src="https://img.shields.io/badge/ Google Sheets-34A853?style=flat-square&logo=Google Sheets&logoColor=ffffff" /> 
</br></br>

### 3. [ERD] :wrench:
--- 
![ERD](https://user-images.githubusercontent.com/113881846/218421285-ea00b0e1-8270-44b8-b012-99c15590556b.png)
</br></br>
### 4. [서비스 소개] :package:
--- 
##### FrontEnd 주요 버전
```cmd
프론트엔드 주요 버전
1. react : 18.2.0
2. next : 12.3.1
3. axios: 0.27.2
4. Visual Studio : 1.71.0

```

#### BackEnd 주요 버전
```cmd
1. JVM : 1.8.0_192
2. WAS : apache-tomcat-9.0.71
3. IntelliJ : IntelliJ IDEA 2021.3.2 (ultimate)
4. springBootVer : '3.0.1'
5. AWS RDS: 8.0.31
6. ubuntu: 20.04 LTS
7. JAVA: 11

```
</br></br>
### 5. [협업 규칙] :bulb:
---
1. 네이밍 규칙
- 클래스/컴포넌트/인터페이스/메소드 : PascalCase(파스칼 표기법)
- 오브젝트/함수/인스턴스/변수/파라미터 : camelCase(카멜 표기법)
</br></br>
2. Git Convention
- [태그: 제목] 형태이며 : 뒤에만 space가 있음을 유의한다.
- Feat: 새로운 기능 추가
- Fix: 버그 수정
- Docs: 문서 수정
- Style: 코드 포맷팅, 세미콜론 누락, 코드 변경이 없는 경우
- Refactor: 코드 리펙토링
- Chore: 빌드 업무 수정, 패키지 매니저 수정
- Design: 디자인 수정
- Remove: 파일 삭제
- Rename: 파일명 변경
</br></br>
3. Git Commit 예시
```cmd
- Docs: README추가
- Remove: 명세서 파일 삭제
- Feat: 간단한 필터 적용
- Refactor: upgrade gradle version to 5.2.1
- Rename: 파일명 변경
```

### 6. [시작하기] :tada:
--- 
```cmd
# /backend/
$ java -jar project.jar

# /frontend/
$ npm install
$ npm start
```
</br></br>
