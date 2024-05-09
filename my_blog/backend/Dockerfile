FROM python:3.9
WORKDIR /app
COPY . /app
RUN pip install --no-cache-dir -r requirements.txt
RUN pip install gunicorn
EXPOSE 5000
ENV NAME World
CMD ["gunicorn", "-b", "0.0.0.0:5000", "app:app"]
