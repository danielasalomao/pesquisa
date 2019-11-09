# Pesquisa de Satisfação - TI

## DESCRICAO DOS DADOS

### TABELA FATO

#### FPESQUISA
* **ID_Processador**<br>
   Tipo de dado:
* **ID_Notificador**<br>
   Tipo de dado:
* **ID_SSI**<br>
   Tipo de dado:
* **Data_Criacao_SSI:** Data de abertura da SSI.<br>
   Tipo de dado:
* **Data_Encerramento_SSI:** Data de encerramento do chamado.<br>
   Tipo de dado:

### TABELAS DE DIMENSAO

#### DNOTIFICADOR: Armazena informacoes relativas ao notificador (pessoa que abre a SSI).<br>
* **ID_Notificador:** <br>
   Tipo de dado: Número Decimal
* **Nome:** <br>
   Tipo de dado: Texto
* **Departamento:** <br>
   Tipo de dado: Texto
* **Diretoria:** <br>
   Tipo de dado: Texto
* **Empresa:** <br>
   Tipo de dado: Texto

#### DSSI: Armazena informacoes relativas a SSI (chamado).<br>
* **ID_SSI:** <br>
   Tipo de dado: Número Decimal
* **SSI:** Número Inteiro.<br>
   Tipo de dado: Número Inteiro
* **Descricao:** Texto.<br>
   Tipo de dado: Texto

#### DPROCESSADOR: Armazena informacoes relativas ao processador (pessoa que atende a SSI).<br>
* **ID_Processador:** Número Decimal.<br>
   Tipo de dado: Número Decimal
* **Nome:** Texto.<br>
   Tipo de dado: Texto
* **Equipe_suporte:** Texto ; Infra, Sistemas, Suporte N1.<br>
   Tipo de dado: Texto

#### DRESPOSTA: Armazena informacoes referentes ao preenchimento da pesquisa de satisfacao.<br>
* **ID_SSI:** Número Decimal<br>
   Tipo de dado: Número Decimal
* **SSI:** Número Inteiro (Necessário??)<br>
   Tipo de dado: Número Inteiro
* **Data_Resposta_Pesquisa:** <br>
   Tipo de dado:
* **Resolucao_Problema:** Texto ; Seu problema foi resolvido neste atendimento? <br>
   Tipo de dado: Texto
* **Agilidade_Atendimento:** Texto ; Quão ágil foi a resolução do seu atendimento?<br>
   Tipo de dado: Texto
* **Qualidade_Atendimento:** Texto ; Quão bem atendido você foi?<br>
   Tipo de dado: Texto
* **Satisfacao_Atendimento:** Número Inteiro ; De 1 a 5, quão satisfeito você está com o serviço prestado neste atendimento?<br>
   Tipo de dado: Número Inteiro
* **Comentários:** Texto ; Compartilhe conosco o que achar importante.<br>
   Tipo de dado: Texto


#### DCALENDARIO:
* **Ano:** AAAA<br>
   Tipo de dado:
* **Data:** DD/MM/AAAA<br>
   Tipo de dado:
* **Dia:** DD<br>
   Tipo de dado:
* **Mes:** MM<br>
   Tipo de dado:
* **Mes/Ano:** MM/AAAA<br>
   Tipo de dado:


## MODELAGEM DIMENSIONAL

### MODELO STAR SCHEMA

![Alt text](https://github.com/danielasalomao/pesquisa/blob/v1/Star_Schema.png)

