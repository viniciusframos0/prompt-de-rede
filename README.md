# Prompt de Rede

Simulador do Prompt de Comando do Windows para praticar comandos de rede no celular, em sala de aula. Acompanha a **Apostila 02 – Comandos de Rede e Diagnóstico** (Redes de Computadores II, ETEMB).

**Abrir:** https://viniciusframos0.github.io/prompt-de-rede/

## O que dá para fazer

- **Identificação:** `ipconfig` (`/all`, `/release`, `/renew`, `/flushdns`, `/displaydns`), `hostname`, `whoami`, `getmac`, `netsh`
- **Testes:** `ping` (`-t`, `-n`, `-l`, `-4`, `-6`), `tracert`, `pathping`, `curl`, e no PowerShell `Test-NetConnection`
- **Análise:** `nslookup` (inclusive modo interativo e `set type=MX`), `netstat -ano`, `tasklist`, `arp`, `route`
- **Outros:** `net view/share/use`, `systeminfo`, `nmap` (somente na rede do laboratório) e `ssh aluno@192.168.0.10` para praticar `ip a`, `ip route`, `ip neigh` e `ss -tuln` no Linux
- **Filtros com `|`:** `netstat -ano | findstr :443`, `tasklist | findstr 6340`
- **Chamados de suporte:** 8 defeitos para diagnosticar com o roteiro da apostila (IP 169.254, pilha TCP/IP, gateway, provedor, DNS, perda de pacotes, serviço fora do ar e ARP spoofing), mais o “chamado surpresa”
- **Apostila no app:** lista de comandos, roteiro de diagnóstico, atividade prática (questões 1 a 16) e quadro Windows × Linux

Cada celular vira um computador diferente do laboratório (IP entre 192.168.0.101 e 192.168.0.199), então os alunos podem fazer ping uns nos outros.

## Como funciona

- Um único arquivo (`index.html`), sem instalação e sem bibliotecas externas.
- Com internet, o `nslookup` faz consultas DNS reais e o `ping` mede o tempo real da conexão do celular. Sem internet, ou numa rede que bloqueia essas consultas, o simulador usa respostas de exemplo. A barra do topo mostra qual modo está ativo.
- Escrito para funcionar também em celulares e navegadores antigos.

## Publicar

O site é servido pelo GitHub Pages a partir da branch `main` (pasta raiz).
