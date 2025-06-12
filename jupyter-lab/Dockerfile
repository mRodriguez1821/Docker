FROM jupyter/base-notebook:latest

# Puerto para JupyterLab
EXPOSE 8182

# Contraseña: Pasterilo123 (hash generado con notebook.auth.passwd)
ENV JUPYTER_PASSWORD="argon2:$argon2id$v=19$m=10240,t=10,p=8$iq00jEUXkgTYEYksIHdeRw$1rGdA66cQqjPxJQM1RGzvrww3xwfgKakIfmDHnX+jyM"

# Comando de inicio
CMD ["jupyter", "lab", "--ip=0.0.0.0", "--port=8182", "--no-browser", "--NotebookApp.password=argon2:$argon2id$v=19$m=10240,t=10,p=8$iq00jEUXkgTYEYksIHdeRw$1rGdA66cQqjPxJQM1RGzvrww3xwfgKakIfmDHnX+jyM", "--NotebookApp.token=''", "--allow-root"]
