FROM python:3.13-slim
WORKDIR /code
COPY requirements.txt ./
COPY requirements.lock ./
COPY pyproject.toml ./
RUN pip install uv && uv pip install --system -r requirements.txt
COPY . .
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000", "--reload"]
