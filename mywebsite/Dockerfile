FROM python:latest
WORKDIR /app
COPY . /app
RUN pip install --no-cache-dir -r requirements.txt
EXPOSE 5000
# Define environment variable
ENV NAME World
CMD ["gunicorn", "-w 4", "-b :5000", "app:app"]
