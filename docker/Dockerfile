FROM python:3.11-alpine

WORKDIR /neighborhood_survey_tool
ADD neighborhood_survey_tool /neighborhood_survey_tool/

COPY requirements.txt .
RUN pip3 install -r requirements.txt

EXPOSE 8000

ENTRYPOINT ["python3"]
CMD ["manage.py", "runserver", "0.0.0.0:8000"]