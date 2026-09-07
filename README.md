# 바람대로 원고 보드

`board.baramdaero.com`에 배포하는 정적 페이지 한 장.

## 배포 (GitHub Pages)

1. 새 레포 `baramdaero-board` 생성 (Public)
2. 이 폴더의 파일 3개를 루트에 올린다 — `index.html` `CNAME` `robots.txt`
3. Settings > Pages > Source = `main` 브랜치 / `/ (root)`
4. Custom domain 칸에 `board.baramdaero.com` 입력
5. 후이즈 DNS > CNAME 레코드 관리에 추가
       호스트명  board     CNAME  baramdaero.github.io
6. 10~30분 뒤 https://board.baramdaero.com 접속 확인

## 데이터 갱신

현재 원고 데이터는 index.html 안에 박혀 있다. 시트가 바뀌면 다시 빌드해서 index.html만 교체한다.
시트를 실시간으로 읽게 하려면 시트를 "웹에 게시"해야 하는데, 그러면 시트 자체가 공개된다.
접근 제어를 정한 뒤에 결정한다.

## 주의

이 페이지는 공개다. 주소를 아는 사람은 누구나 원고 목록 전체를 볼 수 있다.
robots.txt와 noindex는 검색 노출만 막을 뿐 접근을 막지 않는다.
