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

#### <시각화>

![시각화_반려동물 동사](https://user-images.githubusercontent.com/74248362/102816792-ee6a2a80-4411-11eb-9d93-21ab2d23abc9.PNG)
~주세요 형태의 종결 어미 사용이 뚜렷하게 나타난다
---------------------------------------

![시각화_정치개혁 동사](https://user-images.githubusercontent.com/74248362/102816918-26716d80-4412-11eb-84c3-ccade3cc796b.PNG)

~주세요 형태의 종결 어미 사용이 뚜렷하게 나타나지는 않는다.
-----------------------
#### <피벗 테이블 분석>

좀 더 상세한 분석을 위해 동사만을 대상으로 피벗 테이블 분석을 시행

![그림1](https://user-images.githubusercontent.com/74248362/102817136-8831d780-4412-11eb-9231-5e9c5f16c7e8.png)

**반려동물** 카테고리는 호소하는 듯한 종결 어미를 많이 사용

**정치개혁** 카테고리는 좀 더 직설적이고 강한 어조의 요구하는 듯한 어투를 보임.

이를 종합해 보면 같은 국민청원임에도 반려동물 카테고리의 게시글이 좀 더 완곡하고 정중한 표현을 사용했다는 것을 알 수 있다. 국민청원이라는 글의 특성은 같으나 각각의 글쓰기 기법이 다르게 나타나는 이유는 무엇일까? 이것은 사회적 관심도와 연관이 있다. 
반려동물 카테고리는 청와대 국민청원 게시글 중 가장 수가 적고, 정치개혁은 가장 많은 수의 게시글이 올라온다.

이를 바탕으로 생각해 보면 직설적인 표현의 사용은 글을 읽는 데에 다소 거부감을 불러 일으킬 수 있기에 반려동물 관련
게시글이 좀 더 부드럽고 완곡한 표현을 통해 의견을 전달하고자 하고 있는 것이다.

**************************

*(2) 핵심 키워드를 중심으로 청원 게시글 소주제 분류*

#### <시각화>

![시각화_반려동물 명사](https://user-images.githubusercontent.com/74248362/102817574-5e2ce500-4413-11eb-8473-2f0eb9095c9e.PNG)


#### <피벗 테이블 분석>

![그림1](https://user-images.githubusercontent.com/74248362/102817613-7270e200-4413-11eb-9d0b-82fa466b4009.png)

반려동물 카테고리 게시글 제목에서 많이 사용된 유의미한 명사는 ‘강화’, ‘처벌’ , ‘법’, ‘동물보호법’, ‘금지’, ‘보호’, ‘동물학대’, ‘식용’, ‘학대’, 유기견’, ‘공장’, ‘개고기’, ‘개정’ 등이 있었다. 이를 통해 청원 내용의 주제와 핵심을 크게 6가지로 분류하였다.

+ 개농장

+ 도살

+ 동물학대

+ 반려문화

+ 유기동물

+ 의료


*(3)청원 게시글 내용 분석*

상세한 동향 파악을 위해 게시글의 청원 동의 수를 내림차순으로 정렬하고, 동의 수 기준 상위 180개 청원의 주제를 앞서 분류한 6가지 소주제로 나누어 보았다.

전체 180개중 각각의 소주제 비율는 다음과 같았다.

![캡처](https://user-images.githubusercontent.com/74248362/102818026-2ecaa800-4414-11eb-888e-4114ed55e065.PNG)

표에서 확인할 수 있는 바와 같이 상위 180개의 주제 비율은 동물학대가 45%로 1위.이어서 반려문화, 개농장, 유기동물, 도살, 의료 순. 
----------------------------

이렇게 새롭게 분류한 6가지 소주제를 중심으로 180개 게시글의 내용을 피벗 테이블 분석을 통해 자세히 해석해 보았다. 여기서도 동향과 중심 의견 파악이 목적이므로 다른 품사는 제외하고 핵심 키워드인 명사에 초점을 맞추어 진행했다.

## <동물학대>
![동물학대명사](https://user-images.githubusercontent.com/74248362/102818285-a8629600-4414-11eb-8163-c6cb4d95a595.png)

표본 중 가장 많은 비중을 차지한 동물학대 주제의 유의미한 키워드는 ‘학대’, ‘고양이’, ‘처벌’, ‘동물보호법’, ‘동물학대’ 등이었다.

-> 개 ∙ 고양이 포함 동물 학대 처벌 강화 / 동물 보호법 강화
================================
## <반려문화>

![반려문화명사](https://user-images.githubusercontent.com/74248362/102818438-f24b7c00-4414-11eb-9813-067196cd1901.png)

반려문화 주제는 올바른 반려문화 구축을 촉구하는 것을 중심 주제로 하며 여기서 유의미하게 분류되는 명사들은 다음과 같다. 먼저 주목해야 할 명사는 ‘사람’ 이다. 이 주제에서는 반려동물과 사람이 평화롭게 함께 살아갈 수 있는 사회를 만드는 것을 중요한 가치로 삼기 때문에 평균보다 ‘사람’ 명사의 상대빈도가 높게 나타난 것으로 보인다. 

반려문화 주제에서는 사람과 동물이 함께 살아가는 올바른 사회를 지향하며, 반려동물 문화가 발달됨에 따라 나타날 수 있는 문제나 쟁점(맹견에 의한 피해, 동물 실종을 방지할 수 있는 반려동물 등록 제도, 목줄 의무화, 입마개 의무화) 등을 제시하고 제도 개선을 촉구하고 있다.

=> 올바른 반려 문화 구축 / 관련 법 개정
=========================

## <개농장>

![개농장명사](https://user-images.githubusercontent.com/74248362/102818523-29ba2880-4415-11eb-87de-c508aac3059e.png)

이 주제의 정확한 핵심 내용은 개농장을 반대하는 것이다. 아직까지 우리나라 반려 문화에서 가장 심각하다고 꼽히고 있는 문제는 펫샵 분양과 개농장을 통한 인위적 교배이다. 실제로 여러 곳이 존재하며, 이 번식장에서는 품종견들을 가둬 둔 채 억지로 새끼를 낳게 하고 펫샵으로 유통시킨다. 번식장의 어미개들은 구조 받지 못하는 이상 평생 비위생적인 개농장에 갇혀서 죽을 때 까지 새끼만 낳아야 한다. 이렇게나 비윤리적이고 잔인한 구조는 지금도 계속되고 있으며, 그 속에서의 동물들의 희생은 불가피하다. 이러한 번식장의 현실은 매체에도 꾸준히 소개되었고 사람들의 관심 또한 높은 것으로 보인다. 

개농장의 목적을 설명하기 위해 이 주제에서는 ‘분양’ 이라는 단어를 많이 사용하였고, ‘불법’, ‘공장’, ‘번식’, ‘펫샵’ 등의 개농장 관련 단어도 많이 등장함을 알 수 있다. 

=> 개농장 ∙ 펫샵 반대 / 동물 보호법 강화
=======

## <유기동물>

![유기동물 명사](https://user-images.githubusercontent.com/74248362/102818626-5ec67b00-4415-11eb-9c8c-132211c231b7.png)

유기동물 카테고리에서는 다른 카테고리들과 다르게 ‘길고양이’라는 명사의 사용이 두드러진다. 또한 ‘생명’ , ‘보호’ 와 같은 단어를 사용하여 길고양이, 유기견을 포함한 유기동물을 보호하고 한 생명으로써 존중하자는 것을 핵심 내용으로 하고 있다.

=> 유기동물 생명 존중 / 생활에 적합한 보호소 환경 마련 / 동물 보호법 강화
====

## <도살

![도살명사](https://user-images.githubusercontent.com/74248362/102818683-7f8ed080-4415-11eb-98e4-45156364dbe0.png)

도살 분야에서는 말그대로 동물의 도살을 반대하고 개나 고양이가 식용으로 이용되는 것에 반발하고 있다. 이 주제의 게시글에서는 ‘고통’ 과 ‘동물보호’라는 단어의 사용이 두드러지는데, 다른 주제에 비해 식용 도살이 동물에게 주는 고통을 강조한 것으로 보이며 도살이 ‘동물보호’에 가장 큰 걸림돌로 작용한다는 것을 말하고 있다. 또한 특이한 점은 ‘가축’이라는 명사의 등장인데, 내용을 분석해 보니 비윤리적인 공장식 가축 사육과 이를 통한 도축 또한 강하게 반대하고 있음을 알 수 있었다. 

=> 개, 고양이 도살(식용) 반대 / 공장식 가축 사육 반대 / 동물 보호법 강화
========

## <의료> 

![의료 명사](https://user-images.githubusercontent.com/74248362/102818753-a3eaad00-4415-11eb-842b-0c6d026f8b3c.png)

마지막 주제인 ‘의료’ 분야에서는 당연하게도 ‘병원’ , ‘수의사’, ‘의사’ 등의 단어를 사용하여 동물병원의 의료 사고 진상 규명 혹은 수의사 자격에 대한 의문을 제기하고 있다. 또한 ‘대학교’ ‘교수’ 등의 표현을 통해 대학 의료 연구실에서 발생하는 비인간적인 동물 실험을 반대하고 사건 내용을 규명해야 한다고 말하는 청원이 다수 존재함을 파악할 수 있었다.

=> 의료법 개정 / 동물 실험 반대 / 동물 보호법 강화
=============
------------------------------------

*(4) 결론 및 정책 방향성 제시*

- 동물학대 :처벌 수위 강화, 동물 보호법 강화

- 반려문화 : 올바른 반려 문화 구축, 관련 법 제도 개선

- 개농장 : 개농장∙펫샵 폐지, 동물 보호법 강화

- 유기동물 : 유기동물 생명 존중, 적절한 보호소 설치, 동물 보호법 강화

- 도살 : 도살 반대, 공장식 가축 사육 반대, 동물 보호법 강화

- 의료 : 의료법 개선, 동물 실험 반대, 동물 보호법 강화

전체적인 문제를 관통하는 핵심 키워드 __'동물 보호법 강화' __

정부가 취해야할 앞으로의 정책 방향성

① 도살, 개농장, 유기동물, 동물학대 문제 등을 해결할 수 있는 동물 보호법 강화
===========
② 올바른 반려문화 구축을 위한 관련 법 제도 개선
==========






