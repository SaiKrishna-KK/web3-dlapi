FROM tiangolo/uvicorn-gunicorn-fastapi:python3.9

WORKDIR /tensorflow_folder

COPY requirements.txt /code/requirements.txt
RUN pip3 install --no-cache-dir --upgrade -r /code/requirements.txt

COPY ./lumos_hack code/lumos_hack

EXPOSE 80

CMD [ "python", "app.py" ]