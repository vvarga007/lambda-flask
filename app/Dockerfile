FROM python:3.12-slim

WORKDIR /opt/app

COPY requirements.txt /opt/app/requirements.txt
RUN mkdir -p /opt/app && \
  pip3 install --no-cache-dir -r /opt/app/requirements.txt

COPY . /opt/app

CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0"]
