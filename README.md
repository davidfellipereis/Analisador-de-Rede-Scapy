# 🛡️ Scapy Network Analyzer & Security Suite

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)
![Scapy](https://img.shields.io/badge/Library-Scapy-red)
![CustomTkinter](https://img.shields.io/badge/UI-CustomTkinter-darkgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)

O **Scapy Network Analyzer & Security Suite** é uma aplicação desktop completa desenvolvida em Python para análise de tráfego, auditoria de redes locais e detecção de ameaças (IDS) em tempo real. A ferramenta combina o poder do **Scapy** para manipulação de pacotes em baixo nível com uma interface gráfica moderna criada em **CustomTkinter**.

---

## 📸 Interface do Aplicativo

*(Adicione imagens das abas do seu aplicativo aqui)*

---

## ✨ Funcionalidades Principais

### 🔍 1. Scanner de Rede (ARP Scan) & Relatórios PDF
* Mapeamento rápido de dispositivos ativos na rede local via requisições ARP.
* Consulta integrada à API **MacVendors** para identificação do fabricante do hardware (NIC/Placa de Rede).
* Geração automatizada de **relatórios executivos em PDF** contendo tabela formatada de IP, MAC e Fabricante.

### 🚪 2. Scanner de Portas (TCP SYN Scan)
* Varredura stealth (SYN Scan) para detecção de portas TCP abertas em alvos específicos.
* Mapeamento automático dos principais serviços associados às portas (SSH, HTTP, HTTPS, RDP, SMB, etc.).

### 🦈 3. Sniffer de Tráfego
* Captura de tráfego em tempo real com suporte a filtros avançados **BPF** (*Berkley Packet Filter*).
* Exibição detalhada de pacotes TCP, UDP e ICMP.
* Exportação dos dados capturados diretamente para arquivos no formato **`.pcap`** (compatíveis com Wireshark).

### 🚨 4. Detector de ARP Spoofing (IDS)
* Sistema de Detecção de Intrusão em tempo real monitorando a integridade do Gateway/Roteador.
* Alertas visuais automáticos ao detectar discrepâncias entre o endereço MAC legítimo e falsificações na rede (Ataques Man-in-the-Middle).

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3
* **Manipulação de Pacotes:** [Scapy](https://scapy.net/)
* **Interface Gráfica (GUI):** [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter)
* **Geração de PDF:** [ReportLab](https://www.reportlab.com/)
* **Concorrência:** `threading` (para execução assíncrona das varreduras sem travar a interface)

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
* Python 3.10 ou superior instalado.
* Npcap (no Windows) ou Libpcap (no Linux) instalado para permitir a captura de pacotes em modo promíscuo pelo Scapy.

### 1. Clonar o Repositório
```bash
git clone [https://github.com/seu-usuario/scapy-network-suite.git](https://github.com/seu-usuario/scapy-network-suite.git)
cd scapy-network-suite
