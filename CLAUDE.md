# 숏폼 채널

베이비룸과 관련 없는 개인 숏폼 채널(YouTube Shorts · Instagram Reels · TikTok).
베이비룸 브랜드·저장소·계정과 섞지 않는다.

## 채널 정보 (채워 넣기)

- 채널 이름:
- 콘셉트:
- 말투·톤:
- 기본 해시태그:

## 폴더

- `ideas/` — 기획·대본 (마크다운)
- `posts/YYYY-MM-DD_제목/caption.json` — 플랫폼별 제목·설명·해시태그·공개 범위
- 영상 파일은 git 에 넣지 않는다 → `~/Movies/shorts/raw`(원본), `~/Movies/shorts/final`(완성본)

## 업로드

- 도구: `~/personal/git/.social-tools/` (설정·준비 사항은 그 폴더 README)
- 게시 전에 반드시 제목·설명·공개 범위를 보여 주고 확인받는다.

## Claude 에이전트 (`.claude/agents/`)

- `script-writer` — 주제 → `ideas/` 에 대본(훅 3개·초 단위 대본·촬영 컷)
- `caption-writer` — 대본·영상 → `posts/.../caption.json` (플랫폼별 글자 수 제한 지킴, 기본 비공개)
- `upload-checker` — 올리기 직전 영상·캡션 점검(읽기 전용, ffprobe 있으면 해상도·길이까지)
