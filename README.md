# rede
A seguir, um aprofundamento em todos os tópicos essenciais de redes, desde conceitos básicos até tecnologias emergentes.

## 1. Conceitos Fundamentais
### 1.1 O que é uma Rede de Computadores?
Uma rede é um sistema de dispositivos interconectados que trocam dados usando protocolos de comunicação.

### Componentes Básicos:
- **Nós (Hosts)**: Computadores, servidores, smartphones, IoT.

- **Meios de Transmissão**: Cabos (ethernet, fibra óptica), wireless (Wi-Fi, rádio).

- **Dispositivos de Rede**: Switches, roteadores, firewalls.

- **Protocolos**: Regras de comunicação (TCP/IP, HTTP, DNS).

### 1.2 Benefícios das Redes
✔ **Compartilhamento de Recursos** (impressoras, armazenamento).<br>
✔ **Comunicação Instantânea** (e-mail, VoIP, videoconferência).<br>
✔ **Escalabilidade** (adicionar novos dispositivos facilmente).<br>
✔ **Tolerância a Falhas** (balanceamento de carga, redundância).<br>
✔ **Redução de Custos** (compartilhamento de infraestrutura).<br>

## 2. Tipos de Redes
### 2.1 Classificação por Alcance Geográfico
| Tipo |	Alcance	| Exemplo |
|------|------|------|
| **PAN** (Personal Area Network)	| ~10m	| Bluetooth, USB |
| **LAN** (Local Area Network)	| ~1km	| Rede doméstica, escritório |
| **MAN** (Metropolitan Area Network) |	~50km	| Rede de uma cidade |
| **WAN** (Wide Area Network)	| Global |	Internet, redes corporativas |
| **SAN** (Storage Area Network)	| Armazenamento dedicado	| NAS, servidores de backup |
### 2.2 Topologias de Rede
| Topologia	| Vantagens	| Desvantagens |
|------|------|------|
| Estrela (Star)	| Fácil manutenção, falha localizada	| Ponto único de falha (hub/switch) |
| Barramento (Bus) |	Simples, barato	| Colisões de dados, difícil diagnóstico |
| Anel (Ring)	| Baixa latência	| Falha em um nó quebra a rede |
| Malha (Mesh) |	Alta redundância	| Custo elevado, complexidade |
| Híbrida |	Combina vantagens	| Configuração complexa |
### 2.3 Meios de Transmissão
| Tipo	| Velocidade	| Distância	| Exemplo |
|------|------|------|------|
| Cabo Coaxial |	10-100 Mbps |	~500m |	TV a cabo (obsoleto em redes) |
| Par Trançado (UTP/STP) |	1 Gbps (Cat6)	| ~100m |	Ethernet (RJ45) |
| Fibra Óptica	| 10-100 Gbps	| ~40km+	| Backbone de internet |
| Wireless (Wi-Fi)	| 54 Mbps - 10 Gbps	| ~100m (Wi-Fi 6)	| Redes domésticas |
| Rádio (5G, Satélite)	| 100 Mbps - 2 Gbps	| Longo alcance |	Conexões móveis |
## 3. Modelos de Referência (OSI vs TCP/IP)
### 3.1 Modelo OSI (7 Camadas)
| Camada	| Função	| Protocolos/Dispositivos |
|------|------|------|
| 7. Aplicação	| Interface com usuário	| HTTP, FTP, SMTP |
| 6. Apresentação	| Formatação de dados	| SSL, JPEG, MPEG
| 5. Sessão	| Controle de diálogo	| NetBIOS, RPC |
| 4. Transporte	| Entrega confiável	| TCP, UDP |
| 3. Rede	| Roteamento	| IP, ICMP, roteadores |
| 2. Enlace	| Controle de acesso	| Ethernet, switches |
| 1. Física |	Transmissão de bits	| Cabos, hubs |
### 3.2 Modelo TCP/IP (4 Camadas)
| Camada	| Equivalente OSI	| Protocolos |
|------|------|------|
| Aplicação	| 5,6,7	| HTTP, DNS, SSH |
| Transporte	| 4	| TCP, UDP |
| Internet	| 3	| IP, ICMP |
| Acesso à Rede	| 1,2	| Ethernet, Wi-Fi |
## 4. Protocolos de Rede
### 4.1 Camada de Aplicação
| Protocolo	| Função	| Porta |
|------|------|------|
| HTTP/HTTPS	| Navegação web	| 80/443 |
| FTP/SFTP	| Transferência de arquivos	| 21/22 |
| SMTP	| Envio de e-mails	| 25 |
| DNS	| Traduz nomes para IP	| 53 |
| DHCP	| Atribuição automática de IP |	67/68 |
### 4.2 Camada de Transporte
| Protocolo	| Características |	Uso |
|------|------|------|
| TCP	| Confiável, orientado a conexão	| Web, e-mail |
| UDP	| Rápido, sem conexão	| Vídeo, VoIP |
### 4.3 Camada de Rede
| Protocolo	| Função	| Exemplo |
|------|------|------|------|
| IPv4/IPv6	| Endereçamento	| 192.168.1.1 / 2001:db8::1 |
| ICMP	| Diagnóstico	| Ping, Traceroute |
|ARP	| Mapeamento IP-MAC	| `arp -a` |
## 5. Endereçamento IP e Sub-redes
### 5.1 IPv4 vs IPv6
| Característica	| IPv4	| IPv6 |
|------|------|------|
| Tamanho	| 32 bits	| 128 bits |
| Notação	| 192.168.1.1	| 2001:0db8:85a3::8a2e:0370:7334 |
| Endereços |	~4.3 bilhões	| ~3.4×10³⁸ |
| Segurança |	Requer IPSec	| IPSec nativo |
### 5.2 Máscaras de Sub-rede e CIDR
_ **Exemplo**: `192.168.1.0/24` → 256 endereços (192.168.1.1 - 192.168.1.254)
_ **Sub-rede /26** → 64 endereços (úteis: 62)

