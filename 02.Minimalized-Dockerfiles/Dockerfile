FROM python:3-slim AS builder

COPY . .

FROM gcr.io/distroless/python3

COPY --from=builder . .

ENTRYPOINT ["CliCalculator.py"]
