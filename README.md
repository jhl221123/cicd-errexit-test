# cicd-errexit-test

목표: `set -e` 옵션의 동작을 확인합니다.

### 시나리오1

* `set -e` 없이 `echo` 내부에서 gradle 명령어 실행
* gradle 명령이 실패하더라도 작업이 실패하지 않는다.

### 시나리오2

* `set -e` 적용한 후, `echo` 내부에서 gradle 명령어 실행
* gradle 명령이 실패하면, 그 즉시 작업이 실패한다.