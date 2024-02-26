# syntax=docker/dockerfile:1.4
FROM python:3.11-slim
WORKDIR /app
ENV COGNITIO_POOL_ID=us-east-1_PEK81ibt2
ENV COGNITIO_APP_CLIENT_ID=43qbsgia2u5o7a68jp75klere4
COPY requirements.txt ./requirements.txt
RUN pip3 install -r requirements.txt
EXPOSE 8501
COPY . .
ENTRYPOINT ["streamlit", "run", "Home.py", "--server.port=8501", "--server.address=0.0.0.0"]
