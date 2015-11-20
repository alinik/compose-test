FROM alinik/base:latest
RUN apt-get -y install python-setuptools libxml2 libjansson4 libpgm-5.1-0 libpython2.7 libyaml-0-2 libzmq3 && easy_install pip 


ADD . /code
COPY ./wheelhouse /code/wheelhouse
WORKDIR /code
RUN pip install wheelhouse/*
CMD uwsgi --http 0.0.0.0:80  --module app:app
EXPOSE 80
