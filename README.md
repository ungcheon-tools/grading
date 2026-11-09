# 수행평가 채점 도우미

웅천고 교사용 수행평가 AI 채점 도우미(웹앱).

- 이 저장소에는 **앱과 채점기준만** 있고 학생 개인정보는 없다.
- API 키·학생 명단·채점 결과는 접속한 PC의 브라우저에만 저장되고, 2026-12-25 에 모두 지워진다.
- 학생 명단은 교내로 전달된 「명단 열기」 파일로 PC마다 한 번 연결한다.

## 만드는 법·배포법

- 원본은 비공개 저장소(ungcheon-grading-tool)다. 거기서 `make_seed.py` 가 학생 정보 없는 링크판 `web/index.html` 을 만든다(학생 정보 0줄인지 스스로 검사).
- 그 파일을 이 저장소(로컬 `클로드/grading-web`)의 `index.html` 로 복사 → `git pull --rebase` → 커밋 → `git push` 하면 GitHub Pages(가지 `main`, 폴더 `/`)가 1~2분 뒤 https://ungcheon-tools.github.io/grading/ 에 반영한다.
- 여기서 `index.html` 을 직접 고치지 않는다(다음 빌드 때 덮어써진다). 공개 저장소이므로 학생 명단·API 키를 넣지 않는다.
