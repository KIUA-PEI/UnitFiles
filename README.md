meter este ficheiro em etc/systemd/system com
com 
'''
sudo vim etc/systemd/system/daemon.service
'''

ctrl c + v

sudo systemctl daemon-reload

sudo systemctl enable daemon.service

supostamente assim já fica a correr para "sempre", e dá restart automático caso a máquina deslige e ligue outra vez

para manter o daemon atualizado, clonar o repositório e fazer
'''
sudo systemctl restart daemon.service
'''