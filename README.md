na máquina remota garantir que tem python 3
instalar se necessário
clonar o repo
instalar e criar venv


meter este ficheiro em etc/systemd/system com
sudo vim etc/systemd/system/daemon.service
ctrl c + v
alterar os path que estão entre <>
sair
sudo systemctl daemon-reload
sudo systemctl start daemon.service
sudo systemctl enable daemon.service
supostamente assim já fica a correr para "sempre", e dá restart automático caso a máquina deslige e ligue outra vez
para manter o daemon atualizado, clonar o repositório e fazer
sudo systemctl restart daemon.service