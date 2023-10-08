# Use an official Ubuntu base image
FROM ubuntu:latest

# Install Git to clone the repository
RUN apt-get update && \
    apt-get install -y git

# Set the working directory inside the container
WORKDIR /app

# Clone the GitHub repository into the container
RUN git clone https://github.com/venku1BM22CS404/DEVELOPER.git

# You can add any other setup or configuration steps here
