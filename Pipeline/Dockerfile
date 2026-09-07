FROM python:3.12-slim
COPY --from=ghcr.io/astral-sh/uv:latest /uv /bin/


# RUN pip install pandas pyarrow
# COPY  

WORKDIR /app
COPY pipeline.py pipeline.py

ENTRYPOINT [ "python", "pipeline.py" ]