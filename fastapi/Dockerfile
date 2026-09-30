# Use python:3.13-slim as a base image 
FROM python:3.13-slim

# Set /Day8 as a working directory in the container
WORKDIR /homework3

# Copy everything in the working directory to /Day8 in the container
COPY * ./

# Install packages and libraries
RUN pip install -r requirements.txt

# expose port 8000
EXPOSE 8000

# run the extract_save_data.py as fastapi server.
CMD ["fastapi", "run", "extract_save_data.py", "--port=8000"]