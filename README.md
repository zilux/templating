copy vimrc to ~/.vimrc

mkdir playbooks

cp yamllint-config playbooks/.yamllint

yamllint playbooks/xxx.yml
ansible-lint playbooks/xxx.yml



PRE-COMMIT
==========

python3.8 -m venv venv
source venv/bin/activate

pip install pre-commit

pip install --upgrade pip

mkdir mygit; cd mygit ; git init

cd /tmp
git clone https://github.com/zilux/templating.git

cd -

git cp /tmp/templating/pre-commit-config.yaml .

pre-commit install

> x.yaml

pre-commit run --all-files
