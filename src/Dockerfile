FROM python:3.8.20
WORKDIR /app
COPY ./requirements.txt /app/
RUN pip install --no-cache-dir -r requirements.txt

COPY . /app
EXPOSE 5000
RUN chmod +x entrypoint.sh
ENTRYPOINT [ "/app/entrypoint.sh" ]