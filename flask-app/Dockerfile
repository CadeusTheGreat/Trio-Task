#Use Python Image
FROM python:3.7
# Install apt dependencies
RUN apt-get update && apt-get install -y python3-pip
# Run pip dependencies
RUN pip3 install flask flask_sqlalchemy
# Copy contents into image
COPY app.py .
# Expose correct port
EXPOSE 5000
# Create an entrypoint
ENTRYPOINT ["python", "app.py"]
