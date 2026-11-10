# Este arquivo vai preparar o ambiente Linux dentro do container com o Java 21, Maven e o Ollama.

FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

RUN apt-get update && apt-get install -y \
    openjdk-21-jdk \
    maven \
    curl \
    zstd \
    && rm -rf /var/lib/apt/lists/*

# Ajuste para o caminho exato que aparecer no ls -1 /usr/lib/jvm/ (caso utilize arquitetura x86_64/amd64, altere para java-21-openjdk-amd64)
ENV JAVA_HOME=/usr/lib/jvm/java-21-openjdk-arm64
ENV PATH="${JAVA_HOME}/bin:${PATH}"

# Instalar o Ollama
#RUN curl -fsSL https://ollama.com/install.sh | sh

# Expor a porta padrão do Ollama
#EXPOSE 11434