# Usar a imagem oficial do Python 3.12
FROM python:3.12.7

# Definir o diretório de trabalho dentro do container
WORKDIR /app

# Copiar todos os arquivos da aplicação para o diretório de trabalho no container
COPY . /app

# Instalar as dependências a partir do arquivo requirements.txt
RUN pip install --no-cache-dir -r Cinema/requirements.txt

# Expor a porta em que o Flask vai rodar
EXPOSE 5000

# Definir o comando para rodar o servidor Gunicorn
CMD ["gunicorn", "Cinema.app:app"]
