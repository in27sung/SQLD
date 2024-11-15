# SQLD


## 목차
### 과목 1 데이터 모델링의 이해 
##### 제1장 데이터 모델링의 이해
##### [제1절 데이터 모델링의 이해](#제1절-데이터-모델링의-이해-1)
##### [제2절 엔터티(Entity)](#2-데이터-모델의-기본-개념의-이해)
##### 제3절 속성(Attribute) 
##### 제4절 관계(Relationship) 
##### 제5절 식별자

<img width="999" alt="Screenshot 2024-11-11 at 7 09 09 pm" src="https://github.com/user-attachments/assets/ee8e7f0f-4cd1-4110-9875-b805b36e0851">
<img width="999" alt="Screenshot 2024-11-11 at 7 09 37 pm" src="https://github.com/user-attachments/assets/29432faf-6761-4651-a598-430aa9b017bd">
<img width="999" alt="Screenshot 2024-11-11 at 7 10 16 pm" src="https://github.com/user-attachments/assets/71b9626e-c400-44f8-869c-20ae8b643ac0">


# 제1절 데이터 모델링의 이해

## 1.모델링의 이해 

### 가. 모델링의 정의 
- 현실세계를 추상화, 단순화, 명확화하기 위해 일저한 표기법(Notation)에 의해 표현하는 기법 
- 다양한 형상에 대해서 일정한 표기법에 의해 표현해 놓은 모형
1) 복잡한 '현실세계'를 단순화시켜 표현하는 것이다.
2) 모델이란 사물 또는 사건에 관한 양상(Aspect)이나 관점(PErspeactive)을 연관된 사람이나 그룹을 위하여 명학화게 하는 것이다.
3) 모델이란 현실 세계의 추상화된 반영이다.

### 나. 모델링의 특징
1. 추상화(모형화): 현실세계를 일정한 형식에 맞추어 표현 즉, 다양한 현상을 일정한 양식인 표기법에 의해 표현
2. 단순화: 복잡한 현실세계를 약속된 규약에 의해 제한된 표기법이나 언어로 표현하여 쉽게 이해할 수 있또록 하는 개념
3. 명확화: 누구나 이해하기 쉽게 하기위해 대상에 대한 애매모호함을 제거하고 정확하게 현상을 기술

### 다. 모델링의 세 가지 관점 

<img width="999" alt="Screenshot 2024-11-11 at 7 32 36 pm" src="https://github.com/user-attachments/assets/798c76d5-4746-44e7-aab2-ff0edb88b365">

1. 데이터관점: 업무가 어던 데이터와 고나련이 있는지 또는 데이터간의 고나계가 무엇인지에 대해서 모델링하는 방법(What, Data)
2. 프로세스관점: 업무가 실제하고 있는 일은 무엇인지 또는 무엇을 해야 하는지를 모델링하는 방법(How, Process)
3. 데이터와 프로세스의 상관관점: 업무가 처리하는 ㅣㅇㄹ의 방법에 따라 데이터는 어떻게 영향을 받고 있는지 모델링하는 방법(Interaction)

## 2. 데이터 모델의 기본 개념의 이해 
### 가. 모델링의 정의 
* 정보시스템을 구축하기 위해, 해당 업무에 어떤 데이터가 존재하는지 또는 업무가 필요로 하는 정보는 무엇인지를 분석하는 방법
* 기업 업무에 대한 종합적인 이해를 바탕으로 데이터에 존재하는 업무 규칙(Business Rule)에 대하여 참(True) 또는 거짓(False)을 판별할 수 있는 사실(사실명제)을 데이터에 접근하는 방법(How),
  사람(Who), 전산화와는 별개의(똑립적인) 관점에서 이를 명확하게 표현하는 추상화 기법

#### 데이터 모델링의 목적
  1. 업무정보를 구성하는 기초가 되는 정보들을 일정한 표기법에 의해 표현함으로써 정보시스템 구축의 대상이 되는 업무 ㅐㄴ용을 정확하게 분석하는 것
  2. 분석된 모델을 가지고 실제 데이터베이스를 생성하여 개발 및 데이터관리에 사용하기 위한 것
     즉, 데이터 모델링이라는 것은 단지 데이터베이스만을 구축하기 위한 용도로만 쓰이는 것이 아니라 데이터 모델링 자체로서 업무를 설명하고 분석하는 부분에도 매우 중요한 의미를 가지고 있다.
     
<img width="999" alt="image" src="https://github.com/user-attachments/assets/8daadcfe-ceef-48e5-81aa-56f4831be8d8">

### 나. 데이터 모델이 제공하는 기능 
* 시스템을 현재 또는 원하는 모습으로 가시화하도록 도와준다.
* 시스템의 구조와 행동을 명세화 할 수 있게 한다.
* 시스템을 구축하는 구조화된 틀을 제공한다.
* 시스템을 구축하는 과정에서 결정한 것을 문서화한다.
* 다양한 영역에 집중하기 위해 다른 영역의 세부 사항을 숨기는 다양한 관점을 제공한다.
* 특정 목표에 따라 구체화된 상세 수준의 표현방법을 제공한다.

## 3. 데이터 모델링의 중요성 및 유의점 
#### 데이터 모델링의 중요성 
가. 파급효과(Leverage)
나. 복잡한 정보 요구사항의 간결한 표현(Conciseness)
다. 데이터 품질(Data Quality)

#### 데이터 모델링의 유의점 
1. 중복(Duplication)
2. 비유연성(Inflexibility)
3. 비일관성(Inconsistency)

## 4. 데이터 모델링의 3단계 진행 
가. 개념적 데이터 모델링(Conceptual Data Modeling)
나. 논리적 데이터 모델링(Logical Data Modeling)
다. 물리적 데이터 모델링(Physical Data Modeling)

### 제2절 엔터티(Entity)
