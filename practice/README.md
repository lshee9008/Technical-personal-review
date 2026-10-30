# 부족역량 연습 노트북

`부족역량_개념정리.pdf`의 1~6장을 손으로 풀어보는 주피터 노트북이에요.

| 노트북 | PDF | 내용 |
|---|---|---|
| `01_데이터베이스_SQL_MongoDB.ipynb` | 1장 | JOIN·GROUP BY, 인덱스 실행계획/속도, 트랜잭션 롤백, ACID·격리수준, MongoDB 필터 |
| `02_백엔드_서버_Django_Linux_Docker_AWS.ipynb` | 2장 | 상태코드·REST, FastAPI 미니 API, JWT 서명 검증, TTL 캐시, async, N+1, 권한·시그널·리다이렉트, Dockerfile 고치기, AWS |
| `03_데이터분석_pandas_통계_크롤링.ipynb` | 3장 | 결측·중복 정제, groupby·crosstab·merge·resample, 평균/중앙값/p95, A/B 순열검정, BeautifulSoup, JSON API 페이지 수집, robots.txt, 재시도 |
| `04_딥러닝_PyTorch.ipynb` | 4장 | 텐서 shape, 활성화 함수, 손실 직접 계산, 역전파, 경사하강법, ★학습 루프, 과적합·조기 종료, DataLoader, 저장/불러오기, Self-Attention |
| `05_알고리즘_요약.ipynb` | 5장 | 시간복잡도, set/dict, 이분탐색, BFS, 힙 top-k, DP, LRU 캐시 |
| `06_셀프체크_면접질문.ipynb` | 6장 | 랜덤 질문 뽑기 + 14문항 모범 답안 |

## 푸는 법
1. 맨 위 셀(채점 도우미)부터 순서대로 실행해요.
2. `___` 자리를 채우고 실행 → 바로 아래 채점 셀을 실행하면 ✅/❌가 나와요.
3. 막히면 각 문제 아래 `💡 정답 보기`를 열어요. 전체 정답은 `solutions/` 폴더에 있어요.

## 실행 환경 만들기
지금 기본 파이썬(miniconda)은 Intel(x86_64)용이라 PyTorch가 설치되지 않아요. `uv`로 이 폴더에 전용 환경을 만들어요.

```bash
cd practice && uv venv --python 3.12 && uv pip install -r requirements.txt
```

```bash
cd practice && uv run jupyter lab
```

VS Code에서 열 때는 오른쪽 위 커널 선택에서 `practice/.venv`를 고르면 돼요.
