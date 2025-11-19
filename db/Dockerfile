FROM ubuntu
RUN apt-get update
RUN apt-get install -y sqlite3
COPY words.sql /
CMD ["sh", "-c", "sqlite3 -echo /words.db < words.sql"]

