<!--
  공개 저장소 thoven-jun/flickwheel-releases의 README.md 교체 초안.
  메인 세션이 검토 후 그 저장소에 직접 게시한다. macOS 섹션 텍스트는 기존 README를 그대로 옮겼다.
-->

# FlickWheel 릴리즈

After Effects용 우클릭 홀드 방사형 메뉴 **FlickWheel**(macOS / Windows)의 배포 저장소입니다.
소스 코드는 비공개이며, 이 저장소에는 배포 파일과 최신 버전 정보(`latest-mac.yml`, `latest-win.yml`)만
있습니다.

## macOS

### 설치

1. [릴리즈 페이지](https://github.com/thoven-jun/flickwheel-releases/releases/latest)에서
   `FlickWheel-x.y.z-mac.zip`을 내려받는다.
2. 압축을 푼다.
3. 압축을 푼 폴더의 **"Click Me to Fix.command"**를 더블클릭한다.
   - 격리 속성(xattr)을 제거하고, `/Applications`에 설치한 뒤 앱을 실행한다.
4. **시스템 설정 → 개인정보 보호 및 보안 → 손쉬운 사용**에서 FlickWheel을 켠다.
   - 스크립트가 해당 설정 화면을 자동으로 열어준다.
   - 이 권한이 없으면 우클릭 인터셉트와 전역 단축키가 전혀 동작하지 않는다.

### 요구 사항

- macOS 14 이상
- After Effects (전면 앱일 때만 우클릭 인터셉트가 동작)

### 업데이트

새 버전이 나오면 24시간마다 자동으로 확인하고, 상태바 메뉴 맨 위에 안내 항목이 뜨며
처음 발견 시 토스트로 한 번 알려준다. **자동 설치는 하지 않는다** — 안내만 하고,
클릭하면 이 릴리즈 페이지로 이동한다.

## Windows

### 설치

1. [릴리즈 페이지](https://github.com/thoven-jun/flickwheel-releases/releases)에서
   `FlickWheel-x.y.z-win-x64.zip`을 내려받는다.
   - Windows 릴리즈는 태그가 `vx.y.z-win`이다. 페이지 상단의 "Latest"는 macOS 릴리즈용이므로,
     전체 릴리즈 목록에서 원하는 Windows 버전을 찾는다.
2. 압축을 푼다.
3. 압축을 푼 폴더의 **FlickWheel.exe**를 더블클릭한다.
4. Windows가 "Windows의 PC 보호(SmartScreen)" 경고를 띄우면 **추가 정보 → 실행**을 누른다.
   - 코드 서명 인증서가 없어서 뜨는 정상적인 경고다.
5. 처음 실행하면 뜨는 창에서 **설치** 버튼을 눌러 내 PC에 설치한다.
6. After Effects **편집 → 환경설정 → 스크립팅 및 표현식**에서
   **"스크립트가 파일을 쓰고 네트워크에 접근하도록 허용"**을 켠다.

### 사용 방법

- After Effects를 앞에 두고 **우클릭을 길게 누르면** 커서 위치에 휠이 뜹니다.
- 마우스를 원하는 방향으로 옮겨 카테고리를 고르고, 이어서 세부 툴 위에서 버튼을 떼면 실행됩니다.
- 짧게 눌렀다 놓으면 After Effects의 원래 우클릭 메뉴가 그대로 뜹니다.
- 전역 단축키(기본 Ctrl+Alt+Space)로도 휠을 열 수 있고, Esc로 취소합니다.
- 작업 표시줄 트레이의 FlickWheel 아이콘 메뉴:
  - **설정…**: 홀드 시간·트리거·단축키·휠 크기, 로그인 시 자동 실행, 휠 편집기(카테고리·툴 드래그 편집), 프리셋, 정보(버전·업데이트).
  - **이펙트 목록 새로고침**: 설치된 이펙트를 다시 읽어 휠 편집기에서 고를 수 있게 합니다.
  - **AE 확장 다시 설치**: 휠은 뜨는데 액션이 실행되지 않을 때 누릅니다.
  - **업데이트 확인**, **로그 열기**.
- After Effects 안에 "FlickWheel"이라는 작은 패널이 열립니다. 앱과 After Effects를 잇는 연결 창이므로 닫아도 되지만, 닫으면 다음에 After Effects가 앞으로 올 때 자동으로 다시 열립니다.

### 요구 사항

- Windows 10/11 x64 (ARM64 미지원)
- After Effects 2024 이상 (AE 2026 한국어 UI에서 테스트됨)

### 업데이트

앱이 백그라운드에서 주기적으로 새 버전을 확인해 트레이 메뉴/토스트로 알리고,
zip을 내려받아 무결성을 확인한 뒤 자동으로 교체·재시작한다.
