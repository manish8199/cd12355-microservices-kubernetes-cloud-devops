FROM public.ecr.aws/docker/library/python:3.10-alpine

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app/analytics/

ENV DB_USERNAME=mjuser
ENV DB_PASSWORD=mjpassword
ENV DB_HOST=127.0.0.1
ENV DB_PORT=5433
ENV DB_NAME=mjdatabase

# Install any needed dependencies specified in requirements.txt
RUN pip install --no-cache-dir -r /app/analytics/requirements.txt

# Make port 5153 available to the world outside this container
EXPOSE 5153

# Run app.py when the container launches
CMD ["python", "analytics/app.py"]
