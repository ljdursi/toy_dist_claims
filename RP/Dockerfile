FROM python:3.6-alpine
ADD . /code
WORKDIR /code
RUN pip install -r requirements.txt
EXPOSE 8000
CMD ["python3", "src/rp.py", "settings.yaml", "-p 8000"]
