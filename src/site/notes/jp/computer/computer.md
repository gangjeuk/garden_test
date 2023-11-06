---
{"dg-publish":true,"permalink":"/jp/computer/computer/","tags":["Computer-Science"],"created":"2023-10-15","updated":"2023-10-22"}
---


# Reference
컴퓨터과학이 여는 세계
# 컴퓨터의 시작
컴퓨터는 왜 등장했을까?

먼저 컴퓨터라는 단어의 기원에서부터 시작해 보자.

컴퓨터라는 단어는 compute + er ,즉 계산하는 '자' 라는 의미를 가진다. 

의미에서 알 수 있듯이 근대역사에서 컴퓨터가 가지는 의의를 하나의 단어로 정리하자면 계산의 '자동화'일 것이다.

자동 계산기를 이용하여 탄도의 궤적을 계산하고, 핵폭탄의 폭발을 시뮬레이션하는 등 현재 우리가 사용하는 데스크탑 위의 컴퓨터와는 전혀 다른 모습으로 사용되었다.

![jp/computer/assets/computer/image-20231010232656227.png|center|150](/img/user/jp/computer/assets/computer/image-20231010232656227.png)
2015년에 개봉한 엘런 튜닝의 일대기를 다룬 이미테이션 게임에서 등장하는 기계 또한 암호해독을 위한 자동화 기계라고 생각할 수 있다.

> [!note]
> Computer는 *자동화*라는 키워드로 설명할 수 있다


# 자동화, 자동화, 자동화!!
사실 여기까지 이야기를 진행하면 컴퓨터 녀석이 그저 전쟁에서나 사용되고, 사람이 계산해야 하는 값을 대신 계산하는 단순한 기계라고 생각하기 쉽다. 

하지만, 원래 컴퓨터라는 기계는 그것보다는 더 큰 목표를 가지고 만들어졌다...

## 증명하는 기계
과거의 수학자들은 다음과 같은 기계를 발명하길 원하였다.
>[!note]
>어떠한 명제들의 참과 거짓을 *자동으로* 판별하는 기계를 만들고 싶다!!

수학자들은 어떠한 기계적인 과정을 통해 수학의 명제를 던지면(input으로 넣으면), 자동으로 참과 거짓을 출력해 주는(output으로 출력하는) 기계를 원한 것이다.

지금 생각해도 말도 안 되는 정말 거대한 목표를 향하여 나아가고 싶었던 과학자들은 금방 벽을 만나게 된다.

## 불완전성 원리
이상한 단어가 나왔다고 너무 무섭게 생각할 필요는 없다.

불완전성 원리라는 단어보다는 다음과 같은 사실이 중요하다.
>[!error]
>**그런 기계는 못 만들어!!**

그렇다 세상만사가 그렇게 편하게 흘러가지 않는다는 사실을 여기서도 볼 수 있다.

불완전성 원리를 조금 더 자세히 설명하자면 다음과 같다.

>[!info]
>모순이 없는 수학 체계에서 증명할 수 없는 명제가 존재한다

즉 이어지는 논리는 다음과 같다. 
"증명할 수 없는 명제가 존재한다, 그렇기 때문에 모든 명제를 증명할 수 있는 기계는 존재할 수 없다."

이러한 기계가 존재하지 못한다는 사실은 다양한 측면에서 정의되었다.
수학의 세계에서는 괴델에 의해서 그리고 컴퓨터의 세계에서는 엘런 튜닝에 의해서.

## 엘런 튜닝과 튜링 머신
튜닝은 이런 말도 안 되게 편한 기계가 존재할 수 없다는 것을 증명하기 위해서 '기계적인 절차'라는 것을 정의하여야 했다.

즉, 어떤 것이 기계적인 절차인가?

그렇게 등장한 것이 바로 **튜링 머신**이다.

