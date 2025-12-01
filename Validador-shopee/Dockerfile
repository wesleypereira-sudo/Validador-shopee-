# Imagem base do Python
FROM python:3.10

# Criar pasta de trabalho
WORKDIR /app

# Copiar arquivos do projeto
COPY . /app

# Instalar dependências
RUN pip install --no-cache-dir -r requirements.txt

# Expor porta usada pelo Streamlit
EXPOSE 8501

# Rodar Streamlit
CMD ["streamlit", "run", "app.py", "--server.port=8501", "--server.address=0.0.0.0"]
