# Chapter01

## IBM QX setup

책에 있는대로 IBM QX(Quantum Experience) 사이트에서 계정을 생성하고 Composer를 실행해 본다. 현 시점에서는 Circuit Composer라는 이름의 메뉴로 되어 있다.

![IBMQX Circuit Composer](IBMQX_CircuitComposer.png)

책의 스크린샷과 다른 점은 아래와 같다.
- Gates 배치가 우측이 아닌 상단에 있다.
- 최초 qubit 개수는 3개여서 composer 상에 + 버튼을 눌러 qubit 2개를 더 추가해야 5 qubit test가 가능하다.
- QASM 및 Qiskit 코드가 자동 생성되며 composer와 동기화가 되므로 visual coding이 가능하다.
- Histogram 외에 Q-sphere가 추가되서 더 직관적으로 시각화가 가능하다.
- 처음에 backend가 simulator로 되어 있지 않으므로 backend 세팅을 바꾼 후에 진행해야 한다.

### API 키

책은 스크린샷 없이 글로 설명되어 있는데 우측 상단의 my account를 눌러보면 바로 아래와 같은 화면이 나오고 다른 메뉴를 찾아 헤메일 필요 없이 Qiskit in local environment 항목에서 바로 API token을 확인할 수 있다.

![MyAccount_APIToken](MyAccount_APIToken.png)