FROM python:3

# VOLUME [ "/data" ]
RUN mkdir /src
# RUN mkdir /data
WORKDIR /src
COPY ./src/server.py .
COPY ./src/requirements.txt .
# COPY ./api_to_interact_with_bank_db.py .

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 5000

CMD [ "python", "./server.py" ]