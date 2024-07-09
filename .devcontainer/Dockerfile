# .devcontainer/Dockerfile
FROM python:3.9-slim

# 環境変数を設定
ENV PYTHONDONTWRITEBYTECODE=1 \
    PYTHONUNBUFFERED=1

# 作業ディレクトリを設定
WORKDIR /app

# 必要なパッケージをインストール
COPY requirements.txt /app/
RUN pip install --no-cache-dir -r requirements.txt

# アプリケーションのコードをコピー
COPY . /app