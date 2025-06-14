# Trabalho: Integração de habilidades - 2025/1  
**Disciplina:** Redes de Computadores  
**Curso:** Engenharia de Computação / Tecnologia em Análise e Desenvolvimento de Sistemas  

**Nome:**  Lucas C. Bresolino
**RA:**  2037882

---

## Tarefa 1: Sub-Redes

|     Sub- Rede     |       IPv4 - Sub-Rede       |       IPv4 - Máscara      |             IPv6 - Sub-Rede/Prefixo            |
| :---------------: | :-------------------------: | :-----------------------: | :--------------------------------------------: |
|    Pato Branco    | 200.136.**82**.*00* | 255.255.255.*192* |    2001:DB8:CAFE:**82** *00* ::/64   |
| Francisco Beltrão | 200.136.**82**.*64* | 255.255.255.*224* |    2001:DB8:CAFE:**82** *01* ::/64   |
|   Dois Vizinhos   | 200.136.**82**.*96* | 255.255.255.*224* |    2001:DB8:CAFE:**82** *02* ::/64   |
|       Toledo      | 200.136.**82**.*128* | 255.255.255.*224* |    2001:DB8:CAFE:**82** *03* ::/64   |
|     Medianeira    | 200.136.**82**.*160* | 255.255.255.*224* |    2001:DB8:CAFE:**82** *04* ::/64   |
|    Santa Helena   | 200.136.**82**.*192* | 255.255.255.*224* |    2001:DB8:CAFE:**82** *05* ::/64   |
|       pb-vit      | 200.136.**82**.*224* | 255.255.255.*252* | 2001:DB8:CAFE:**82**FF:: *00* :0/112 |
|       vit-fb      | 200.136.**82**.*228* | 255.255.255.*252* | 2001:DB8:CAFE:**82**FF:: *01* :0/112 |
|       fb-ita      | 200.136.**82**.*232* | 255.255.255.*252* | 2001:DB8:CAFE:**82**FF:: *02* :0/112 |
|       ita-pb      | 200.136.**82**.*236* | 255.255.255.*252* | 2001:DB8:CAFE:**82**FF:: *03* :0/112 |
|       ita-dv      | 200.136.**82**.*240* | 255.255.255.*252* | 2001:DB8:CAFE:**82**FF:: *04* :0/112 |



## Tarefa 2: Endereçamento de Dispositivos

