FROM python:3.12-slim
# COPY --from=ghcr.io/astral-sh/us:latest /us /bin/


# RUN pip install pandas pyarrow
# COPY  

WORKDIR /code
COPY pipeline.py .

ENTRYPOINT [ "python", "pipeline.py" ]