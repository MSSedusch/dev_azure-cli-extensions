FROM mcr.microsoft.com/devcontainers/python:1-3.12-bullseye
USER vscode
ENV VIRTUAL_ENV=/home/vscode/venv
RUN python3 -m venv $VIRTUAL_ENV
ENV PATH="$VIRTUAL_ENV/bin:$PATH"

# Install dependencies:
RUN pip install azdev azure.cli
RUN azdev setup -r /workspaces/dev_azure-cli-extensions/azure-cli-extensions