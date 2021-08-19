자율주행로봇 프로젝트를 하기로 마음먹고 드디어 젯봇을 받았다.

![image](https://user-images.githubusercontent.com/87622597/130150379-54090464-c3cf-421a-a332-a229257cb60a.png)

받았는데 hdmi to hdmi 케이블이 없어 또 기다리다가 케이블을 받고 이제 컴퓨터에 연결했는데 화면이 뜨질 않는다. 

전기수가 하던걸 받아서 하는거라 os부터 안되어있다고 판단하고 다시 처음부터 시작했다.

제일 먼저 한 일은 젯슨나노용 sd card이미지를 굽는것 그러기 위해 우선 니비디아 홈페이지에서 

젯슨 나노용 이미지파일을 다운로드받고(zip파일이 5GB, 압축풀면 12GB이다...)

![image](https://user-images.githubusercontent.com/87622597/130150854-900911e4-7afb-427a-b3ce-44edc822bae1.png)

그 다음 SD 카드 포매터를 이용해 sd카드를 포맷시켜줬다.(다행히 전에 라즈베리를 하며 sd카드리더기가 있었다.)

![image](https://user-images.githubusercontent.com/87622597/130151197-6de0cc09-babb-42a7-8891-c9698e4cd87f.png)

완료되면 아래와 같은 창이 뜬다. 확인 후 프로그램을 종료했다.

![image](https://user-images.githubusercontent.com/87622597/130151277-3f359d80-1a2c-4a3a-a030-45aa150a264d.png)

그 다음은 sd카드에 이미지를 로드하기 위해서는 여러 방법이 있는데 나는 익숙한 Win32Disk Imager를 이용하기로 했다.

https://sourceforge.net/projects/win32diskimager/

이미지 파일은 아까 받았던 12GB를 지정하고 디바이스는 우리의 sd카드를 지정한 후 실행한다.

![image](https://user-images.githubusercontent.com/87622597/130151644-4fa163dc-b0f6-43e4-a696-189f94111b2c.png)

![image](https://user-images.githubusercontent.com/87622597/130151659-53a3df26-8237-42e4-80d1-8d649dce0149.png)

(사진을 못찍어서 다른 사이트의 사진을 잠깐 가져왔다...출처 : https://wendys.tistory.com/141)

![image](https://user-images.githubusercontent.com/87622597/130151752-76f0d7b1-9694-4a08-8561-a62871650627.png)

이후 수많은 디스크볼륨으로 할당되게 되고 포맷을 해야한다고 15개정도가 뜨는데 다 취소를 눌러 준다.

자 이제 잿슨나노에 sd카드를 넣고 부팅하는데 화면이 까맣다...

![image](https://user-images.githubusercontent.com/87622597/130152037-7386fdf7-e4fd-49dc-a5ff-701e38c06f62.png)

여기서 1차 패닉. 아니 화면도 못보고 막혀버리다니... 방법을 열심히 찾아보고 나온 1차 결론은 잿슨나노에 넣었던 전류와 전압이

기준치를 미달해서라고 생각했고 또 다른 어댑터를 기다려야겠다고 생각했다. 

근데 그렇게 다른 어댑터를 기다리기에는 미심쩍은 부분이 있었다.

첫째 어댑터의 스펙을 보면 분명 미달이 아니었고 

둘째 전원 문제인 경우는 micro usb 5v 2.0A인 사람들이었는데 우리는 배럴잭을 사용했고 

심지어 더 높은 전원을 위해 점퍼도 달려있었다.

![InkedKakaoTalk_20210820_072914503_LI](https://user-images.githubusercontent.com/87622597/130152655-e58148bb-61f6-42b2-9a09-897115516fbc.jpg)

하지만 그 외의 다른 해결방안을 찾아봐도 없고 심지어 퇴근시간이라 강사님께서도 내일 새로운 잿슨나노를 가져올테니 한번 비교해보고

문제를 찾아보자 하셨다. 여기서 나도 집에 가야하나 하고 잠깐 밖에나가 전화통화 하며 리프레시하다 다시 들어왔는데

문득 예전에 나는 경험안했지만 다른 학생들이 모니터가 hdmi를 인식못하고 아날로그만 인식해서 화면이 안떴던적을 떠올랐다.

설마 설마 하며 모니터의 환경설정 버튼을 알아보고 적용해보니까...

![image](https://user-images.githubusercontent.com/87622597/130152918-e4ff2338-1e47-49b5-b709-f713283e3f76.png)

![image](https://user-images.githubusercontent.com/87622597/130152982-c29e9ddb-1c5f-4c46-b9ab-8212b408f0ab.png)

![image](https://user-images.githubusercontent.com/87622597/130152988-ae493c0c-be6e-4e19-be1e-9cbe92d76c56.png)

![InkedKakaoTalk_20210820_070135626_01_LI2](https://user-images.githubusercontent.com/87622597/130153205-e8e3eda2-c8e1-450f-92fa-52f2e393f740.jpg)

뜬다... 화면이 떴다.. 와 이때 진짜 기쁘면서도 너무 억울했다. 알기전에는 도대체 무슨 문제지 감도 안잡혔는데

알고나니 이렇게 허탈할 수가.. 복잡한 마음으로 다음 단계를 수월하게 진행했다. 

![image](https://user-images.githubusercontent.com/87622597/130153299-ece0e1f6-0271-4342-b65e-c20d325ee672.png)

![image](https://user-images.githubusercontent.com/87622597/130153324-168c8970-c036-4133-8fe0-b0b0dd1e70cf.png)

![image](https://user-images.githubusercontent.com/87622597/130153343-632b0b2f-80f2-4ff8-aea6-ad211a3b43ec.png)

![image](https://user-images.githubusercontent.com/87622597/130153356-8ce68ee1-baab-4fb7-83de-1f86b8807e18.png)

![InkedKakaoTalk_20210820_070135626_01_LI2](https://user-images.githubusercontent.com/87622597/130153205-e8e3eda2-c8e1-450f-92fa-52f2e393f740.jpg)

![image](https://user-images.githubusercontent.com/87622597/130153442-02fe126e-24ab-4ba2-aaad-af72488e21e7.png)

![image](https://user-images.githubusercontent.com/87622597/130153456-8b665a58-5f12-41d7-92f4-33d0b75196cd.png)

![image](https://user-images.githubusercontent.com/87622597/130153472-5cb7e43b-05af-4d4d-8992-e4bf7b2e50e8.png)

언어는 경로지정문제때문에 한글로 해도 잘된다하지만 일단 영어로 했다.

키보드는 기본 english(us)로

랜선이 있었기에 자동 지정해주어서 서울 시간으로 잘 지정되었고 

이름은 우리가 잘 인식할 수 있는 이름과 비밀번호로 하였다.

파티션 사이즈는 최대로, 사용안하는 부트로더파티션은 삭제

![image](https://user-images.githubusercontent.com/87622597/130154396-8f95621d-d750-41dd-9e0e-18696c1d0146.png)

우리는 5V어댑터를 쓰기때문에 MAXN을 했다. 나중에 sudo nvpmodel -m0명령어를 통해서 이부분을 수정할 수 있다고 한다.

![image](https://user-images.githubusercontent.com/87622597/130154505-91803bee-03c9-4f7e-9d92-a949727692f6.png)

![image](https://user-images.githubusercontent.com/87622597/130154517-77eb52d9-68e2-474e-840d-96f365518611.png)

![image](https://user-images.githubusercontent.com/87622597/130154544-289f0657-757d-4eb2-af7d-086f2edb9d4b.png)

![image](https://user-images.githubusercontent.com/87622597/130154560-7c9d4ad7-4392-41a6-8b43-c8bfd97d66cc.png)

순서로 부팅이 진행되며 다 진행하면

![image](https://user-images.githubusercontent.com/87622597/130154586-19acb47c-f008-4ca8-b0c3-61a2e04989e7.png)

니비디아 로고가 뜬다. 감격이다. 이게뭐라고...

![image](https://user-images.githubusercontent.com/87622597/130154626-72c18c84-d02d-494c-911a-bee81535b198.png)

![image](https://user-images.githubusercontent.com/87622597/130154635-d2a89a78-a43a-467d-8373-976e05317003.png)

출처:

https://robertchoi.gitbook.io/jetbot/1

https://developer.nvidia.com/embedded/downloads

https://wooono.tistory.com/308

https://deep-eye.tistory.com/56

https://developer.nvidia.com/embedded/learn/get-started-jetson-nano-devkit#write

https://seoftware.tistory.com/107

https://blog.nulsom.com/16

https://blog.nulsom.com/14?category=849958

https://crossall.tistory.com/7

https://wendys.tistory.com/141

https://opencourse.tistory.com/223
