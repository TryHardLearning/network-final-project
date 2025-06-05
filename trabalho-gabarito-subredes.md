# Trabalho: Integração de habilidades - 2025/1  
**Disciplina:** Redes de Computadores  
**Curso:** Engenharia de Computação / Tecnologia em Análise e Desenvolvimento de Sistemas  

**Nome:**  
**RA:**  

---

## Tarefa 1: Sub-Redes

|     Sub- Rede     |       IPv4 - Sub-Rede       |       IPv4 - Máscara      |             IPv6 - Sub-Rede/Prefixo            |
| :---------------: | :-------------------------: | :-----------------------: | :--------------------------------------------: |
|    Pato Branco    | 200.136.**N**.*00*          | 255.255.255.*192*         |    2001:DB8:CAFE:**NN***00*::/64               |
| Francisco Beltrão | 200.136.**N**.*64*          | 255.255.255.*224*         |    2001:DB8:CAFE:**NN***01*::/64               |
|   Dois Vizinhos   | 200.136.**N**.*96*          | 255.255.255.*224*         |    2001:DB8:CAFE:**NN***02*::/64               |
|       Toledo      | 200.136.**N**.*128*         | 255.255.255.*224*         |    2001:DB8:CAFE:**NN***03*::/64               |
|     Medianeira    | 200.136.**N**.*160*         | 255.255.255.*224*         |    2001:DB8:CAFE:**NN***04*::/64               |
|    Santa Helena   | 200.136.**N**.*192*         | 255.255.255.*224*         |    2001:DB8:CAFE:**NN***05*::/64               |
|       pb-vit      | 200.136.**N**.*224*         | 255.255.255.*252*         |    2001:DB8:CAFE:**NN**FF::/112                |
|       vit-fb      | 200.136.**N**.*228*         | 255.255.255.*252*         |    2001:DB8:CAFE:**NN**FF::*1*:0/112           |
|       fb-ita      | 200.136.**N**.*232*         | 255.255.255.*252*         |    2001:DB8:CAFE:**NN**FF::*2*:0/112          |
|       ita-pb      | 200.136.**N**.*236*         | 255.255.255.*252*         |    2001:DB8:CAFE:**NN**FF::*3*:0/112          |
|       ita-dv      | 200.136.**N**.*240*         | 255.255.255.*252*         |    2001:DB8:CAFE:**NN**FF::*4*:0/112          |



## Tarefa 2: Endereçamento de Dispositivos

|         Dispositivo        | Interface | IPv4                | IPv4 - Máscara    | IPv4 - Gateway     | IPv6/Prefixo (GUA)                    | IPv6 (LLA) | IPv6-Gateway |
| :------------------------: | :-------: | ------------------- | ----------------- | ------------------ | ------------------------------------- | ---------- | ------------ |
|             PC1            |    NIC    | 200.136.**N**.*3*   | 255.255.255.*192* | 200.136.**N**.*1*  | 2001\:DB8\:CAFE:**NN***00*::*3*/64    | EUI-64     | FE80::1      |
|             PC2            |    NIC    | 200.136.**N**.*4*   | 255.255.255.*192* | 200.136.**N**.*1*  | 2001\:DB8\:CAFE:**NN***00*::*4*/64    | EUI-64     | FE80::1      |
|             PC3            |    NIC    | 200.136.**N**.*67*  | 255.255.255.*224* | 200.136.**N**.*65* | 2001\:DB8\:CAFE:**NN***01*::*3*/64    | EUI-64     | FE80::1      |
|             PC4            |    NIC    | 200.136.**N**.*68*  | 255.255.255.*224* | 200.136.**N**.*65* | 2001\:DB8\:CAFE:**NN***01*::*4*/64    | EUI-64     | FE80::1      |
|             PC5            |    NIC    | 200.136.**N**.*99*  | 255.255.255.*224* | 200.136.**N**.*97* | 2001\:DB8\:CAFE:**NN***02*::*3*/64    | EUI-64     | FE80::1      |
|             PC6            |    NIC    | 200.136.**N**.*100* | 255.255.255.*224* | 200.136.**N**.*97* | 2001\:DB8\:CAFE:**NN***02*::*4*/64    | EUI-64     | FE80::1      |
|     Switch-Pato Branco     |    SVI    | 200.136.**N**.*2*   | 255.255.255.*192* | 200.136.**N**.*1*  | -                                     | -          | -            |
|  Switch-Francisco Beltrão  |    SVI    | 200.136.**N**.*66*  | 255.255.255.*224* | 200.136.**N**.*65* | -                                     | -          | -            |
|    Switch-Dois Vizinhos    |    SVI    | 200.136.**N**.*98*  | 255.255.255.*224* | 200.136.**N**.*97* | -                                     | -          | -            |
|    Roteador-Pato Branco    |   Fa0/0   | 200.136.**N**.*1*   | 255.255.255.*192* | -                  | 2001\:DB8\:CAFE:**NN**00::*1*/64      | FE80::1    | -            |
|    Roteador-Pato Branco    |  Se0/0/0  | 200.136.**N**.*225* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**NN**FF::*0*:*1*/112 | EUI-64     | -            |
|    Roteador-Pato Branco    |  Se0/0/1  | 200.136.**N**.*238* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**NN**FF::*3*:*2*/112 | EUI-64     | -            |
| Roteador-Francisco Beltrão |   Fa0/0   | 200.136.**N**.*65*  | 255.255.255.*224* | -                  | 2001\:DB8\:CAFE:**NN***01*::*1*/64    | FE80::1    | -            |
| Roteador-Francisco Beltrão |  Se0/0/0  | 200.136.**N**.*233* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**NN**FF::*2*:*1*/112 | EUI-64     | -            |
| Roteador-Francisco Beltrão |  Se0/0/1  | 200.136.**N**.*230* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**NN**FF::*1*:*2*/112 | EUI-64     | -            |
|      Roteador-Vitorino     |  Se0/0/0  | 200.136.**N**.*229* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**NN**FF::*1*:*1*/112 | EUI-64     | -            |
|      Roteador-Vitorino     |  Se0/0/1  | 200.136.**N**.*226* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**NN**FF::*0*:*2*/112 | EUI-64     | -            |
|     Roteador-Itapejara     |  Se0/0/0  | 200.136.**N**.*237* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**NN**FF::*3*:*1*/112 | EUI-64     | -            |
|     Roteador-Itapejara     |  Se0/0/1  | 200.136.**N**.*234* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**NN**FF::*2*:*2*/112 | EUI-64     | -            |
|     Roteador-Itapejara     |   Fa0/1   | 200.136.**N**.*241* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**NN**FF::*4*:*1*/112 | EUI-64     | -            |
|   Roteador-Dois Vizinhos   |   Fa0/0   | 200.136.**N**.*97*  | 255.255.255.*224* | -                  | 2001\:DB8\:CAFE:**NN***02*::*1*/64    | FE80::1    | -            |
|   Roteador-Dois Vizinhos   |   Fa0/1   | 200.136.**N**.*242* | 255.255.255.*252* | -                  | 2001\:DB8\:CAFE:**NN**FF::*4*:*2*/112 | EUI-64     | -            |


