# 공식 MySQL 이미지 사용
FROM mysql:latest

# 환경 변수 설정
ENV MYSQL_ROOT_PASSWORD=1234
ENV MYSQL_DATABASE=moheng
ENV MYSQL_USER=moheng_user
ENV MYSQL_PASSWORD=1234

# 초기화 SQL 스크립트 복사
COPY init.sql /docker-entrypoint-initdb.d/

# MySQL 포트 노출
EXPOSE 3306

# 컨테이너 시작 시 실행할 명령어
CMD ["mysqld"]
