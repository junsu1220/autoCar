지금 현재 학원에서 진행하고 있는 jetson tx2 과정을 내가 진행하고 있는 jetson nano 에 적용시켜 바로 응용시키려 하고 있다.

 


os를 까는것까지는 실행했고 우선 nano에 tensorflow를 수동 설치 하였다.

Tensorflow 수동설치






Tensorflow 예제 테스트

git clone 안되는 경우 해결법

 

출처 : https://apeltop.blogspot.com/2019/01/git-git-clone-fatal-unable-to-access.html

데이터 관리 책을 보며 따라 하던 와중 git 코드를 쳤는데 안되었습니다.

$ git clone https://www.github.com/efkbook/blog-sample
fatal: unable to access 'https://www.github.com/efkbook/blog-sample/': Could not resolve host: www.github.com


해결 방법은


git config --global --unset http.proxy
git config --global --unset https.proxy
git clone https://www.github.com/efkbook/blog-sample 가 아니라
git clone https://www.github.com/efkbook/blog-sample.git



우선 tensorflow 설치에서 

 

libnvinfer.so.5 cannot open shared object file no such file or directory

 

가 떴지만 진행은 되어 일단 계속 진행하는데

 

다 진행하다가 마지막 image테스트에서

 

opencv가 없다고 오류가 떴다.

 

opencv 를 까는데 

 

makefile:162: 'all' failed 오류가 떴다...

 


 

뭔가 잘못되도 단단히 잘못되고 있었다.

 

하지만 지난번의 os 문제를 경험한 나는 이런경우의 좋은 해결법을 깨달았다.

 

신뢰할 수 있는 사이트의 레퍼런스를 그대로 따라하는것!

 

역시 제일 신뢰하는 사이트는 

 

https://blog.naver.com/zeta0807/221894230137

 
젯슨 나노에 waveshare 동키카 개발환경 만들기

글 작성: 2020.04.06 1차 수정: 2021.03.22, 시작 이미지 다운로드 하는 곳 추가 아래 최대표님의 글 중 2....

blog.naver.com
 

이 사이트이다. 정말 매우 많은 도움을 받고 있다.

(혹시 문제시 연락주세요...)

 

이 사이트를 토대로 다시 opencv부터 yolo까지 실행해 봐야겠다.
