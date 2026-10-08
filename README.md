# nhelix drive

내 Tailscale 계정의 컴퓨터 사이에서 파일을 복사하는 데스크톱 앱입니다.

[설치 파일 다운로드](https://github.com/Simon-nhelix/nhelix-drive-releases/releases)

이 저장소는 공개 설치 파일과 업데이트 메타데이터를 배포합니다. 소스 저장소는 별도로 관리합니다.

## 설치

- macOS Apple Silicon: `.dmg`를 열어 앱을 Applications에 설치합니다.
- Linux x64 / SteamOS: `.AppImage`에 실행 권한을 준 뒤 실행합니다.
- alpha.3부터 **공유 및 설정 → 앱 업데이트**에서 다운로드·설치할 수 있습니다. 기존 alpha.2는 최초 한 번 직접 새 앱을 설치해야 합니다.
- 에이전트 단독 설치는 데스크톱 자동 업데이트 대상이 아닙니다.

## macOS에서 "확인할 수 없는 개발자" 경고가 뜰 때

앱이 Apple 공증(notarization)을 받지 않았기 때문에 최초 실행 시 다음과 같은 경고가 뜰 수 있습니다:

> "Apple이 이 소프트웨어에 악성 코드가 있는지 확인할 수 없기 때문에 'nhelix drive'을(가) 열 수 없습니다."

앱에 문제가 있는 것이 아니며, 아래 방법으로 실행할 수 있습니다:

1. 경고 창에서 **완료**를 누릅니다. (**휴지통으로 이동은 누르지 마세요**)
2. **시스템 설정 → 개인정보 보호 및 보안**으로 이동해 맨 아래의 **"그래도 열기"**를 누릅니다.
3. 암호를 입력하면 앱이 실행되고, 이후에는 다시 경고가 뜨지 않습니다.

터미널을 사용하는 경우 다음 한 줄로도 해결됩니다:

```bash
xattr -dr com.apple.quarantine "/Applications/nhelix drive.app"
```

> 참고: macOS 15 Sequoia부터는 예전의 우클릭 → 열기 방식이 더 이상 지원되지 않습니다.

현재는 알파 버전입니다. macOS는 Apple Development 서명이며 공증되지 않았습니다. SteamOS 실기 및 실제 버전 간 앱 교체 검증은 아직 남아 있습니다.
