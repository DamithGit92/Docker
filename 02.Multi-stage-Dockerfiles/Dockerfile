FROM python:3.10 AS builder

RUN pip install pyinstaller && pip install --upgrade pip

COPY CliCalculator.py .

FROM python:3.10-slim

COPY --from=builder CliCalculator.py .

CMD ["python", "CliCalculator.py"]
