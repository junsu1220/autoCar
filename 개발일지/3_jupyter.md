![image](https://user-images.githubusercontent.com/87622597/130533837-b06be5ce-ec6d-4ca0-a834-b5c569102789.png)

이제는 지긋지긋한 도커화면

아직도 도커의 늪에서 빠져나오지 못하고 있다.

현재 드는 생각은 전에 라즈베리파이 했을때처럼 vnc를 이용해서 원격조종을 해야 할 것 같다는 것인데

우선 지금까지 진행한 과정은 

구버전을 깔아서 해보니 

![image](https://user-images.githubusercontent.com/87622597/130533943-f5e8b143-38f2-4775-bbaf-b4c2b4f9c39b.png)

에러가 떠서 

![image](https://user-images.githubusercontent.com/87622597/130533967-de4ab70d-238d-4236-90bf-25e33552351f.png)

로 헤결했고 그래도 도커가 떠서 이번에는 sudo apt update 와 sudo apt upgrade를 안해봤다 

그러니 도커는 안떴지만 여전히 로컬사이트:8888은 들어가지 못했고 

다른 방법으로 아예 주피터랩을 까는 방법을 시도했다.

![image](https://user-images.githubusercontent.com/87622597/130534079-c605a601-dc71-4952-a9d8-c474a9bb8542.png)

그렇게 약간 편법을 써서 주피터 노트북에 드디어 접속을 성공했다.

![image](https://user-images.githubusercontent.com/87622597/130534124-6d91cf79-f7b5-447d-a108-ab31360d5a15.png)

![image](https://user-images.githubusercontent.com/87622597/130534147-4e50f413-489b-4f11-a937-017411a4c0bb.png)

하지만 역시 이상하게 들어가서 그런지 오류가 너무 많이떴다.

cannot allocate memory in static tls block 특히 이 오류는 아직 해결을 못했는데 근본적으로 

이게 맞는 방법인지 의문이 든다... 일단 이해하기로는 주피터랩을 사용해서 구글 드라이브와 연동하고

자체기능으로 켜자마자 주피터노트북이 켜지게 하여 구동하는 것 같은데 개운하지가 않다..

다시 처음으로 돌아가 생각해봐야겠다.

주피터랩 -> https://opencourse.tistory.com/345

부트로더오류 -> https://www.codeleading.com/article/30734974788/

웨이브쉐어 -> https://www.waveshare.com/wiki/JetBot_AI_Kit

유용한 블로그 -> https://m.blog.naver.com/zeta0807/221716022336
