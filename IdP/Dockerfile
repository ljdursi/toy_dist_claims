FROM python:3.6-alpine
ADD . /code
WORKDIR /code
RUN apk add build-base \
    && apk add libffi-dev \
    && apk add openssl-dev \
    && pip install -r requirements.txt
EXPOSE 443
CMD ["python3", "src/run.py", "settings.yaml", "-p", "443", "-b", "https://0.0.0.0"]
