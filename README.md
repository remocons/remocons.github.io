# remocons 

## 리모컨 블로그
리모컨 공개 라이브러리 세부 정보는 블로그를 참고하시기 바랍니다.
[https://blog.remocon.kr](https://blog.remocon.kr)


## 리모컨 오픈소스 라이브러리 목록입니다. 


## Remote Signal

1. 목적

   리모트시그널은 웹 디바이스의 인증 및 실시간 암호 통신을 지원하는 공개 라이브러리와 프로그램입니다. JavaScript와 C/C++ 를 지원하므로 웹브라우저(Web Browser) 부터 아두이노(Arduino)까지 다양한 장치에 적용 가능합니다.

2. 구성
- Mac, Windows, Linux 용 서버 및 클라이언트 CLI 프로그램
- 아두이노 클라이언트 용 C/C++ 라이브러리 및 예제소스
- 서버용 JavaScript 라이브러리 및 인증기능 적용 예제소스

3. 응용예
- WebRTC 시그널링
- 암호화 채팅서비스
- IoT 웹 통합
- 서버간 보안통신

4. 저장소
- Javascript: `remote-signal` [ [github](https://github.com/remocons/remote-signal) | [npm](https://www.npmjs.com/package/remote-signal) ]
  - Node.js server
  - Node.js client ( WebSocket, CongSocket)
  - Web Browser client( WebSocket)
- Arduino client: 
  - `remote-signal-arduino` [ [github](https://github.com/remocons/remote-signal-arduino) ]
  - or use Arduino Library Manager: `RemoteSignal`
- CLI program 
  - `remocon` [ [github](https://github.com/remocons/remocon) | [npm](https://www.npmjs.com/package/remocon) ]
  - install: `sudo npm i -g remocon`
  - support mac, linux and windows.
  - server and client


## remocon

리모콘(리모트콘솔)은 리모트시그널(Remote Signal) 서버와 클라이언트를 실행할 수 있는 CLI 프로그램입니다. NodeJS 를 지원하는 맥, 윈도우, 리눅스 모두에 설치 가능합니다.


- 저장소 `remocon` [ [github](https://github.com/remocons/remocon) | [npm](https://www.npmjs.com/package/remocon) ]
- install: `sudo npm i -g remocon`
- support mac, linux and windows.
- server and client


## meta-buffer-pack
```
npm i meta-buffer-pack
```
[ [npm](https://www.npmjs.com/package/meta-buffer-pack) 
| [github](https://github.com/remocons/meta-buffer-pack)
| [online demo](https://remocons.github.io/meta-buffer-pack/example/index.html)

Node.js 와 Browser 에서 공통으로 사용 가능한 버퍼 패키징 도구입니다. 
다양한 크기와 타입의 바이트 정보들을 하나의 버퍼 구조로 합쳐주고, 원래의 자료형으로 자동 복원해주는 기능이 있습니다.

MB: 메타 버퍼란?
- ["이름","타입","버퍼"] 정보를 명시적으로 내포한 자료형입니다.
- 이름: 사용자 정의 버퍼의 이름
- 타입: 버퍼의 크기, 엔디안, 자료형이 모두 내포된 정보입니다.
- 버퍼: 실제 저수준 바이너리 정보입니다.

특징
- 다중 함수 인자를 자동으로 버퍼팩으로 만들어줍니다. (MBA)
- 복원시 초기 자료형, 사용자 정의 이름을 자동으로 복원 해줍니다. (MBO)

## file-tool(ft)
```
npm i file-tool
```
[ [npm](https://www.npmjs.com/package/file-tool) 
| [github](https://github.com/remocons/file-tool)]

Node.js 와 Browser 는 File 사용법이 다릅니다. file-tool은  Node.js 환경에서 Browser 호환 Web APIs File 인터페이스를 제공하며, 몇가지 암호화 지원 기능을 추가했습니다.

특징
- 파일시스템상의 파일을 브라우저 호환 파일로 변환해줍니다.
- 암호화 삭제(wipe) 기능
- 이름 암호화 변경 (UUID사용) 기능
- 노드 전용입니다.


## otpus 
```
npm i otpus
```
[ [npm](https://www.npmjs.com/package/otpus) 
| [github](https://github.com/remocons/otpus)
| [online demo ](https://remocons.github.io/otpus/example/index.html) ]

이미 Node.js 와 Browser 에 암호화 구현을 위한 API가 포함되어있습니다. 또한 오픈소스 암호 알고리즘도 공개되어있습니다. 하지만 실제 암호화 구현시엔 여러가지 추가 프로세스가 필요합니다. 이러한 과정을 일반화하여 쉽게 바로 사용가능한 범용 암호화 함수를 제공합니다.




