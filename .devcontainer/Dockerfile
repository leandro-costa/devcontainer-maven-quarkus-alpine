FROM maven:3.9.4-eclipse-temurin-20-alpine
RUN apk add --no-cache bash curl git zip && \
  curl -s "https://get.sdkman.io" | bash
RUN bash -c "source $HOME/.sdkman/bin/sdkman-init.sh && sdk install quarkus"
RUN sed -i 's,/bin/ash,/bin/bash,' /etc/passwd
