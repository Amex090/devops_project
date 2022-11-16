FROM python:3.10
EXPOSE 8501
WORKDIR /app
COPY  ./streamlit/requirements.txt ./requirements.txt
RUN pip3 install -r requirements.txt
COPY ./streamlit/interface.py .
CMD ["streamlit", "run", "interface.py"]
