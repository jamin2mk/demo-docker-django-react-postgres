FROM python:3.11.4-slim-buster

WORKDIR /apps/backend

COPY ./apps/backend .

RUN python3 -m venv /opt/venv && \
    /opt/venv/bin/pip install --upgrade pip && \
    /opt/venv/bin/pip install -r requirements.txt && \
    chmod +x /apps/backend/entrypoint.sh

CMD [ "/apps/backend/entrypoint.sh" ]