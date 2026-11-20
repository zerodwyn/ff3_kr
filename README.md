# [FC] 파이널 판타지3 한글패치

패미콤 **파이널 판타지3** 한글패치입니다. 패미콤 실기에서 구동하는 것을 목표로 작업했습니다.

- 블로그 소개글: https://dwyn.tistory.com/4
- 최신 버전 다운로드: [Releases](../../releases/latest)
- 버그 제보: [Issues → 버그 제보](../../issues/new/choose)
- 후원: https://litt.ly/dwyn

## 작업 사항 및 변경 이력

주요 작업 사항, 추가 기능, 변경 이력 등 자세한 내용은 **[블로그](https://dwyn.tistory.com/4)** 글을 참조해 주세요.

본 한글패치의 정보를 공유하실 때는 블로그 패치 글로 링크를 걸어 주세요.

## 적용 방법

1. [Releases](../../releases/latest)에서 패치 파일을 받습니다.
2. 직접 가지고 계신 원본 ROM에 패치를 적용합니다.
   - 웹에서 적용: [ROM Patcher JS](https://www.marcrobledo.com/RomPatcher.js/)
   - PC 프로그램: Delta Patcher, Floating IPS 등
3. 패치된 ROM을 에뮬레이터나 플래시카트로 실행합니다.

### 체크섬 확인

패치는 **iNES 헤더(16바이트)가 붙은 일본판 원본 ROM**(524,304바이트)에 적용해야 합니다.

| 구분 | CRC32 | MD5 | SHA1 |
|---|---|---|---|
| 원본 ROM (일본판) | `170163F1` | `4E9BDCDD1071FF48638A3AA0FDA325FC` | `C4443FC24625E3C2BB859525EB44B6B3A80E7C35` |
| 패치 후 (v1.2, 524,304바이트) | `8AD68EEF` | `059CD341DFFFD0352ED680ECABA0A74D` | `CC2D8DD6FEF30DA22DC858318973E416547FA39E` |

- ROM Patcher JS에 ROM 파일을 넣으면 CRC32, MD5, SHA1이 바로 표시됩니다.
- 크기가 같아도 헤더 내용이 다르면 체크섬이 다르게 나오고 패치가 적용되지 않습니다. 이때는 헤더를 제외한 CRC32가 `57E220D0`인지 확인해 보세요.

> 이 저장소에는 패치 파일만 있습니다. ROM 파일이나 패치를 적용한 ROM은 배포하지 않으며, 요청에도 응하지 않습니다.
