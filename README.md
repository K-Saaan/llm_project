# Prompt Engneering

LLM을 사용해서 Fine-tuning 없이 prompt engneering으로 어느정도의 성능을 얻을 수 있는지 확인하기 위한 project <br/>
Zero-shot text가 주어졌을 때 정형화된 결과를 받고자 하고 이에 대한 성능 평가를 진행하고자 함.<br/>

## Data
> 네이버 쇼핑 리뷰 데이터	  <br/>
> 출처: 네이버 쇼핑 (https://shopping.naver.com/)	<br/>
> 수집 기간: 2020.06~2020.07	<br/>
> 데이터 건수: 20만 건	<br/>

## LLM
> chatGPT 3.5 turbo

## Experiment

#### 1차
- 20건의 데이터 추출하여 수행
- 전체 응답 중 두건에 대해 빈값을 받고 이외에는 정상정인 값 수신
- accuracy : 90%로 빈값을 제외하고 옳바른 값 수신

생각보다 높은 정확도를 보여주는 것을 확인할 수 있었지만 잘못된 응답건은 보완해야할 것으로 보임 또한 텍스트의 길이가 길지 않았기에 길이 및 데이터를 더 늘려서 진행해야할 것으로 고려됨