# Trabalho: Integração de habilidades - 2025/2
## **Disciplina:** Redes de Computadores
### **Cursos:** Engenharia de Computação / Tecnologia em Análise e Desenvolvimento de Sistemas
**Nome:Bernardo Lucini**
**RA:A2773473**

---

## 📑 Tarefa 1: Tabela de Sub-Redes (0,5 Ponto)


| Sub- Rede | IPv4 - Sub-Rede | IPv4 - Máscara | IPv6 - Sub-Rede/Prefixo |
| :---: | :---: | :---: | :---: |
| **Pato Branco** | 200.136.73.0 | 255.255.255.192 | 2001:DB8:CAFE:7300::/64 |
| **Francisco Beltrão** | 200.136.73.64 | 255.255.255.224 | 2001:DB8:CAFE:7301::/64 |
| **Dois Vizinhos** | 200.136.73.92 | 255.255.255.224 | 2001:DB8:CAFE:7302::/64 |
| **Toledo** | 200.136.73.128 | 255.255.255.224 | 2001:DB8:CAFE:7303::/64 |
| **Medianeira** | 200.136.73.160 | 255.255.255.224 | 2001:DB8:CAFE:7304::/64 |
| **Santa Helena** | 200.136.73.192 | 255.255.255.224 | 2001:DB8:CAFE:7305::/64 |
| **pb-vit** | 200.136.73.224 | 255.255.255.252 | 2001:DB8:CAFE:73FF::/112 |
| **vit-fb** | 200.136.73.228 | 255.255.255.252 | 2001:DB8:CAFE:73FF::1:0/112 |
| **fb-ita** | 200.136.73.232 | 255.255.255.252 | 2001:DB8:CAFE:73FF::2:0/112 |
| **ita-pb** | 200.136.73.236 | 255.255.255.252 | 2001:DB8:CAFE:73FF::3:0/112 |
| **ita-dv** | 200.136.73.240 | 255.255.255.252 | 2001:DB8:CAFE:73FF::4:0/112 |




---

## 🖥️ Tarefa 2: Tabela de Endereçamento Lógico (0,5 Ponto)

*Preencha o endereçamento estático de todos os dispositivos de infraestrutura (Servidores, Switches e Roteadores). PCs usarão DHCP.*

| Dispositivo | Interface | IPv4 | IPv4 - Máscara | IPv4 - Gateway | IPv6/Prefixo (GUA) | IPv6 (LLA) | IPv6-Gateway |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **SRV-PB-DNS-DHCP** | NIC | 200.136.73.3 | 255.255.255.192 | 200.136.73.1 | 2001:DB8:CAFE:73(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-PB-WEB** | NIC | 200.136.73.4 | 255.255.255.192 | 200.136.73.1 | 2001:DB8:CAFE:73(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-FB-DNS-DHCP** | NIC | 200.136.73.67 | 255.255.255.224 | 200.136.73.65 | 2001:DB8:CAFE:73(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-FB-WEB** | NIC | 200.136.73.68 | 255.255.255.224 | 200.136.73.65 | 2001:DB8:CAFE:73(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-DV-DNS-DHCP** | NIC | 200.136.73.99 | 255.255.255.224 | 200.136.73.97 | 2001:DB8:CAFE:73(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-DV-WEB** | NIC | 200.136.73.100 | 255.255.255.224 | 200.136.73.97 | 2001:DB8:CAFE:73(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **Switch-Pato Branco** | SVI | 200.136.73.2 | 255.255.255.192 | 200.136.73.1 | 2001:DB8:CAFE:73(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **Switch-Fco. Beltrão** | SVI | 200.136.73.66 | 255.255.255.224 | 200.136.73.65 | 2001:DB8:CAFE:73(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **Switch-Dois Vizinhos** | SVI | 200.136.73.98 | 255.255.255.224 | 200.136.73.97 | 2001:DB8:CAFE73(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **Roteador-Pato Branco** | Fa0/0 | 200.136.73.1 | 255.255.255.192 | **-** | 2001:DB8:CAFE:73(preencher)::(preencher)/64 | *FE80::1* | **-** |
| **Roteador-Pato Branco** | Se0/0/0 | 200.136.73.225 | 255.255.255.252 | **-** | 2001:DB8:CAFE:73FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Pato Branco** | Se0/0/1 | 200.136.73.238 | 255.255.255.252 | **-** | 2001:DB8:CAFE:73FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Fco. Beltrão** | Fa0/0 | 200.136.73.65 | 255.255.255.224 | **-** | 2001:DB8:CAFE:73(preencher)::(preencher)/64 | *FE80::1* | **-** |
| **Roteador-Fco. Beltrão** | Se0/0/0 | 200.136.73.233 | 255.255.255.252 | **-** | 2001:DB8:CAFE:73FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Fco. Beltrão** | Se0/0/1 | 200.136.73.230 | 255.255.255.252 | **-** | 2001:DB8:CAFE:73FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Vitorino** | Se0/0/0 | 200.136.73.229 | 255.255.255.252 | **-** | 2001:DB8:CAFE:73FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Vitorino** | Se0/0/1 | 200.136.73.226 | 255.255.255.252 | **-** | 2001:DB8:CAFE:73FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Itapejara** | Se0/0/0 | 200.136.73.237 | 255.255.255.252 | **-** | 2001:DB8:CAFE:73FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Itapejara** | Se0/0/1 | 200.136.73.234 | 255.255.255.252 | **-** | 2001:DB8:CAFE:73FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Itapejara** | Fa0/1 | 200.136.73.241 | 255.255.255.252 | **-** | 2001:DB8:CAFE:73FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Dois Vizinhos** | Fa0/0 | 200.136.73.97 | 255.255.255.224 | **-** | 2001:DB8:CAFE:73(preencher)::(preencher)/64 | *FE80::1* | **-** |
| **Roteador-Dois Vizinhos** | Fa0/1 | 200.136.73.242 | 255.255.255.252 | **-** | 2001:DB8:CAFE:73FF::(preencher):(preencher)/112 | EUI-64 | **-** |
---

## 🗺️ Tarefa 3: Tabela de Roteamento (0,5 Ponto)

> Observação: Preencher apenas as rotas estáticas para redes remotas. Lembre-se do fluxo assimétrico (PB $\rightarrow$ VT $\rightarrow$ FB e FB $\rightarrow$ ITA $\rightarrow$ PB).

### Roteador Pato Branco

#### IPv4

| Rede de Destino | Máscara | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) | (preencher) |

#### IPv6

| Rede de Destino /Prefixo | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) |

### Roteador Francisco Beltrão

#### IPv4

| Rede de Destino | Máscara | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) | (preencher) |

#### IPv6

| Rede de Destino /Prefixo | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) |

### Roteador Vitorino

#### IPv4

| Rede de Destino | Máscara | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) | (preencher) |

#### IPv6

| Rede de Destino /Prefixo | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) |

### Roteador Itapejara D'Oeste

#### IPv4

| Rede de Destino | Máscara | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) | (preencher) |

#### IPv6

| Rede de Destino /Prefixo | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) |

### Roteador Dois Vizinhos

#### IPv4

| Rede de Destino | Máscara | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) | (preencher) |

#### IPv6

| Rede de Destino /Prefixo | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) |

---

### Checklist para Entrega 1

- [X] Tarefa 1: Tabela de Sub-Redes preenchida corretamente
- [ ] Tarefa 2: Tabela de Endereçamento preenchida corretamente para todos os dispositivos de infraestrutura
- [ ] Tarefa 3: Tabela de Roteamento completa para todos os roteadores
- [ ] Documento salvo no formato .md
