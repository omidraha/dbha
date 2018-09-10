FROM postgres:9.4
RUN apt-get update
RUN apt-get install -y python3-pip  python3-psycopg2
RUN pip3 install --upgrade
RUN apt-get install -y git htop vim curl wget
RUN pip3 install patroni
RUN mkdir -p /home/ws/git/
RUN git clone https://github.com/zalando/patroni
RUN cd patroni && pip3 install -r requirements.txt
USER postgres


#  docker run -it --rm -p5432:5432 -p8008:8008  -v ~/ws/git/patroni:/patroni psp   patroni /patroni/postgres0.yml
# /usr/lib/postgresql/9.4/bin/pg_ctl -D  /var/lib/postgresql/data



