FROM mcr.microsoft.com/devcontainers/python:1-3.13-bookworm

RUN sudo rm -f /etc/apt/sources.list.d/yarn.list \
    && sudo apt-get update \
    && sudo apt-get install -y jq \
    && sudo rm -rf /var/lib/apt/lists/*


USER vscode

#Install UV
RUN curl -LsSf https://astral.sh/uv/install.sh | sh 
ENV PATH="/home/vscode/.local/bin:${PATH}"