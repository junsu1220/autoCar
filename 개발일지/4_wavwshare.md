![image](https://user-images.githubusercontent.com/87622597/130595273-3d3f2f0d-ee55-43f3-b031-6ba190a841f7.png)

드디어 정상적인 방법으로 jupyter notebook을 성공했다.

그동안의 실패이유는 살짝 짐작했던대로 os 버전의 문제였다.

나는 지금까지 jetson nano의 버전에서 선택하여 쓰고있었는데 

강사님이 나의 레퍼런스 사이트들을 보시더니 이건 waveshare에서 지원하는 것이라고 거기서 받아야 한다고 하신것이다.

![image](https://user-images.githubusercontent.com/87622597/130595879-21a2dfac-a9c9-4bf1-8443-78079f3fc487.png)

세상에 여기에 다운로드 링크가 있었다니...

사실 지금까지 힌트가 있었던게 참고 사이트들이 다 이미지를 올려줬었고 그 이미지 이름과 내 이미지이름이 틀렸었다.

또한 다운로드 속도나 굽는시간 업그레이드 시간도 달랐던게 좋은 근거였는데 그걸 다 몰랐었다...

정상적으로 진행되니 OLED에도 정보들이 잘 표기 되었다.

![image](https://user-images.githubusercontent.com/87622597/130596651-679cc7b6-2446-418c-a13e-48a0a82d1dba.png)


결국 이렇게 진행해서 jupyter notebook에 들어가는데 성공했다!

그 다음은 일사천리로 진행되어 카메라와 모터가 정상적으로 작동하는 것을 확인했고 

컨트롤러 관련 코드는 현재 나에게 컨트롤러가 없기에 내일 수정해서 다시 확인해봐야 할 것 같다.

이제 해결해야할 문제들은 

1. 원격접속을 어떻게 할 것인지 : 여자친구가 노트북을 가지고 있으나 여자친구도 써야해서 

계속쓰긴 미안하고 데스크탑에서도 wifi로 접속할 수 있다고 하는데 그건 좀 더 알아봐야할 것 같다 ex)samba server

2. 하드웨어 디자인 : 지금 상태가 영 아닌데 내일 간단하게라도 프레임 역할을 할 나무젓가락과 테이프? 같은걸 준비해서 

한번 뼈대만이라도 잡아 봐야 할 것 같다.

![image](https://user-images.githubusercontent.com/87622597/130596850-6ef187a4-c5e7-4bc0-9c53-23a465a5b228.png)

3. 딥러닝 코드 : 주피터노트북에 있는 코드들을 응용하여 파이썬으로 코드를 짜면 빠르게 딥러닝을 하여 객체인식까지도 가능할 것 같다. 

지금 강사님이 있을때 같이 진도를 맞추어 나가 우선 도움을 받는편이 훨씬 효율적일 것 같다. 따라서 내일은 다같이 지급받은 jetson tx가 아닌

jetson nano로 진행하기위해 지금까지의 과정들을 나노에 빠르게 진행시켜야 할 것이다.

g캠프라는 곳의 강의 과정(심화) https://www.g.camp/1208

한국인을 위한 젯슨나노 깃허브 정말 정보가 어마어마 하다...  https://github.com/jugfk?tab=repositories

젯슨나노 스타트 ssh 관련 주피터노트북과 가상환경등의 정보가 있다(영어)  https://medium.com/@heldenkombinat/getting-started-with-the-jetson-nano-37af65a07aab

항상 도움받는 제타블로그(충돌방지 정보수집) https://blog.naver.com/zeta0807/221760384550

제타블로그도 참고한 기본 젯슨 강의 https://robertchoi.gitbook.io/jetbot/2

제타블로그도 참고한 기본 젯슨 강의가 참고한 제일 중요한 waveshare 공식홈페이지 https://www.waveshare.com/wiki/JetBot_AI_Kit

주피터랩 설치방법 https://opencourse.tistory.com/345

ros 부터 opencv까지 나중에 도움될지도?.. https://95mkr.tistory.com/entry/ROS3?category=746766

오늘 발견한 세종대 sally의 동료 블로그(심화) 도움이 매우 될것같다. https://jgrammer.tistory.com/entry/JETSON-NANO-%EC%9B%90%EA%B2%A9-%EC%A0%91%EC%86%8D?category=903609

원조 sally 티스토리 https://sol2gram.tistory.com/12?category=816331

젯슨나노 부트로더 오류 해결방법(중국어)  https://www.codeleading.com/article/30734974788/

현대모비스 젯슨나노강의 상당히 괜찮음 https://www.mincasurong.com/teaching-experience/mobis-sw-2021-jetson-nano/1-jetson-nano-%EC%A4%80%EB%B9%84
