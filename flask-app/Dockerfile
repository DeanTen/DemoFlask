# we are using Python, labelled as version 3.7
FROM python:3.7
#set the working directory
WORKDIR /usr/src/app
# copy from . which means current directory to . or /usr/src/app
COPY . . 
# pip install is a python shell, --no-cache-dir means no caching and we are running the file requirements.txt
RUN pip install --no-cache-dir -r requirements.txt
# expose port 5000 which is in the app.py
EXPOSE 5000
# add an entrypoint or use cmd in comments below
ENTRYPOINT [ "python" ]
# run app.py using python
#CMD ["python", "./app.py"]
CMD ["./app.py"]