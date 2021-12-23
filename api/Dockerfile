FROM python:3.7

LABEL maintainer="René Mifsud"
LABEL description="Red Acre Devops Test"

RUN mkdir /backend

WORKDIR /backend
COPY requirements.txt /backend/requirements.txt

ENV PYTHONDONTWRITEBYTECODE="1"


RUN pip install --upgrade pip && \
    pip install -r requirements.txt

COPY . .

ENTRYPOINT [ "flask", "run", "--host=0.0.0.0" ]