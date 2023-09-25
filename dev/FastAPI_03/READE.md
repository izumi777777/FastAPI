# メモ  ※ 編集中  

## 公式ドキュメント 

https://fastapi.tiangolo.com/ja/

## 1.ローカル環境の場合は先に以下のコマンドを実行しライブラリをインストールする。  
※ 仮想環境をアクティベート後に仮想環境ディレクトリ内で実行しても良い。  
```sh
pip install -r requirements.txt　（ぴっぴ　インストール　オプションr レクァイエムンツ）
```  

## 2.FastAPI基本ディレクトリ構造  

```sh
.
├── Dockerfile
├── app
│   ├── __pycache__
│   │   └── main.cpython-311.pyc
│   └── main.py
└── requirements.txt

```

## 3.OpenAPI表示方法

```
http://localhost:ポート/docs#/

```  

## 4.FastAPIの基本のDockerfile  
```txt
FROM tiangolo/uvicorn-gunicorn-fastapi:python3.9-slim

COPY ./app /app
```



## 5.コンテナの稼働状態を5秒おきに確認  

```sh  
watch -n 0.5 -d docker ps
```