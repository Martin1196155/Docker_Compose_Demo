FROM python:3.7-alpine
Maintainer martinbrightin1@gmail.com
WORKDIR /code
ENV FLASK_APP Python-app/app.py
ENV FLASK_RUN_HOST 0.0.0.0
RUN apk add --no-cache gcc musl-dev linux-headers
COPY Python-app/requirements.txt requirements.txt
RUN pip install -r requirements.txt
COPY . .
CMD ["flask", "run"]
