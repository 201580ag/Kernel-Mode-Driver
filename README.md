**본 레포지토리는 커널 모드 드라이버 연습을 위해 만들어진 레포지토리입니다.**

# 출처? 배운곳
[Hello World](https://boa9448.tistory.com/31)

# 경고 (Warning)

커널 모드 드라이버를 작성하거나 사용하는 것은 매우 위험할 수 있습니다. 다음 사항을 반드시 숙지하세요:

1. **시스템 불안정**: 잘못된 커널 모드 드라이버는 시스템 충돌, 데이터 손실, 블루 스크린 등의 문제를 일으킬 수 있습니다.
2. **보안 취약점**: 안전하지 않은 코드나 입력 검증 실패는 보안 취약점을 초래할 수 있습니다.
3. **자원 누수**: 메모리 누수, 핸들 누수 등은 시스템 성능 저하 및 불안정을 초래할 수 있습니다.
4. **복구 어려움**: 잘못된 드라이버로 인해 시스템이 부팅되지 않거나 심각한 오류가 발생하면 복구가 어려울 수 있습니다.

### 안전 가이드라인

- **테스트 환경 사용**: 실제 시스템에 배포하기 전에 가상 머신이나 테스트 환경에서 충분히 테스트하세요.
- **코드 검토**: 코드 검토를 통해 잠재적인 문제를 찾고 해결하세요.
- **디버깅 도구 활용**: WinDbg와 같은 커널 디버깅 도구를 사용하여 문제를 추적하고 해결하세요.
- **최신 문서 참조**: 최신 Windows Driver Kit (WDK) 및 공식 문서를 참고하여 작성하세요.

이 프로젝트를 사용하거나 수정하기 전에 위의 경고 사항을 충분히 이해하고 준수하시기 바랍니다. 안전한 개발과 테스트를 통해 시스템의 안정성을 유지하세요.

# **면책 조항(Disclaimer)**
### English
By using this code, the author bears no responsibility for any issues that may arise. The usage of this code is at the user's discretion, and any consequences resulting from it are solely the responsibility of the user. The author assumes no liability for any outcomes or damages incurred from the use of this code. The user absolves the author of any accountability for losses or damages resulting from the usage of this code. By using this code, the user agrees to the following terms and acknowledges being sufficiently warned of any potential risks associated with its use:

1. **Freedom of Use:** The usage of the code is at the user's discretion, and the author imposes no restrictions.
2. **Responsibility:** The user bears sole responsibility for any issues arising from the use of the code.
3. **Consequences of Usage:** The author disclaims all responsibility for any outcomes resulting from the use of the code.
4. **Liability Waiver:** The user holds the author harmless from any losses or damages resulting from the usage of the code.

### Korean
이 코드를 사용함으로써 발생하는 어떤 문제에도, 작성자는 일체의 책임을 지지 않습니다. 코드를 사용하는 것은 사용자의 자유이며, 이로 인해 발생하는 모든 문제에 대한 책임은 오로지 사용자에게 있습니다. 이 코드를 사용함으로써 발생하는 어떠한 결과에도 작성자는 일체의 책임을 지지 않으며, 이 코드를 사용함으로써 발생하는 어떠한 손실이나 손해에 대해 사용자는 작성자를 책임 지지 않습니다. 이 코드를 사용함으로써 사용자는 다음 사항에 동의하며, 이 코드를 사용함으로써 발생할 수 있는 모든 위험에 대해 충분히 경고받았음을 인지해야 합니다:

1. **자유로운 사용**: 코드를 사용하는 것은 사용자의 자유이며, 작성자는 사용 제약을 가하지 않습니다.
2. **책임의 귀속**: 코드 사용으로 발생하는 모든 문제에 대한 책임은 오로지 사용자에게 있습니다.
3. **코드 사용의 결과**: 작성자는 코드 사용으로 발생하는 모든 결과에 대해 일체의 책임을 지지 않습니다.
4. **손실 또는 손해에 대한 면책**: 사용자는 코드 사용으로 발생하는 어떠한 손실이나 손해에 대해 작성자를 책임 지지 않습니다.
