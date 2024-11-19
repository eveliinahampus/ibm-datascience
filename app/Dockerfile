# Use the official Python image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy the requirements file and install dependencies
COPY requirements.txt requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Copy the app code and data
COPY app/ /app/ibm-datascience/app/spacex_dash_app.py
COPY data/ /app/data/

# Expose port 8050 for the Dash app
EXPOSE 8050

# Run the app
CMD ["python3", "app.py"]
