---
name: Custom Test Case
about: Describe this issue template's purpose here.
title: "[TEST]"
labels: ''
assignees: ''

---

---
name: "🚀 Custom Test Case 공유"
description: "직접 작성한 xv6 테스트 케이스를 공유하고 기여합니다."
title: "[TEST] <테스트할 기능이나 버그를 요약해주세요>"
labels: ""
assignees: ""
---

## 🎯 1. 테스트 목적 (Objective)
> 이 테스트 케이스가 무엇을 검증하기 위한 것인지 간략하게 설명해 주세요.
(예: MLFQ에서 우선순위 역전이 발생하는지 확인, 파이프 버퍼가 꽉 찼을 때의 데드락 검증 등)

## 💻 2. 테스트 코드 (Test Code)
> `uuser/usertest.c`에 추가하거나 독립적인 유저 프로그램으로 실행할 C 코드를 작성해 주세요.
> 성공적으로 테스트에 통과하였을 때에는 0, 에러가 발생하거나 예상과 다른 결과가 발생했을 때는 1, 출력된 결과를 통해 확인해야하는 경우에는 2를 반환하도록 작성해주세요.

```c
// 여기에 C 코드를 붙여넣어 주세요.
int
my_custom_test(char * s)
{
  // test logic here...
  
  return 0;
}
```

## 🚀 3. 실행 방법 (How to Run)
> 다른 학우들이 이 테스트를 어떻게 실행해 볼 수 있는지 명령어를 적어주세요.

### 예시
1. `user/usertest.c` 에 테스트 코드 함수를 붙여넣고 quicktests 배열에 해당 함수를 "custom_test"로 등록한다.
2. `make qemu` 후 `$ usertests custom_test`로 실행한다.

## 🖥️ 4. 기대 결과 (Expected Output)
> 정상적인(버그가 없는) xv6 커널에서 이 테스트를 실행했을 때의 결과를 묘사해주세요.
> 자주 발생할 수 있을 법한 실패 시나리오가 있다면 같이 묘사해주세요.
