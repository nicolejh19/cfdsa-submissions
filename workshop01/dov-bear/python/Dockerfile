FROM python:3.11.5

WORKDIR /python

COPY . .

RUN pip install pip
RUN pip install -r requirements.txt

ENV PORT=3000
ENV INSTANCE_NAME=dov-bear
ENV INSTANCE_HASH=888

# if env variable changes, then this line changes too
EXPOSE ${PORT}

CMD ["sh", "run.sh"]