튜링 머신의 대략적인 구조는 다음과 같다.
![jp/computer/assets/computer/image-20231015200814852.png|center round|450](/img/user/jp/computer/assets/computer/image-20231015200814852.png)
\[출처 - https://gusdnd852.tistory.com/66\]

위 그림이 복잡해 보일 수 있다.

[[jp/computer/computer#조금 더 자세한 설명\|복잡하면 무시하고 지나가도 된다.]]

하지만 조금 더 알고 싶은 사람은 계속 글을 읽어보자, 현대의 컴퓨터의 구조와 거의 똑같다!! (~~그렇다 컴퓨터의 구조는 그때부터 지금까지 거의 바뀌지 않았다~~)
### 조금 더 자세한 설명
위 튜링머신을 간단하게 이해하기 위해서 우리가 사용하는 컴퓨터의 모식도와 비교하여 보자.
![jp/computer/assets/computer/image-20231015203014572.png|center round|700](/img/user/jp/computer/assets/computer/image-20231015203014572.png)

일단 그림을 보면 다음과 같은 생각이 들 수 있다.
1. 그림이 허접하다!!
	1. ~~죄송합니다~~
2. 이게 뭐가 컴퓨터야!! 뭐가 너무 빠져있다!!
	1. 키보드도 없다, 마우스도 없다
	2. 하드디스크, SSD는 어디있냐?
	3. 그래픽카드는?
그림이 조금 허접해도 기억해 두길 바란다, 우리의 여정은 이 그림에 **키보드와 마우스를 연결하고, 또 하드디스크를 추가하는 여정이 될 테니까!!**

다시 본론으로 돌아와서 튜링머신은 다음과 같은 요소로 이루어져 있다.
1. 무언가를 기록할 수 있는 테이프
2. 테이프에 기록되는 심벌들
3. 심벌들이 기록된 테이프를 읽거나 쓰는 장치
4. 장치의 상태를 나타내는 심벌들
5. 기계의 작동 규칙 표

벌써 머리가 아파온다, 하지만 다음과 같이 생각하여 보자.

| 튜링 머신              | 컴퓨터                           |
| ---------------------- | -------------------------------- |
| 테이프                 | RAM 메모리(RAM을 모르는 사람은 [클릭](https://en.wikipedia.org/wiki/Dynamic_random-access_memory))                   |
| 테이프 위 심벌들       | 메모리상의 값                    |
| 읽거나 쓰는 장치       | CPU                              |
| 상태를 나타내는 심벌들 | 레지스터(?)                      |
| 작동규칙표             | 그림에서의 명령어(add, write, etc..) |
~~이런 혁명적인 분류에 대해서 전공자분들의 관대한 양해를 부탁드립니다..~~

이제 조금 편해졌는가?
이제 CPU가 되어서 메모리(RAM 메모리) 상의 다음과 같은 명령어를 수행하여 보자.
- add 10 20: 10과 20을 더하고 레지스터에 기록하라
- write: 메모리(테이프)에 값을 적어라
그림으로 나타내면 다음과 같을 것이다(작을 경우 확대해서 확인).
![jp/computer/assets/computer/image-20231015205705383.png|center|700](/img/user/jp/computer/assets/computer/image-20231015205705383.png)
CPU는 명령어(작동규칙표)에 따라서 값을 계산하거나, 메모리(테이프)에 값을 쓰거나 하는 동작을 하나씩 *기계적으로* 수행해나가게 된다. 

튜링은 이러한 일련의 과정을 수행하는 기계의 동작을 '기계적 동작'이라 정의하였고, 이러한 '기계적 동작'을 수행하는 기계를 이용해서 불완전성 원리를 일명 **정지 문제**[^1]라는 문제로 증명하였다.

여기서 조금 더 나아가 한번 더 추상화를 통해 생각하면, 튜링 머신을 나타낸  Software(그림상에서 Software라고 적힌 부분)가 우리가 부르는 Code라고 생각하여도 무방하다. 사진에서의 코드는 메모리 상에서 데이터 배열 `* $ * *` 을 `* * * $`로 바꾸는 코드 이다.

관심이 있는 사람은 [[jp/computer/computer#부록 - 튜링 머신 해석하기\|해석 방법을 아래에 추가해 두었다]].
# 부록 - 그 외 유명한 인물
컴퓨터과학의 영역에서는 빼먹을 수 없는 유명한 사람들을 알아보자.

## 에이다 러브레이스 - if, for(반복, 조건)의 구조를 사용한 최초의 프로그래머
컴퓨터과학이라는 학문이 꽃 피던 시절에 여성 프로그래머들의 공헌은 부정할 수 없는 사실이다.
하지만 이분은 컴퓨터과학이라는 학문이 존재하기도 전에 혼자서 현대의 프로그래밍의 개념을 만들어서 사용하신 ==최초의 프로그래머==이시다.
![jp/computer/assets/computer/image-20231015221228342.png|center round|150](/img/user/jp/computer/assets/computer/image-20231015221228342.png)
위에서는 마치 최초의 컴퓨터는 전쟁이라는 배경에서 탄생하였고, 수학자들에 의해서 증명된 것처럼 이야기하였지만, 사실 자동화', '컴퓨터 라는 키워드는, 단어는 사용되지 않았을지언정 그 전에서부터 존재하였다.

그 대표적인 예시가 바로 [해석 기관](https://en.wikipedia.org/wiki/Analytical_engine)이다. 해석 기관은 천공 카드라는 프로그래밍 코드가 적힌 판을 입력받아서 동작하는 CPU라고 이미지화하면 된다.

그 당시 과학자들은 이러한 CPU에 간단한 사칙 연산 등이 가능하게  에이다 러브레이스는 이 CPU의 코드를 만든 최초의 프로그래머이다.
## 그레이스 호퍼 - 최초의 디버깅
![jp/computer/assets/computer/image-20231015224013657.png|center round|200](/img/user/jp/computer/assets/computer/image-20231015224013657.png)


![jp/computer/assets/computer/image-20231015222037438.png|center round|300](/img/user/jp/computer/assets/computer/image-20231015222037438.png)
실제로 버그가 끼어서 발생한 문제를 최초로 디버깅한 프로그래머이다.
버그와 디버그가 컴퓨터 과학에서 본격적으로 사용되었다는 대표적인 일화를 만든 장본인이자, 최초로 영어로 만든 언어를 창시한 컴퓨터 과학자이기도 하다.

과거에 BASIC과 함께 교육용으로 많이 사용된, 그리고 코로나19가 창궐하던 시절 개발자 모집 문제로 뉴스가 나왔던 ==코볼==이라는 언어의 창시자이다!!



## 마가렛 해밀튼 - 아폴로 프로젝트

![jp/computer/assets/computer/image-20231015220526810.png|center round|150](/img/user/jp/computer/assets/computer/image-20231015220526810.png)
혹시 아폴로 로켓에도 CPU가 들어있었다는 사실을 아는가?

사실 아폴로 로켓이라는 거대한 구조체를 다루기 위해서 컴퓨터가 탑제되어 있었다. 그리고 그 말인즉슨 프로그램도 존재했다는 사실이다.

정말 믿기지 않게도 사진의 마가렛 해밀튼 옆에 쌓여있는 종이가 전부 코드이다;;
[(깃허브에서 코드도 볼 수 있다 ㄷㄷ)](https://github.com/chrislgarry/Apollo-11/tree/master)

마가렛 해밀튼은 아폴로 프로젝트에서 여러 소프트웨어를 담당하여 개발을 진행하였고 이후 이러한 대규모 소프트웨어를 다루기 위한 이론인 '소프트웨어 엔지니어링'이라는 분야에 큰 영향을 끼치게 된다.

약간의 첨언을 하자면, 이러한 생각을 하는 사람이 있을 수 있다. "아니, 저게 코드면 저걸 전부 로켓에 실어서 발사했나?"

물론 아니다, 이 시절에도 놀랍게도 HDD, RAM 같은 저장매체가 존재하였다 바로 [자기 코어 메모리](https://en.wikipedia.org/wiki/Magnetic-core_memory)이다.
![jp/computer/assets/computer/image-20231015223043904.png|center round|100](/img/user/jp/computer/assets/computer/image-20231015223043904.png)
컴퓨터는 위 그림에서 보이는 자기 코어 메모리에 이러한 데이터를 저장하여 우주에서 실행하였다. (그 시절 자신의 프로그램이 오작동하여 우주 비행사가 죽을 수도있다는 압박감을 이겨내고 프로그램을 만든 사람들이 정말 존경스럽기까지 하다;;)
## 데니스 리치 / 켄 톰프슨 - Unix, C 언어
지금까지 여성 과학자들을 살펴보았다면 이제 컴퓨터 공학의 레전드들인 데니스 리치와 켄 톰프슨을 소개하지 않을 수 없다.
![jp/computer/assets/computer/image-20231015223409468.png](/img/user/jp/computer/assets/computer/image-20231015223409468.png)
자세한 운영체제의 역사는 따로 설명하겠지만, 이분들 둘이서 지금까지 사용되는 C 언어, 그리고 Unix를 개발하고 사실상 오픈소스 운영체제의 표준인 Linux의 기준(POSIX)을 제시하셨다.

또한 켄 톰프슨은 UTF-8, 정규표현식 등 컴퓨터공학을 조금이라도 하였다면 들어본 적 있을 법한 것들을 많이 만드셨다.
# 부록 - 역사... 조금만 더 
역사, 특히 전쟁의 역사와 기술의 개발은 공학자를 흥분시키는 키워드 중 하나일 것이다.

운영체제의 역사를 조금 더 논하기 전에 운영체제와 뗄레야 뗄 수 없는 인터넷의 역사를 조금만 맞보고 가자.

우리가 흔히 'The Internet'이라고 부르는 단어의 기원은 ==미국 국방부== 산하 ==고등 연구 계획국==(흔히 달파, 다르파라고 부르는)에서 제작한 알파넷(아파넷, 아르파넷)에 그 기원을 두고있다.

미국의 국방부가 다른 나라의 국방부와 차별화되는 가장 큰 부분은 아마도 국방부가 국가 기술 개발의 선두에 서 있다는 점일 것이다.(현재까지고 이러한 기조는 이어지고있다)

알파넷또한 국방부의 요구에 따라 만들어졌고, 첫선을 보인 시기가 1969년, 우리가 흔히 냉전 시기라 부르는 때에 만들어졌다.

알파넷은 핵전쟁에 대비하기 위해 서버 간이 연결을 위해 탄생하였고, 최초로 end-to-end의 패킷 교환 방식의 인터넷이었다. 이 시기를 기점으로 우리가 흔히 사용하는 E-mail 등 도 탄생하게되었다.

# 부록 - 튜링 머신 해석하기 
![jp/computer/assets/computer/image-20231015200814852.png|center round|500](/img/user/jp/computer/assets/computer/image-20231015200814852.png)
먼저 해석을 위해서는 Software라는 표를 이해하여야 한다.
CPU에서 예를 들었던 add 또는 write 같은 명령은 다음과 같은 블럭 단위로 읽어야 한다.

![jp/computer/assets/computer/image-20231015211351355.png|center|250](/img/user/jp/computer/assets/computer/image-20231015211351355.png)
add, write와 달라 보이지만 같은 명령어이다. 
해석 방법은 다음과 같다, 
- 현재 프로세서의 상태: Start
- 읽는 값: R
- 쓰는 값: W
- 프로세서의 위치 이동: Point
- 다음 프로세서의 상태: End
위 그림은 다음과 같이 해석할 수 있다.
>[!note]
>현재 프로세서의 상태(Start)가 A이 경우에 
>읽는 값(R)이 \* 이면
>쓰는 값(W)으로 \* 을 쓰고
>프로세서의 위치(Point)를 오른쪽으로 옮기고(>)
>다음 프로세서의 상태(End)를 A로 한다
>

각 명령어에 번호를 붙이면 다음과 같다.
![jp/computer/assets/computer/image-20231015212728453.png|center round|300](/img/user/jp/computer/assets/computer/image-20231015212728453.png)
이제 CPU(Processor)가 읽어 들이는 값에 따라서 어떻게 동작하는지 살펴볼 수 있다.

CPU가 메모리상에서 처음 읽는 값은 \* 이고 (==\*== \$ \* \*) 이고, 초기 CPU의 상태는 `A`이다, 그러므로 명렁어 `1`이 실행된다. 그리고 CPU의 위치를 오른쪽으로 옮기고 CPU 상태를 `A`로 한다.

다음으로 읽는 값은 $이고(\* ==\$== \* \*) 현재 CPU의 상태는 `A`이다, 그러므로 명령어 `2`가 실행된다. 그리고 CPU(Processor)의 위치를 오른쪽으로 옮기고 CPU(Processor) 상태를 `B`로 한다.

이렇게 계속 이어가면 최종적으로 메모리의 상태가 `* * * $`가 되고, 위 그림의 코드(Software)로 작성된 프로그램은 종료한다.



[^1]: 정지 문제는 찾아보는 것을 추천한다.(재미있다 ~~조금 헷갈리지만~~) - http://youtube.com/watch?v=92WHN-pAFCs&embeds_referring_euri=https%3A%2F%2Fnamu.wiki%2F&source_ve_path=Mjg2NjY&feature=emb_logo