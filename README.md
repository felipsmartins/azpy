# azpy

Esse repositório é apenas um teste de como usar o S3 como package index privado 
para pacotes python, em resumo: um pypi privado seguindo a estrutura do PEP 503.

--- 

Exemplo de instalação de um pacote de fonte privada:

```bash
export EXTRA_INDEX=private-pypi.s3-website-us-east-1.amazonaws.com
python2 -m pip install --force-reinstall --extra-index-url http://$EXTRA_INDEX azpy==0.1.0 --trusted-host $EXTRA_INDEX
python3 -m pip install --force-reinstall --extra-index-url http://$EXTRA_INDEX azpy==0.1.0 --trusted-host $EXTRA_INDEX

```