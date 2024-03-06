FROM python:3.11.1

WORKDIR /app

COPY . /app

RUN pip install --no-cache-dir --upgrade pip

RUN pip install --no-cache-dir -r requirements.txt

RUN pip install pylint

RUN pylint $(find . -name '*.py')

RUN pip install requests

EXPOSE 5000

ENV NAME python

CMD ["python","main.py"]