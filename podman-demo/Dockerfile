FROM alpine:latest

# Install a package
RUN apk add --no-cache figlet

# Create an app directory
WORKDIR /app

# Create a script file
RUN echo '#!/bin/sh' > /app/hello.sh && \
    echo 'figlet "Hello, $1!"' >> /app/hello.sh && \
    chmod +x /app/hello.sh

# Run our script
ENTRYPOINT ["/app/hello.sh"]
CMD ["Podman"]
