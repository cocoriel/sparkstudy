
### Support Vector Machine

1. 참고사이트
	- [SVM part1](http://gentlej90.tistory.com/43)
	- [SVM part2](http://gentlej90.tistory.com/44)
	- [VC Dimension](http://www.svms.org/vc-dimension/)
2. 중요 개념
	- margin(마진)
	- support vector(서포트벡터)
	- kernel(커널)
3. 마진
	- 데이터 포인트와 판별경계(hyperplane)과의 최소
	- 여러 판별경계가 있을때는 결국 minmax가 되는군...
	- 학습오차를 일반오차가 최대로 줄어들 때까지 줄이면 좋은 분류기가 되는데 이 때 기준이 되는 학습오차의 정도를 svm에서는 마진이라고 보면 됨
	
	3-1. VC dimension
		- dichotomy : 데이터 포인트들을 나누는 것을 말함
		- shattering : 모든 데이터 포인트를 구분하는 분류모델을 찾을 수 있는 경우에 분류모델이 N개의 데이터 포인트들을 shattering 한다고 함
		- VC dimension : 분류기(모델)에 의해 shatter 될 수 있는 최대 데이터 포인트 개수를 VC dimension이라고 함
		- 따라서 VC dimension은 분류기의 데이터 수용 능력을 즉정하는 기준이라 할 수 있다
		- 보통 n차원 선형 분류기에서의 VC dimension은 (n+1)이 된다
		- VC dimension이 높아지면 일반화 오류가 높아진다고 알려짐(shatter 할때 데이터에 대해 오류없이 완전히 학습되어 지니까 과적합되는 효과가 있음. 따라서 학습 데이터의 차원이 높아질수록 해당 차원의 노이즈까지 학습할 수 있으므로 전체적으로 일반화 오차가 커지게 됨. 그래서 VC dimension이 높으면 좋지 않음)
4. 서포트벡터(support vector)
	- 판별 경계(분류기)까지의 거리가 가장 짧은 데이터를 서포트벡터라고 함
	- 서포트벡터와 마진은 판별경계(분류기)에 따라 달라짐. 
	- 새로운 데이터가 들어왔을 때 전체 데이터포인트와의 내적거리를 보지 않고 서포트벡터와의 내적거리만 구하면 되어서 상당히 계산 비용을 줄일 수 있다는 강점이 있음
5. 커널(kernel)
	- 



> Written with [StackEdit](https://stackedit.io/).