# Claude Code 이어서 할 일 — GitHub 연결 & Pages 배포

## 위치
- 로컬 폴더: `/Users/nam/Downloads/npley-spep-deck`
- 대상 저장소: https://github.com/UXUI-Test-2/claude-setting
- 원하는 결과: GitHub Pages 공유 URL

## Claude Code에 붙여 넣을 요청
```
/Users/nam/Downloads/npley-spep-deck 폴더는 정적 웹 프레젠테이션이야(index.html + assets/, 빌드 불필요).
이걸 https://github.com/UXUI-Test-2/claude-setting 저장소의 npley-spep-deck/ 하위 폴더로 올려줘.
1) 저장소를 클론하고, 기존 파일은 건드리지 말고 npley-spep-deck/ 폴더로 복사 (README.md, CLAUDE_CODE_HANDOFF.md 포함 가능)
2) 저장소 루트에 .nojekyll 이 없으면 추가
3) main 브랜치에 커밋 후 push
4) GitHub Pages 활성화: gh api -X POST repos/UXUI-Test-2/claude-setting/pages -f "source[branch]=main" -f "source[path]=/"
   (이미 켜져 있으면 건너뜀. 저장소가 private이고 무료 플랜이면 Pages가 안 되니 알려줘)
5) 배포 완료 확인 후 URL 알려줘: https://uxui-test-2.github.io/claude-setting/npley-spep-deck/
```

## 참고
- 경로는 모두 상대경로(`assets/...`)라 하위 폴더에 둬도 그대로 동작
- 별도 저장소로 배포하고 싶으면 폴더 내용을 새 저장소 루트에 두고 Pages를 main / (root)로 설정
- Pages 사이트는 링크를 아는 누구나 열람 가능 (공개 저장소 필요)
