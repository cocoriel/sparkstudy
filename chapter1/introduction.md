
1. Introduction to Spark
	- spark runtime architecture를 활용하면 분산 프로그램을 로컬 프로그램을 작성하듯이 작성할 수 있다!!!
	- 함수형 프로그램을 활용해서 코드를 작성할 수 있음
	- python, java, scala, R로 코드 작성할 수 있음
	- MapReduce 와 비슷한 역할을 하는 배치 프로그램 작성 및 SQL을 활용해서 데이터를 handling할 수 있고 그래프나 machine learning을 활용할 수도 있음
	- spark는 OLTP(online trasaction processing)를 위해서 만들어진 프로그램이 아님!!
2. MapReduce's shortcomings
	- 맵리듀스는 다른 맵리듀스 job에 활용되려면 결과를 HDFS에 저장해 두어야 함
	- 이런 이유 때문에 iterative한 알고리즘에서는 성능이 좋지 않음
	- 또 한가지 문제는 많은 problems들이 맵리듀스의 two-step paradigm에 적용하기 어려움
3. What spark brings to th table
	- spark의 core concept은 in-memory execution모델이라는 점
	- 이 덕분에 맵리듀스보다 최대 100배 정도의 성능을 낼 수 있고, iterative 알고리즘인 machine learning이나 그래프 알고리즘등에 탁월한 효과를 낼 수 있음
	- spark API는 맵리듀스보다 쉬움
	- spark-shell은 interactive console을 제공해줌
	- spark는 unifying platform
	- **OLTP에는 어울리지 않음. 배치 프로세스를 염두에 두고 만들어진 platform임!!**
4. Spark core
	- Resilient distributed dataset(RDD) : 회복력이 있는 분산 데이터셋

> Written with [StackEdit](https://stackedit.io/).