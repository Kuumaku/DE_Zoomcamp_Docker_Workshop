FROM python:3.12-slim
COPY --from=ghcr.io/astral-sh/uv:latest /uv /bin/


# RUN pip install pandas pyarrow
WORKDIR /app
COPY  pyproject.toml .python-version uv.lock ./
RUN uv sync --locked --no-install-project
ENV PATH='/app/.venv/bin:$PATH'

COPY pipeline.py .

ENTRYPOINT ["python", "pipeline.py" ]