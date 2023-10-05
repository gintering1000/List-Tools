[ReasonWhy](/README.md)
===
[Software / Coding_IDE / UniversialIDE](./README.md)
```
#Choosing #Reason #Software
```

## :card_index_dividers: 유니버셜 IDE ( CUI/GUI )
유니버셜 IDE 는 플랫폼에 종속된 코딩을 제외한 스크립트코딩과 범용적인 코딩을 위한 IDE입니다. 현재 모바일컴퓨터(패드,폰)에서 코딩을 함에 있어서 적절한 IDE가 존재하지 않습니다. 모바일에서는 원격제어를 통한 CUI 에디터로 코딩이 가능하기에 CUI/GUI를 하나씩 선택해야합니다.

**선택조건**
- 기본 : 플랫폼앱개발를 제외한 범용적인 언어선택이 가능해야한다.
- UI : 터미널, 파일트리 기능이 존재해야 한다. ( 별도로 가져가게 되면 굳이 IDE는 필요없다. 메모장이면 된다 )
- UX : 단축키설정과 세부적인 이동, 포커스 기능이 세밀하게 되어야 한다 ( 마우스없이 사용가능 )
- 기능 : 프로젝트파일검색, 명령어검색, 심볼검색, 파일타입선택, 찾기&변환, 멀티커서, 이지모션
- 기타 : CUI/GUI의 통합이 되야함으로 두 에디터의 기능이 동일해야한다.

선택대상
- GUI : ATOM ( 제외 )
- GUI : VSCODE ( 확인중 )
- GUI : INTELLIJ ( 제외 )
- GUI : 클라우드IDE ( 제외 )
- CUI : VIM, NEOVIM ( 제외 )
- CUI : EMACS ( 선택 )

## :card_index_dividers: 상세설명
### GUI : ATOM ( 제외 )

> 제외이유
> - UX부족 : 각종 플러그인에서 터미널의 Toggle이 적절하게 이루어지지 않는다
> - 전반적으로 플러그인이 많으나 그 수준이 낮고 동일한 기능의 플러그인들이 복붙되어 퍼져있다.

> 확인 플러그인
> - platformio-ide-terminal
> - terminal-plus
> - vk-terminal
> - terminal-tab
> - iv-terminal
> - x-terminal

Editor 부분에 포커스 상태에서는 Toggle이 정상적으로 이루어지나, 포커스가 터미널에 존재할때 Toggle이 적절하게 되는 플러그인이 존재하지 않는다.
![Screen Capture 2022-02-11 at 09 23 45](https://user-images.githubusercontent.com/77244047/153519344-b0444273-6a26-4c1d-8816-2a6dfd6413b5.gif)

### CUI : INTELLIJ ( 제외 )

> 제외이유
> - 제작사의 기획의도상 범용적인 IDE 가 아닌 자바에 대한 에디터이다. ( 이는 Eclipse의 대안 밖에 되지 못한다 )
> - 각종 플러그인을 붙일 수 있지만, 여전히 기획의도상 파이썬은 PyCharm, 웹은 Webstrom과 같이 '파편화'되어 있다

![image](https://user-images.githubusercontent.com/77244047/153520896-ab848e9e-9bfa-4a91-bccc-fae6ddc18f97.png)
![image](https://user-images.githubusercontent.com/77244047/153520910-57e18bc2-253e-41c3-ade4-8dec43dd1186.png)

### GUI : 클라우드IDE ( 제외 )

> 제외이유
> - 모든 클라우드IDE는 원하는 프로젝트의 로컬프로그램을 연동하기 힘들다. ( 도커, 가상머신등 각종 툴 전부포함 )
> - 언어를 아무리 많이 지원한들 프로젝트의 시각으로 보면 단순 저수준의 웹코딩이 한계이다.
> - 이는 모바일(아이패드, 안도르이도 등)에서 앱을 사용하지 않고 굳이 SSH로 원격서버에 접속해 IDE를 사용하는 이유와 동일하다.
> - 이동간에 유리하다지만, 노트북과 인터넷이 일상화되어 있는 상황에서 별로 유리점이 없다.
> - 굳이 따지자면 설치나 설정이 필요없어, 기초수준의 <단체 교육시장> 정도에 적합하다.

> 확인된 서비스
> - Codeanywhere
> - Cloud9
> - Eclipse Che 및 관련 프로젝트
> - Goorm IDE

### CUI : VIM, NEOVIM ( 제외 )

> 제외이유
> - 일반적인 GUI 에디터와 사용자 인터페이스 통합을 해야하나 VIM, NEOVIM은 기본적으로 insert모드가 기본이 아님으로 CUI, GUI의 사용성 통합이 어렵다.
> - 서버에 붙어서 사용할 때 단순하게 사용하는게 더 적절할 듯하다. ( 이는 개발용 IDE가 아니라는 뜻이다 )
> - Emacs를 경험해보니 vim의 경쟁자는 Emacs가 아니라 독자노선으로 가고 있다.
> - "난 멋지게 통합에디터로 VIM을 쓸거야!" 하는거면 GUI에디터와 기초사용성이 완전 다르기에 통합된 UX를 포기해야한다.
> - 오해할 수도 있지만 필자는 VIM을 약 10년 가까이 사용했다

### CUI : EMACS ( 선택 )

> 선택이유
> - VIM, NEOVIM의 제외이유들은 Emacs를 선택해야하는 이유이다. ( 다른 대안은 없다 )
> - 설정이 어렵지만 러닝커브는 겪다보면 큰 어려움이 아니다. ( 진짜 어려운건 vim을 선택할시 나중에도 통합이 안된다는거다 )
> - 현대의 GUI 에디터처럼 커스터마이징이 실제 전부 가능하더라. ( 마우스를 안쓴다는 조건으로 )
> - Emacs의 경쟁자는 vim이 아니라, 사실 Nano이다. ( 현대의 모든에디터는 기본모드가 편집모드 )
