FROM python:3
EXPOSE 5000
RUN apt-get update -y && apt-get install -y git postgresql libpq-dev
RUN git clone https://github.com/Lukxsx/PakastimenHallinta.git
WORKDIR /PakastimenHallinta
RUN pip3 install --upgrade pip
RUN pip3 install --no-cache-dir -r requirements.txt
CMD [ "python3", "./run.py" ]
