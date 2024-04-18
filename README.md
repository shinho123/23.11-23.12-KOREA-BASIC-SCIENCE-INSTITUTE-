# 23.08-23.12-KOREA-BASIC-SCIENCE-INSTITUTE-
기관 협업 공동 연구 - 한국기초과학지원연구원(Korea Basic Science Institute)

기간 : 23.08 ~ 23.12

참여인원 : 8명

# 연구 배경
+ 한국기초과학지원연구원 (이하 KBSI) 가 보유한 분석 장비를 대상으로 12대 국가전략기술에 해당하는 기술 및 관련 산업을 지원하고, 장비 활용도를 극대화하기 위한 신규 분석장비 개발 및 기존 분석장비 활용도 요구가 커지고 있음
+ 이에 KBSI가 보유한 분석장비 관련 기술의 경쟁력을 파악하고, 전략산업과 연관된 분석장비의 특성을 반영하여 분석장비 활용도를 높이고 자원 활용도를 극대화하는 것이 필요함
+ 특허는 기술의 중요한 대용지표로 활용될 수 있으므로, 특허분석을 바탕으로 해당기술의 경쟁력 및 관련 전략기술과의 유사성 및 적합성 등을 파악하는 것이 요구됨 


# 연구 목적
+ KBSI(Korea Basic Science Institute) 보유 분석장비 관련 기술의 경쟁력을 파악하고, 전략산업과 연관된 적용가능 유망기술을 도출하고자 함
+ 이러한 과정을 시스템적이고 체계적으로 수행하기 위한 특허분석 방법론을 제시하고 이를 개발·적용하는 데 목적이 있음

# 프레임워크

![image](https://github.com/shinho123/23.08-23.12-KOREA-BASIC-SCIENCE-INSTITUTE-/assets/105840783/4026b77a-ca3c-4d91-a390-e795af04cd62)

# 수행 역할
+ 특허 데이터 수집(Google Patents), 데이터 필터링, 데이터 전처리, LDA 토픽 모델링, 네트워크 분석

+ 데이터 수집 : Goole Patents에서 수집

# 분석 결과
+ LDA 분석 결과 - 국내·외 MRAM(Magnetoresistive Random Access Memory)과 연관되어 있는 특허(총 31,148건) 중 특허의 'abstract'속성과 'title' 부분의 데이터를 결합 후 LDA 토픽 분석을 수행
+ MRAM과 연관되어 있는 특허에서 주로 중요한 관점으로 도출 되는 기술 키워드들을 분석
  
```python
ldamodel = gensim.models.ldamodel.LdaModel(corpus, num_topics = 6, id2word = dictionary, random_state = 3)
ldamodel.print_topics(num_words = 10)
```

## 토픽별 주제 선정 및 키워드 도출

![image](https://github.com/shinho123/23.08-23.12-KOREA-BASIC-SCIENCE-INSTITUTE-/assets/105840783/bed3332a-dee0-4b52-9ea1-e9675a0d8017)

+ Topic 1은 박막 및 회로 구조에서 바닥 부분에 위치한 절연 소재와 소재의 제조 과정에 관한 키워드로 구성되어 있음
+ insulating, dielectric - 절연소재, element, material - 소재, 성분, bottom, area - 위치, barrier - 경계, ferromagnetic - 자성 소재 





