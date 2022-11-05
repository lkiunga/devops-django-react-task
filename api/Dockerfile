FROM python:3.9.5-alpine
WORKDIR /api
# set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1
# Install dependencies
RUN pip install --upgrade pip
COPY ./requirements.txt /api/
RUN  pip install -r requirements.txt

# Copy project
COPY . .

EXPOSE 8000

CMD ["python", "manage.py","runserver"]
