#Use officialy .NET 10.0.X sdk image as the base image
FROM mcr.microsoft.com/devcontainers/dotnet:10.0

# Optional tools and dependencies (git, curl, etc)
# Final command to clean up apt-get cache and reduce image size
RUN apt-get update && apt-get install -y \
    git \
    curl \
    jq \
    && rm -rf /var/lib/apt/lists/*