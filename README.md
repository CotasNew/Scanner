Scanner Ultra 1.0 - Termux

Scanner Ultra 1.0 é um script completo e profissional para uso no Termux (Android), desenvolvido por @diego_cotas, que integra diversas ferramentas de segurança para testes de vulnerabilidades, enumeração de subdomínios, fingerprinting, crawling, fuzzing e SQL Injection.

Funcionalidades

Scanner de subdomínios (Amass + Subfinder)

Detecção de tecnologias (WhatWeb)

Varredura de portas (Nmap)

Crawling de links (Hakrawler)

Fuzzing de diretórios ocultos (Ffuf)

Testes de SQL Injection (SQLmap)

Relatório final em HTML responsivo e profissional

Menu interativo com design moderno e animações


Requisitos

Instale os seguintes pacotes no Termux:

pkg update && pkg upgrade -y
pkg install git wget curl python nmap -y
pkg install golang -y
pip install requests colorama tqdm

# Instalar ferramentas adicionais
pkg install whatweb
pkg install sqlmap
pkg install amass
pkg install nmap
pkg install ffuf
pkg install golang

# Subfinder (Go)
go install -v github.com/projectdiscovery/subfinder/v2/cmd/subfinder@latest

# Hakrawler (Go)
go install github.com/hakluke/hakrawler@latest

# Adicione o PATH do Go (caso não esteja ativo)
echo 'export PATH=$PATH:/data/data/com.termux/files/home/go/bin' >> ~/.bashrc
source ~/.bashrc

Como usar

git clone https://github.com/seuusuario/scanner-ultra-termux
cd scanner-ultra-termux
chmod +x scanner-ultra.sh
./scanner-ultra.sh

Autor

Desenvolvido por @diego_cotas

Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo LICENSE para detalhes.
pkg update && pkg upgrade -y
pkg install git wget curl python nmap -y
pkg install golang -y
pip install requests colorama tqdm

# Instalar ferramentas adicionais
pkg install whatweb
pkg install sqlmap
pkg install amass
pkg install nmap
pkg install ffuf
pkg install golang

# Subfinder (Go)
go install -v github.com/projectdiscovery/subfinder/v2/cmd/subfinder@latest

# Hakrawler (Go)
go install github.com/hakluke/hakrawler@latest

# Adicione o PATH do Go (caso não esteja ativo)
echo 'export PATH=$PATH:/data/data/com.termux/files/home/go/bin' >> ~/.bashrc
source ~/.bashrc


COMO USAR ****
git clone https://github.com/seuusuario/scanner-ultra-termux
cd scanner-ultra-termux
chmod +x scanner-ultra.sh
./scanner-ultra.sh

