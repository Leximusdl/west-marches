FROM python:3-slim

WORKDIR /opt/wm-manager-api

RUN apt update && apt install -y gcc libev-dev

COPY requirements.txt ./

RUN pip install --no-cache-dir -r requirements.txt

COPY src ./

CMD ["python", "./__main__.py"]
