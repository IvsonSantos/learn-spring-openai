
# Este arquivo vai preparar o ambiente Linux dentro do container com o Java, Maven e o Ollama.

FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

RUN apt-get update && apt-get install -y \
    openjdk-17-jdk \
    maven \
    curl \
    zstd \
    && rm -rf /var/lib/apt/lists/*

# Ajuste para o caminho exato que aparecer no ls -1 /usr/lib/jvm/
ENV JAVA_HOME=/usr/lib/jvm/java-17-openjdk-arm64
ENV PATH="${JAVA_HOME}/bin:${PATH}"

# Instalar o Ollama
#RUN curl -fsSL https://ollama.com/install.sh | sh

# Expor a porta padrão do Ollama
#EXPOSE 11434



