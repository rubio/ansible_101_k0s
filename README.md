# README

```
git clone git@github:rubio/ansible_101_k0s.git
cd ansible_101_k0s
docker run -ti \
   --mount type=bind,source=/var/run/docker.sock \
   --mount type=bind,source=$PWD/,target=/src \
   python:3.8.8 bash
```
o 
```
docker run -ti --mount type=bind,source=/var/run/docker.sock,target=/var/run/docker.sock python:3.8.8 bash
git clone https://github.com/rubio/ansible_101_k0s.git
```


Con el primero, tendrás el repositorio clonado en tu equipo y con el segundo una vez acabes, no tendrás nada, sólo los contenedores creados, si no los has destruido antes.


Instalamos pipen y ansible

python -m pip install --user pipenv
pipenv install
ansible-galaxy install -r requirements.yaml

