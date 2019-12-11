---
layout: page
title: 학습준비(setup)
root: .
---

학습을 수행하는데 다음 파일을 다운로드 받는다:

1. [data-shell.zip]({{ page.root }}/data/data-shell.zip) 파일을 다운로드 받아서 바탕화면(Desktop)으로 이동한다.
2. 다운로드 받은 파일 압축을 푼다.(도움이 필요한 경우 강사에게 도움을 요청한다.) 바탕화면에 **data-shell** 폴더가 새로 생성되어야 한다.
3. 터미널을 열고 `cd`를 타이핑하고 엔터를 친다. 현재 작업 디렉토리로 홈 펄도로 이동하게 된다. 

이번 학습을 통해서, **data-shell** 폴더에 저장된 데이터에 접근하는 방법을 알게 된다.


> ## 명령어를 타이핑하는 장소: 쉘을 새로 여는 방법
> 쉘은 프로그램으로 명령을 컴퓨터에 전송하고 출력값을 받게하는 역할을 한다.
> 터미널(terminal) 혹은 명령라인(commmand line)으로도 불린다.
> 
> 일부 컴퓨터 운영체제에 유닉스 쉘 프로그램이 기본내장되어 있다.
> 아래에 (설치된 경우) 유닉스 쉘 프로그램을 열고 식별하는 방법을 기술되어 있다.
> 
> 유닉스 쉘 프로그램, 리눅스/유닉스 에뮬레이터, 서버에 유닉스 쉘에 접근하는 프로그램을 다운로드하고 식별하는 선택옵션도 존재한다.
>
> 아래 선택옵션중 어떤 것도 해법이 되지 않는다면, 온라인 도움말을 참고한다: 유닉스 쉘 [your computer model] [your operating system].
>
> ### 리눅스(Linux)
> 리눅스 운영체제에 기본 설정된 유닉스 쉘은 배쉬(Bash)다.
> 대부분의 리눅스 버전에서, [(Gnome) Terminal](https://help.gnome.org/users/gnome-terminal/stable/),
> [(KDE) Konsole](https://konsole.kde.org/),
> [xterm](https://en.wikipedia.org/wiki/Xterm) 을 실행해서 접근할 수 있다.
> 응용프로그램 메뉴 혹은 검색창을 통해서도 가능하다.
> 배쉬외에 다른 쉘이 장착되어 있다면, 터미널을 열고, `bash`를 실행하면 된다.
>
>
> ### 맥(Mac OS)
> 맥 컴퓨터의 경우도 기본설정된 유닉스 쉘은 배쉬(Bash)다.
> Application 폴더에 Terminal Utilities 프로그램을 실행하면 사용할 수 있다.
>
> 터미널을 열려면, 다음 선택지중 하나를 시도하면 된다:
>
> * Applications으로 이동한다. Applications 에서, Utilities 폴더를 연다. Utilities 폴더에서 Terminal을 지정하고 열면 된다.
> * 맥 ‘Spotlight’ 검색 기능을 사용하는 경우. `Terminal`을 검색어로 던지고 나서 <kbd>Return</kbd>를 친다.
>
> #### 참고문헌
> [How to Use Terminal on a Mac](http://www.macworld.co.uk/feature/mac-software/how-use-terminal-on-mac-3608274/)
>
> ### 윈도우
> 윈도우 운영체제를 갖춘 컴퓨터에는 자동으로 유닉스 쉘 프로그램이 설치되어 있지 않다.
> 이번 학습에서 윈도우 사용자는 **Git for Windows**에 포함된 에뮬레이터를 사용하길 권장한다.
> **Git for Windows**는 배쉬 쉘 명령과 Git을 동시에 사용할 수 있게 해 준다.
> 소프트웨어 카펜트리 워크샵에 참석한 경험이 있다면, 이미 **Git for Windows**를 설치하는 방법을 알고 있을 것이다.
>
> **Git for Windows** 설치가 끝나면, 윈도우 시작 메뉴에서 Git Bash 를 실행하게 되면 터미널이 열린다.
>
>
> 윈도우에서 배쉬 명령을 실행하는 다른 방법도 존재한다.
> 윈도우 10에서는 배쉬 쉘 명령라인 툴이 가능하게 되었다.
> 추가로, 윈도우 컴퓨터에서 유닉스 쉘이 장착된 원격 컴퓨터 혹은 서버에서 배쉬 명령어를 실행할 수도 있다.
> 
> 이 작업은 보통 Secure Shell (SSH) 클라이언트로 작업하게 된다.
> 윈도우 컴퓨터에서 무료로 이용가능한 클라이언트 프로그램이 PuTTY다. 
> PuTTY를 설치하고 사용하는 방법, 윈도우 10 명령-라인 도구, 유닉스/리눅스 에뮬레이터 설치 및 사용에  대한 도움말은 다음 참고문헌을 살펴보기 바란다.
>
> #### 참고문헌
> * [Git for Windows](https://git-for-windows.github.io/)
> * [How to Install Bash shell command-line tool on Windows 10](https://www.windowscentral.com/how-install-bash-shell-command-line-windows-10)
> * [Install and Use the Linux Bash Shell on Windows 10](https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/)
> * [Using the Windows 10 Bash Shell](https://www.howtogeek.com/265900/everything-you-can-do-with-windows-10s-new-bash-shell/)
> * [Using a Unix/Linux emulator (Cygwin) or Secure Shell (SSH) client (Putty)](http://faculty.smu.edu/reynolds/unixtut/windows.html)
{: .callout}
