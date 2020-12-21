### analysis_of_petitions_about_animal

데이터 분석 프로젝트
======================
## 청와대 국민청원 반려동물 카테고리 분석
-----------------------------------------
#### 중국언어문화전공 201803274 정소진

#### 1. 배경

2020년 대한민국은 반려동물 1000만 시대로, 올바른 반려문화와 동물권에 대한 관심이 점점 더 높아지고 있다. 과거에는 반려동물을 그저 집에서 키우는 '동물' 로 인식했으나 근래에는 하나의 '가족 구성원' 으로 대하는 가정이 급격하게 늘어났다. 실제로 우리나라에는 동물을 적절하게 보호 및 관리하고 동물의 생명보호, 안정보장 및 복지 증진을 꾀하며 동물의 생명 존중 등 국민의 정서를 함양하기 위한 목적으로 규정된 '동물 보호법이 존재한다.
그러나 동물권에 관심이 있는 사람들은 여기서 멈추지 않고, 계속해서 인식 변화에 힘쓰고 법률 개정을 촉구하고 있다.

#### 2. 연구 목적

그렇다면 사람들이 현재 반려동물 문화를 어떻게 인식하고 있고 어떤 부분에서 개선 노력을 지속하고 있는지 알아볼 필요가 있다.
이를 분석하기 위해 청와대 국민청원을 대상으로 데이터 분석을 진행하였다.

청와대 국민청원 게시판이란 청와대국민청원 게시판이란 2017년 문재인 대통령 취임 100일을 맞아 새로 개설된 게시판으로 대한민국 국민이라면 누구나 자유롭게 직접 게시글을 올릴 수 있고 다른 게시글에 동의하는 것 또한 가능하다. 청원글이 공개된 날짜로부터 30일 이내, 20명 이상 동의를 받을 경우 정부 및 청와대 관계자(각 부처 장관, 대통령 수석 비서관 등)이 직접 답변을 하는 시스템으로 운영된다.

이 국민청원 게시판은 정치개혁, 외교/통일/국방, 일자리, 미래, 성장동력, 농산어촌, 보건복지, 육아/교육, 안전/환경, 저출산/고령화대책, 행정, 반려동물, 교통/건축/국토, 경제민주화, 인권/성평등, 문화/예술/체육/언론, 기타 등 17가지 카테고리로 분류되어 있다.

본 프로젝트에서는 청와대 국민청원 반려동물 카테고리를 분석하여 다음과 같은 내용을 탐구했다.

* 한국의 동물 관련 문제와 동향을 파악

* 정부가 취해야 할 올바른 정책성 방향성

#### 3. 대상 데이터

분석 대상은 청와대 국민청원 반려동물 카테고리에 올라온 전체 게시글이며, 
연구 초반에 반려동물 카테고리만의 특성을 파악하기 위하여 정치개혁 카테고리 게시글도 분석에 함께 사용하였다. 
데이터는 모두 정제화 과정을 거쳤으며, 이를 마친 후의 반려동물 카테고리 게시글 데이터 개수는 총 4,461개이다.

#### 4. 방법

청와대 국민청원 반려동물 카테고리 게시글을 필요에 따라 
제목 혹은 글 내용으로 나누어 언어분석 (형태소 분석) 을 시행하였다.
추가로 단어시각화 ∙ 피벗테이블 분석 방법을 이용하여 데이터 해석을 진행했다.

#### 5. 해석

*(1) 반려동물 카테고리만의 특성 파악*

변별력 있는 비교 분석을 위하여 정치개혁 카테고리를 선택하여 반려동물 카테고리와 비교를 진행했다.

정치개혁 카테고리는 정제 후 반려동물 카테고리보다 약 15배 가량 많은 수의 67,811개의 청원 게시글 수를 기록했다. 
또 정치개혁 카테고리는 전체 카테고리 중 가장 많은 글이 올라오는 분야이다. 

이를 통해 대조점을 좀 더 명확히 하여 비교 분석하는 것이 가능하다고 판단되어, 각각의 제목을 형태소 분석을 시행했다.

<시각화>

![시각화_반려동물 동사](https://user-images.githubusercontent.com/74248362/102816792-ee6a2a80-4411-11eb-9d93-21ab2d23abc9.PNG)
