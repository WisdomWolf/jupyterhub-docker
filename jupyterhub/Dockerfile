FROM jupyterhub/jupyterhub:1.2

COPY jupyterhub_config.py .

RUN apt update && apt install --no-install-recommends -y git

RUN pip install \
    dockerspawner==0.11.1 \
    oauthenticator==0.11 \
    git+https://github.com/jupyterhub/jupyterhub-idle-culler.git@master