|      Dispositivo      | Interface | IPv4                      | IPv4 - Máscara          | IPv4 - Gateway            | IPv6/Prefixo (GUA)                                   | IPv6 (LLA) | IPv6-Gateway |
| :-------------------: | :-------: | ------------------------- | ----------------------- | ------------------------- | ---------------------------------------------------- | ---------- | ------------ |
|          PC1          |    NIC    | 200.136.**82**.3 | 255.255.255.192 | 200.136.**82**.1 | 2001:DB8:CAFE:**82**00::3/64     | EUI-64     | *FE80::1*      |
|          PC2          |    NIC    | 200.136.**82**.4 | 255.255.255.192 | 200.136.**82**.1 | 2001:DB8:CAFE:**82**00::4/64     | EUI-64     | *FE80::1*      |
|          PC3          |    NIC    | 200.136.**82**.67 | 255.255.255.224 | 200.136.**82**.65 | 2001:DB8:CAFE:**82**01::3/64     | EUI-64     | *FE80::1*      |
|          PC4          |    NIC    | 200.136.**82**.68 | 255.255.255.224 | 200.136.**82**.65 | 2001:DB8:CAFE:**82**01::4/64     | EUI-64     | *FE80::1*      |
|          PC5          |    NIC    | 200.136.**82**.99 | 255.255.255.224 | 200.136.**82**.97 | 2001:DB8:CAFE:**82**02::3/64     | EUI-64     | *FE80::1*      |
|          PC6          |    NIC    | 200.136.**82**.100 | 255.255.255.224 | 200.136.**82**.97 | 2001:DB8:CAFE:**82**02::4/64     | EUI-64     | *FE80::1*      |
|  Switch-Pato Branco   |    SVI    | 200.136.**82**.2 | 255.255.255.192 | 200.136.**82**.1 | -                                                    | -          | -            |
|  Switch-Fco. Beltrão  |    SVI    | 200.136.**82**.66 | 255.255.255.224 | 200.136.**82**.65 | -                                                    | -          | -            |
|  Switch-Dois Vizinhos |    SVI    | 200.136.**82**.98 | 255.255.255.224 | 200.136.**82**.97 | -                                                    | -          | -            |
|  Roteador-Pato Branco |   Fa0/0   | 200.136.**82**.1 | 255.255.255.192 | -                         | 2001:DB8:CAFE:**82**00::1/64     | *FE80::1*    | -            |
|  Roteador-Pato Branco |  Se0/0/0  | 200.136.**82**.225 | 255.255.255.252 | -                         | 2001:DB8:CAFE:**82**FF::0:1/112 | EUI-64     | -            |
|  Roteador-Pato Branco |  Se0/0/1  | 200.136.**82**.238 | 255.255.255.252 | -                         | 2001:DB8:CAFE:**82**FF::3:2/112 | EUI-64     | -            |
| Roteador-Fco. Beltrão |   Fa0/0   | 200.136.**82**.65 | 255.255.255.224 | -                         | 2001:DB8:CAFE:**82**01::1/64     | *FE80::1*    | -            |
| Roteador-Fco. Beltrão |  Se0/0/0  | 200.136.**82**.233 | 255.255.255.252 | -                         | 2001:DB8:CAFE:**82**FF::2:1/112 | EUI-64     | -            |
| Roteador-Fco. Beltrão |  Se0/0/1  | 200.136.**82**.230 | 255.255.255.252 | -                         | 2001:DB8:CAFE:**82**FF::1:2/112 | EUI-64     | -            |
|   Roteador-Vitorino   |  Se0/0/0  | 200.136.**82**.229 | 255.255.255.252 | -                         | 2001:DB8:CAFE:**82**FF::1:1/112 | EUI-64     | -            |
|   Roteador-Vitorino   |  Se0/0/1  | 200.136.**82**.226 | 255.255.255.252 | -                         | 2001:DB8:CAFE:**82**FF::0:2/112 | EUI-64     | -            |
|   Roteador-Itapejara  |  Se0/0/0  | 200.136.**82**.237 | 255.255.255.252 | -                         | 2001:DB8:CAFE:**82**FF::3:1/112 | EUI-64     | -            |
|   Roteador-Itapejara  |  Se0/0/1  | 200.136.**82**.234 | 255.255.255.252 | -                         | 2001:DB8:CAFE:**82**FF::2:2/112 | EUI-64     | -            |
|   Roteador-Itapejara  |   Fa0/1   | 200.136.**82**.241 | 255.255.255.252 | -                         | 2001:DB8:CAFE:**82**FF::4:1/112 | EUI-64     | -            |
| Roteador-Dois Vizinhos|   Fa0/0   | 200.136.**82**.97 | 255.255.255.224 | -                         | 2001:DB8:CAFE:**82**02::1/64     | *FE80::1*    | -            |
| Roteador-Dois Vizinhos|   Fa0/1   | 200.136.**82**.242 | 255.255.255.252 | -                         | 2001:DB8:CAFE:**82**FF::4:2/112 | EUI-64     | -            |

---

## Tarefa 3: Tabela de Roteamento
>Observação: inserir o número de linhas necessárias em cada tabela

### Roteador Pato Branco
#### IPv4
|  Rede de Destino   |      Máscara        |     Próximo Salto     | Interface de Saída  |  
|:------------------:|:-------------------:|:---------------------:|:-------------------:|  
| 200.136.82.64       | 255.255.255.224          | 200.136.82.226           | Se0/0/0         |
| 200.136.82.96        | 255.255.255.224          | 200.136.82.237           | Se0/0/1         |

#### IPv6
|  Rede de Destino /Prefixo             |     Próximo Salto        | Interface de Saída  |  
|:-------------------------------------:|:------------------------:|:-------------------:|  
|2001:DB8:CAFE:8201::/64                           | 2001:DB8:CAFE:82FF:1:1              | Se0/0/0          |
| 2001:DB8:CAFE:8202::/64                          | 2001:DB8:CAFE:82FF:3:1              | Se0/0/1          |  


