# MTD-releases

MTD 데스크탑 앱의 **공개 배포 채널**. 앱 소스는 private(`kwonjiy/MTD`)이고, 여기엔 설치파일과
업데이트 매니페스트(`latest.json`)만 릴리스로 올라간다. 설치된 앱이 이 저장소의 최신 릴리스를 보고 자동 업데이트한다.

## 릴리스하는 법
1. `kwonjiy/MTD`에서 버전 올리고(`src-tauri/tauri.conf.json` + `package.json`) push
2. 여기 **Actions → "Release MTD (desktop)" → Run workflow**

필요한 Secrets(Settings → Secrets and variables → Actions): `MTD_SOURCE_PAT`, `TAURI_SIGNING_PRIVATE_KEY`, `TAURI_SIGNING_PRIVATE_KEY_PASSWORD`(선택), `VITE_SUPABASE_URL`, `VITE_SUPABASE_ANON_KEY`.
