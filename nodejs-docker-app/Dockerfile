# 베이스 이미지 명시
FROM node:10

# 앱 디렉토리 생성
WORKDIR /usr/src/app

# 종속성 캐시 처리 문제로 루트 폴더 파일 복사를 분리
COPY package.json ./

# 추가적으로 필요한 파일들을 다운로드
RUN npm install

# 루트 폴더 파일(server.js)을 docker 컨테이너 내부로 복사
COPY ./ ./

# 컨테이너 시작시 실행될 명령어 명시
CMD ["node", "server.js"]

