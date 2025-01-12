# rede
### Conectando o Roteador no Modem
Conecte o cabo de ethernet na entrada LAN do Modem e na entrada WAN do Roteador
Passo 1: Acesse o navegador com o IP 192.168.0.1 no Modem para desabilitar o WI-FI
Passo 2: Configurar o IP no Roteador começando pela entrada LAN
Endereço IP: 192.168.1.1
Máscara de Sub-Rede: 255.255.255.0
Passo 3: Configurar a rede com o IP Estático
Endereço IP: 192.168.0.2
Máscara de Sub-Rede: 255.255.255.0
Gateway Padrão: 192.168.0.1
DNS Primário: 8.8.8.8
DNS Secundário: 1.1.1.1

Classe A: 0 - 127
Classe B: 128 - 191
Classe C: 192 - 223

Classe A: 10.1.1.10 Rede:(10.) Host:(1.1.10)
Classe B: 172.16.10.1 Rede:(172.16.) Host:(10.1)
Classe C: 192.168.0.1 Rede:(192.168.0.) Host:(1)

IPs Restritos ou Privados (RFC 1918)
10.0.0.0
172.16.0.0
192.168.0.0

Máscara de Rede
Classe A: 255.0.0.0
Classe B: 255.255.0.0
Classe C: 255.255.255.0

127.0.0.0 (Loop Back)
169.254.0.0 (Apipa)
0.0.0.0 (Inicialização)
255.255.255.255 (BroadCast Geral)

Fazer o teste de funcionamento do Modem através do CMD (Prompt de Comando)
No CMD digite > ipconfig e aperte ENTER e procure o IP do Modem Conectado
Depois de identificar o IP do Modem que é 192.168.0.1 fazer o teste do PING 
No CMD Digite > ping 192.168.0.1 e aperte ENTER

PING - É o comando que testa a conectividade
LATÊNCIA - É o tempo de espera de resposta
MS - Milissegundo medida de tempo
TTL - Time To Live (0 - 255) tempo de vida do pacote na rede
ICMP - Protocolo de teste de conectividade

Testar a Placa de Rede no CMD com o comando Ping
>ping 127.0.0.1 e aperta ENTER

Testar site do Google no CMD através do PING e TRACERT 
>ping google.com.br aperte ENTER
>tracert google.com.br aperte ENTER

# Liberação do cache do DNS
>ipconfig /flushdns

>ipconfig /release

>ipconfig /renew

# PORTA DE REDE
FTP (20-21) TRANSFERÊNCIA DE ARQUIVOS
SSH (22) TERMINAL REMOTO OU ACESSO REMOTO COM CRIPTOGRAFIA
TELNET (23) ACESSO REMOTO SEM CRIPTOGRAFIA
SMTP (25-587) GERÊNCIA O E-MAIL
DNS (53) ASSOCIA A UM NOME
DHCP (67) DISTRIBUI AS CONFIGURAÇÕES DE REDES
TFTP (69) TRANSFERÊNCIA  DE ARQUIVOS SIMPLES
FINGER (79) INFORMAÇÃO DE USUÁRIOS
HTTP (80) TRANSFERÊNCIA DE HIPER TEXTO SEM CRIPTOGRAFIA
POP (110) RECEBIMETO DE E-MAIL DESTRUTIVO (BAIXADO PRA MÁQUINA E EXCLUIDO DO SERVIDOR)
NTP (123) SICRONIZAÇÃO DE DATA E HORA
IMAP (143) RECEBIMETO DE E-EMAIL NÃO DESTRUTIVO (BAIXA UMA CÓPIA DO SERVIDOR PRA MÁQIUNA)
SNMP (161-162) GERENCIAMENTO DE CONEXÕES
HTTPS (443) TRANSFERÊNCIA DE HIPER TEXTO COM CRIPTOGRAFIA (SSL-TLS)

# CONFIGURAÇÃO REMOTO
RENOMEIE O COMPUTADOR E O NOME DO GRUPO DE TRABALHO
COLOCAR O IP FIXO NAS MÁQUINAS SEGUINDO O GATEWAY PADRÃO DO ROTEADOR
PARTICIONAR O ARMAZENAMENTO NO GERENCIAMENTO DE DISCO
