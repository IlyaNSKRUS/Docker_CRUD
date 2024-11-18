FROM python:3.12.3-alpine

WORKDIR /src

COPY ./requirements.txt ./requirements.txt
RUN pip3 install --upgrade pip && pip3 install --no-cache-dir --upgrade -r requirements.txt	

COPY . .	
ENV MY_ENV=crud_18_11_24	

EXPOSE 5050
	
CMD ["python3", "manage.py", "runserver", "0.0.0.0:5050"]
