# Usando uma imagem base com Python
FROM python:3.9

# Definir o diretório de trabalho
WORKDIR /app

# Copiar o arquivo requirements.txt para dentro do container
COPY requirements.txt .

# Instalar as dependências
RUN pip install -r requirements.txt

# Copiar o restante dos arquivos da aplicação
COPY . .

# Definir a porta que o container vai expor
EXPOSE 5000

# Comando para iniciar a aplicação
CMD ["python", "app.py"]
