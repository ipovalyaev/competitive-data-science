FROM ubuntu

RUN apt-get update && apt-get install --no-install-recommends -y libpq-dev build-essential curl wget git python3-pip python3-setuptools python3-dev\
 && apt-get clean && rm -rf /var/lib/apt/lists/*

##
RUN cd /usr/local && ln -s /usr/bin/python3 /usr/bin/python
COPY requirements.txt /tmp/
RUN  python3 -m pip install --upgrade pip==19.3.1 && pip3 install -r /tmp/requirements.txt

