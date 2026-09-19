# FlickWheel 릴리즈

After Effects용 우클릭 홀드 방사형 메뉴 **FlickWheel**(macOS)의 배포 저장소입니다.
소스 코드는 비공개이며, 이 저장소에는 배포 파일과 최신 버전 정보(`latest-mac.yml`)만 있습니다.

## 설치

1. [Releases](https://github.com/thoven-jun/flickwheel-releases/releases/latest)에서 `FlickWheel-<버전>-mac.zip`을 내려받아 압축을 풉니다.
2. 압축을 푼 폴더에서 **Click Me to Fix.command**를 더블클릭합니다. 격리 속성을 풀고 `/Applications`에 설치한 뒤 앱을 실행합니다.
3. 접근성 권한 창이 뜨면 시스템 설정 › 개인정보 보호 및 보안 › 손쉬운 사용에서 FlickWheel을 켭니다.
4. After Effects에서 우클릭을 길게 누르면 휠이 열립니다.

FlickWheel은 Apple 개발자 인증서가 아닌 자체 서명을 사용하므로 macOS가 "손상되었다"고 표시할 수 있습니다. 설치 스크립트가 이를 해결합니다.

## 요구 사항

- macOS 14 이상
- Adobe After Effects

## 업데이트

앱이 이 저장소의 `latest-mac.yml`을 읽어 새 버전이 있으면 메뉴막대에서 안내합니다. 자동 설치는 하지 않으며, 위 설치 과정을 다시 진행하면 됩니다.
