# 한글 수식 도우미

광장(Portal) **원안 생성**의 「＋ 수식」을 누르면 이 PC에 설치된 **한글(한컴오피스)의 수식 편집기**가 뜨게 해 주는 작은 Windows 프로그램입니다. 수식을 쓰고 한글에서 하던 대로 **Shift+Esc**로 닫으면 결과가 원안의 수식 블록에 들어갑니다.

## 설치 (PC마다 한 번)

1. [hwp-equation-helper.exe 받기](https://github.com/puroome/hwp-equation-helper/releases/latest/download/hwp-equation-helper.exe)
2. 받은 파일을 **한 번 실행**합니다.
   - 서명이 없는 프로그램이라 브라우저나 Windows가 경고할 수 있습니다. "Windows의 PC 보호" 창에서는 `추가 정보 → 실행`을 누릅니다.
   - "설치했습니다" 창이 뜨면 끝입니다. 받은 파일은 지워도 됩니다.
3. 광장으로 돌아가 「＋ 수식」을 다시 누릅니다.

필요한 것: Windows, 한컴오피스 한글.

## 하는 일

- 자신을 `%LOCALAPPDATA%\hwp-equation-helper\`에 복사하고 시작 프로그램에 등록해, PC를 켤 때마다 조용히 실행됩니다.
- 이 PC 안(`127.0.0.1:48720`)에서만 듣고, 광장 주소에서 온 요청만 받습니다. 인터넷으로 아무것도 보내지 않습니다.
- 요청이 오면 한글을 따로 하나 띄워 수식 편집기를 열고, 닫히면 수식 스크립트와 크기를 돌려줍니다. 열어 둔 한글 문서는 건드리지 않습니다.
- 기록은 `%LOCALAPPDATA%\hwp-equation-helper\helper.log`에 남으며 수식 내용은 적지 않습니다.

## 업데이트

새 파일을 받아 한 번 실행하면 켜져 있던 도우미를 끄고 새 것으로 바꿉니다.

## 삭제

1. `Win+R` → `shell:startup` → `한글수식도우미` 바로가기 삭제
2. 작업 관리자에서 `한글수식도우미` 끝내기
3. `%LOCALAPPDATA%\hwp-equation-helper` 폴더 삭제
