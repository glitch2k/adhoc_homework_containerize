FROM nginx

# VOLUME [ "/data" ]
# RUN mkdir /src
# RUN mkdir /data
# WORKDIR /src
COPY ./nginx.conf /etc/nginx/conf.d/
COPY requirements.txt .
# COPY ./api_to_interact_with_bank_db.py .

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 5000

CMD [ "python", "./server.py" ]