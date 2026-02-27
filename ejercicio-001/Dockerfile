FROM ubuntu:22.04

RUN apt update && apt install -y \
    build-essential \
    valgrind \
    make

WORKDIR /app
COPY . .

CMD ["bash"]