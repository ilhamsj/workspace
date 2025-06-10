FROM ubuntu:latest

# Set environment variables to noninteractive
ENV DEBIAN_FRONTEND=noninteractive

# Update and install basic tools
RUN apt-get update && apt-get install -y \
    curl \
    wget \
    git \
    unzip \
    software-properties-common \
    ca-certificates \
    lsb-release \
    gnupg \
    build-essential \
    vim

# --- Install PHP ---
RUN apt-get install -y php php-cli php-mbstring php-xml php-curl php-mysql

# --- Install Node.js (LTS version) ---
RUN curl -fsSL https://deb.nodesource.com/setup_22.x | bash - && \
    apt-get install -y nodejs

# Working directory
WORKDIR /opt/workspace

# Default command
CMD [ "bash" ]