---

## Tarefa 3: Tabela de Roteamento
>Observação: inserir o número de linhas necessárias em cada tabela

### Roteador Pato Branco
#### IPv4
|  Rede de Destino   |      Máscara        |     Próximo Salto     | Interface de Saída  |  
|:------------------:|:-------------------:|:---------------------:|:-------------------:|  
| (preencher)        | (preencher)         | (preencher)           | (preencher)         |  

#### IPv6
|  Rede de Destino /Prefixo             |     Próximo Salto        | Interface de Saída  |  
|:-------------------------------------:|:------------------------:|:-------------------:|  
| (preencher)                           | (preencher)              | (preencher)         |  


#### Roteador Francisco Beltrão
#### IPv4
|  Rede de Destino   |      Máscara        |     Próximo Salto     | Interface de Saída  |  
|:------------------:|:-------------------:|:---------------------:|:-------------------:|  
| (preencher)        | (preencher)         | (preencher)           | (preencher)         |  

#### IPv6
|  Rede de Destino /Prefixo             |     Próximo Salto        | Interface de Saída  |  
|:-------------------------------------:|:------------------------:|:-------------------:|  
| (preencher)                           | (preencher)              | (preencher)         |  

#### Roteador Vitorino
#### IPv4
|  Rede de Destino   |      Máscara        |     Próximo Salto     | Interface de Saída  |  
|:------------------:|:-------------------:|:---------------------:|:-------------------:|  
| (preencher)        | (preencher)         | (preencher)           | (preencher)         |  

#### IPv6
|  Rede de Destino /Prefixo             |     Próximo Salto        | Interface de Saída  |  
|:-------------------------------------:|:------------------------:|:-------------------:|  
| (preencher)                           | (preencher)              | (preencher)         |  

#### Roteador Itapejara D'Oeste
#### IPv4
|  Rede de Destino   |      Máscara        |     Próximo Salto     | Interface de Saída  |  
|:------------------:|:-------------------:|:---------------------:|:-------------------:|  
| (preencher)        | (preencher)         | (preencher)           | (preencher)         |  

#### IPv6
|  Rede de Destino /Prefixo             |     Próximo Salto        | Interface de Saída  |  
|:-------------------------------------:|:------------------------:|:-------------------:|  
| (preencher)                           | (preencher)              | (preencher)         |  

#### Roteador Dois Vizinhos
#### IPv4
|  Rede de Destino   |      Máscara        |     Próximo Salto     | Interface de Saída  |  
|:------------------:|:-------------------:|:---------------------:|:-------------------:|  
| (preencher)        | (preencher)         | (preencher)           | (preencher)         |  

#### IPv6
|  Rede de Destino /Prefixo             |     Próximo Salto        | Interface de Saída  |  
|:-------------------------------------:|:------------------------:|:-------------------:|  
| (preencher)                           | (preencher)              | (preencher)         |  


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


