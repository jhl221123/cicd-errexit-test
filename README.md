# cicd-echo-test

목표: `echo` 내부 명령어 실패가 Job 실패로 이어지는지 확인합니다.

### 시나리오1

* `echo` 내부에서 gradle 명령어 실행
* gradle 명령이 실패하더라도 작업이 실패하지 않는다.

### 시나리오2

* `echo` 내부에서 gradle 명령어 분리
* gradle 명령이 실패하면, 그 즉시 작업이 실패한다.