#### Roteador Francisco Beltrão
#### IPv4
|  Rede de Destino   |      Máscara        |     Próximo Salto     | Interface de Saída  |  
|:------------------:|:-------------------:|:---------------------:|:-------------------:|  
| 200.136.82.0        | 255.255.255.192        | 200.136.82.237         | Se0/0/0        |  
| 200.136.82.96       | 255.255.255.224        | 200.136.82.237         | Se0/0/0        |

#### IPv6
|  Rede de Destino /Prefixo             |     Próximo Salto        | Interface de Saída  |  
|:-------------------------------------:|:------------------------:|:-------------------:|  
| 2001:DB8:CAFE:8200::/64            | 2001:DB8:CAFE:82FF:2:2              | Se0/0/0         |  
| 2001:DB8:CAFE:8202::/64            | 2001:DB8:CAFE:82FF:2:2             | Se0/0/0         |  

#### Roteador Vitorino
#### IPv4
|  Rede de Destino   |      Máscara        |     Próximo Salto     | Interface de Saída  |  
|:------------------:|:-------------------:|:---------------------:|:-------------------:|  
| 200.136.82.64        | 255.255.255.224         | 200.136.82.230  | Se0/0/0         |

#### IPv6
|  Rede de Destino /Prefixo             |     Próximo Salto        | Interface de Saída  |  
|:-------------------------------------:|:------------------------:|:-------------------:|  
| 2001:DB8:CAFE:8201::/64                           | 2001:DB8:CAFE:82FF:1:2              | Se0/0/0         |  

#### Roteador Itapejara D'Oeste
#### IPv4
|  Rede de Destino   |      Máscara        |     Próximo Salto     | Interface de Saída  |  
|:------------------:|:-------------------:|:---------------------:|:-------------------:|  
| 200.136.82.0        | 255.255.255.192        | 200.136.82.238          | Se0/0/1        | 
| 200.136.82.64        | 255.255.255.224          | 200.136.82.234           | Se0/0/1         |

#### IPv6
|  Rede de Destino /Prefixo             |     Próximo Salto        | Interface de Saída  |  
|:-------------------------------------:|:------------------------:|:-------------------:|  
| 2001:DB8:CAFE:8200::/64                           | 2001:DB8:CAFE:82FF:3:2             | Se0/0/1        | 
| 2001:DB8:CAFE:8201::/64                          | 2001:DB8:CAFE:82FF:2:1             | Se0/0/1         |

#### Roteador Dois Vizinhos
#### IPv4
|  Rede de Destino   |      Máscara        |     Próximo Salto     | Interface de Saída  |  
|:------------------:|:-------------------:|:---------------------:|:-------------------:|  
| 200.136.82.0       | 255.255.255.192        | 200.136.82.241           | Fa0/1         |  
| 200.136.82.64       | 255.255.255.224         | 200.136.82.241           | 	Fa0/1         | 

#### IPv6
|  Rede de Destino /Prefixo             |     Próximo Salto        | Interface de Saída  |  
|:-------------------------------------:|:------------------------:|:-------------------:|  
| 2001:DB8:CAFE:8200::/64                         | 2001:DB8:CAFE:82FF:4:1             | Fa0/1         |  
| 2001:DB8:CAFE:8201::/64                          | 2001:DB8:CAFE:82FF:4:1              | Fa0/1        | 


---

## Tarefa 5: Testes de Conectividade (Opcional, mas recomendado)

| Origem     | Destino    | Tipo de Teste | Resultado       |  
|:----------:|:----------:|:-------------:|:---------------:|
| (preencher)| (preencher)| ping IPv4     | (sucesso/falha) |
| (preencher)| (preencher)| ping IPv6     | (sucesso/falha) |

---

## Checklist para Entrega

- [ ] Tabela de Sub-Redes preenchida corretamente  
- [ ] Tabela de Endereçamento preenchida corretamente para todos os dispositivos  
- [ ] Tabela de Roteamento completa para todos os roteadores  
- [ ] Testes realizados e documentados (opcional)  
- [ ] Documento salvo no formato .md com nome no padrão: Trabalho_Redes_Nome_RA  

