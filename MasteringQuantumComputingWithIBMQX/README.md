# Quantum Computing with IBM QX

## Overview

이 책에는 각 챕터별로 실행해 볼 수 있는 프로그램 코드가 있으며 이는 github의 아래 주소에서 확인할 수 있다.
[SourceCode](https://github.com/jongfeel/Mastering-Quantum-Computing-with-IBM-QX)

여기 있는 예제 코드를 기반으로 해서 실제 연습문제를 풀어보고 양자 컴퓨터와 그 프로그래밍에 대한 이해를 높이기 위한 목적이 있다.

## Copyright

아마 책 내용을 적으면 문제가 될 소지가 있기 때문에 한번 출판사 쪽에 확인하고 진행할 예정이다. 만약 연습문제 정도가 허락이 되지 않는다고 하면 문제의 간략한 정리 이후 답을 적을 예정이다.

## Development Environment

github의 README에는 필요한 패키지의 버전을 명시하고 있는데 작년 출판된 책 기준이다 보니 버전이 오래됐다.
[예제코드 README의 버전 확인](https://github.com/jongfeel/Mastering-Quantum-Computing-with-IBM-QX#software-and-hardware-list)

그래서 아래와 같이 환경을 최신 버전으로 설치하고 진행해 본다.
설치 방법도 위 링크의 README.md를 확인하면 cli를 확인할 수 있으며 정리해 보면 아래와 같다.

- git clone https://github.com/PacktPublishing/Mastering-Quantum-Computingwith-IBM-QX.git
- cd Mastering-Quantum-Computing-with-IBM-QX
- python3 -m venv book
- source book/bin/activate
- pip install -r requirements.txt
- pip install ipykernel
- ipython kernel install --user --name=bookkernel

### Troubleshooting 1 - activate path

cli 중에 MQC 가상 환경 설정 이후 아래와 같은 명령어는 OS 별로 다르니 확인후에 활성화해야 한다

Mac/Linux

``` python
source MQC/bin/activate
```

Windows

``` python
source MQC/Script/activate
or
cd MQC/Script
Activate.bat
```

### Troubleshooting 2 - jupyter install

위의 설치 방법 명령어에는 jupyter 설치가 빠져 있는데, python 환경을 써 왔고 jupyter notebook을 써왔던 사람이라면 모를까 PC에 처음 세팅하는 사람은 아래와 같은 명령을 실행하면 오류만 날 것이다.

``` python
jupyter notebook
```

당연하게도 jupyter가 설치되지 않아서 생기는 에러이므로 pip로 jupyter를 설치한다.

``` python
pip install jupyter
```

중간에라도 버전이 업데이트 되면 이 README.md문서도 업데이트 될 예정이다.

| Chapter | Software required | OS required |
| -------- | ------------------------------------ | ----------------------------------- |
| All | Python 3.8.5 | Cross platform |
| All | qiskit 0.21.0 | Cross platform |
| All | numpy 1.19.2 | Cross platform |
| All | matplotlib 3.3.2 | Cross platform |
| 8 | pygame 1.9.6 | Cross platform |