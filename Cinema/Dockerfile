FROM python:3.12

# Instalar as dependências
RUN apt-get update && apt-get install -y python3-pip

# Definir diretório de trabalho
WORKDIR /app

# Copiar o arquivo de dependências
COPY requirements.txt .

# Instalar as dependências
RUN pip install -r requirements.txt

# Copiar o restante dos arquivos da aplicação
COPY . .

# Definir o comando de execução
CMD ["python", "app.py"]