## 6. Segurança em Redes
### 6.1 Ameaças Comuns
- **Ataques DDoS** (sobrecarga de servidores)
- **Man-in-the-Middle** (interceptação de dados)
- **Phishing** (fraude por e-mail/sites falsos)
- **Exploração de Vulnerabilidades** (Zero-day, Ransomware)

### 6.2 Medidas de Proteção
✔ **Firewalls** (filtro de tráfego)<br>
✔ **VPNs** (criptografia de dados)<br>
✔ **Autenticação Multifator** (MFA)<br>
✔ **IDS/IPS** (detecção de intrusões)<br>

## 7. Redes Sem Fio (Wi-Fi)
### 7.1 Padrões Wi-Fi
| Padrão	| Velocidade	| Frequência |
|------|------|------|
| 802.11n (Wi-Fi 4)	| 600 Mbps	| 2.4/5 GHz |
| 802.11ac (Wi-Fi 5)	| 3.5 Gbps	| 5 GHz |
| 802.11ax (Wi-Fi 6)	| 9.6 Gbps	| 2.4/5/6 GHz |
### 7.2 Segurança Wi-Fi
**WPA3** (mais seguro, resistente a ataques)
**WEP** (inseguro, evitado)

## 8. Virtualização e SDN
### 8.1 VLANs
- Divisão lógica de redes físicas.
- **Exemplo**: VLAN 10 (Departamento Financeiro), VLAN 20 (TI).

### 8.2 SDN (Software-Defined Networking)
- Separa plano de controle (software) do plano de dados (hardware).
- **Benefícios**: Automação, escalabilidade, flexibilidade.

## 9. Tendências em Redes
🚀 **5G e 6G** (ultra-velocidade, baixa latência)<br>
🌐 **IoT** (Internet das Coisas) (dispositivos inteligentes)<br>
☁ **Edge Computing** (processamento próximo ao usuário)<br>
🤖 **IA em Redes** (otimização automática)<br>
