# Use the base image
FROM mcr.microsoft.com/devcontainers/python:1-3.11-bullseye

# Switch to root to perform installation
USER root

# Copy the requirements file into the image
COPY requirements.txt /tmp/requirements.txt

# Install the requirements
RUN pip install -r /tmp/requirements.txt

# Clean up
RUN rm /tmp/requirements.txt

# Switch back to the default non-root user
USER vscode