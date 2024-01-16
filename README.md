# 주가 & 뉴스 데이터 감성분석 파이프라인 구축프로젝트  
<br/>
<br/>
<br/>

## 이어드림스쿨3기 데이터엔지니어링트랙 mlops 파이프라인 프로젝트 5팀의 프로젝트 기록입니다.
<br/>
<br/>
<br/>
<br/>
<br/>

## 프로젝트 요약.
<br/>
<img width="642" alt="image" src="https://github.com/junyoungparkdev/yeardreamstock-team05/assets/132217286/0a7afa9e-4dc7-4fed-b892-fea0939cbb20">
<br/>
<br/>
주식에 관심 있지만, 시간은 없는 바쁜 사회인들을 위해 주식차트와 해당 시간대에 보도된 뉴스를 함께 보여주며 감성분석모델까지 적용하는 대시보드를 만드는 것을 목표로 진행한 프로젝트입니다.<br/>
<br/>
<br/>

## 아키텍쳐 설명. <br/>
<img width="631" alt="image" src="https://github.com/junyoungparkdev/yeardreamstock-team05/assets/132217286/9099e591-9211-4bd1-b1d8-4945db0cf8e7">
<br/>
<br/>

1. 증권사 api를 통하여 국내 상장 주식의 5분봉 데이터와 함께 뉴스 데이터를 kafka로 전송합니다. <br/>
2. kafka로부터 hadoop으로 데이터를 전송하는 작업, 백업db인 mysql,hbase로의 데이터 전송, 모델 테스트를 airflow dag으로 관리합니다. <br/>
3. 최종 대시보드 형태는 flask 웹 어플리케이션으로 구현합니다. <br/>
4. 데이터의 정합성 여부 판단, 부하 이슈 등 모니터링을 위해 grafana, portainer를 구축했습니다.<br/>
5. 이미지 빌드를 통하여 아키텍쳐를 구축했습니다.<br/>
<br/>
<br/>






