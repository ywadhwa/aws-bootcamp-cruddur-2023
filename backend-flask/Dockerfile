FROM python:3.10-slim-buster

WORKDIR /backend-flask

COPY . .

RUN pip3 install -r requirements.txt

ENV FLASK_ENV=development
ENV FRONTEND_URL=*
ENV BACKEND_URL=*

EXPOSE ${PORT}
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]