FROM debian:bullseye-slim

RUN apt update -y

# Install git, curl, bash and unzip
RUN apt install \ 
    git     \
    curl    \
    bash    \
    unzip -y

# Install Bun
RUN curl -fsSL https://bun.sh/install | bash

# Set path
RUN export BUN_INSTALL="/home/YOUR_USERNAME/.bun"
RUN export PATH="$BUN_INSTALL/bin:$PATH"

# Expose port 10073
EXPOSE 10073

# Start bash
CMD ["/bin/bash"]
