# 베이스 이미지 명시
FROM node:10

# 루트 폴더 파일(package.json, server.js)을 docker 컨테이너 내부로 복사
COPY ./ ./

# 추가적으로 필요한 파일들을 다운로드
RUN npm install

# 컨테이너 시작시 실행될 명령어 명시
CMD ["node", "server.js"]
