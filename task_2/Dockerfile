FROM python:3.6
WORKDIR /usr/src/backend
COPY . .
RUN pip install -r requirements.txt
RUN echo "python manage.py migrate; exec python manage.py runserver 0:8000" > /start.sh
RUN chmod +x /start.sh
EXPOSE 8000
ENTRYPOINT exec /start.sh
