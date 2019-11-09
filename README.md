# Pesquisa de Satisfação - TI

## DESCRICAO DOS DADOS

### TABELA FATO

#### FPESQUISA
* **ID_Processador**
* **ID_Notificador**
* **ID_SSI**
* **Data_Criacao_SSI:** Data de abertura da SSI.<br>
* **Data_Encerramento_SSI:** Data de encerramento do chamado.<br>

### TABELAS DE DIMENSAO

#### DNOTIFICADOR: Armazena informacoes relativas ao notificador (pessoa que abre a SSI).<br>
* **ID_Notificador:** Número Decimal<br>
   Tipo de dado:
* **Nome:** Texto<br>
   Tipo de dado:
* **Departamento:** Texto<br>
   Tipo de dado:
* **Diretoria:** Texto<br>
   Tipo de dado:
* **Empresa:** Texto<br>
   Tipo de dado:

#### DSSI: Armazena informacoes relativas a SSI (chamado).<br>
* **ID_SSI:** Número Decimal.<br>
   Tipo de dado:
* **SSI:** Número Inteiro.<br>
   Tipo de dado:
* **Descricao:** Texto.<br>
   Tipo de dado:

#### DPROCESSADOR: Armazena informacoes relativas ao processador (pessoa que atende a SSI).<br>
* **ID_Processador:** Número Decimal.<br>
   Tipo de dado:
* **Nome:** Texto.<br>
   Tipo de dado:
* **Equipe_suporte:** Texto ; Infra, Sistemas, Suporte N1.<br>
   Tipo de dado:

#### DRESPOSTA: Armazena informacoes referentes ao preenchimento da pesquisa de satisfacao.<br>
* **ID_SSI:** Número Decimal<br>
   Tipo de dado:
* **SSI:** Número Inteiro (Necessário??)<br>
   Tipo de dado:
* **Data_Resposta_Pesquisa:** <br>
   Tipo de dado:
* **Resolucao_Problema:** Texto ; Seu problema foi resolvido neste atendimento? <br>
   Tipo de dado:
* **Agilidade_Atendimento:** Texto ; Quão ágil foi a resolução do seu atendimento?<br>
   Tipo de dado:
* **Qualidade_Atendimento:** Texto ; Quão bem atendido você foi?<br>
   Tipo de dado:
* **Satisfacao_Atendimento:** Número Inteiro ; De 1 a 5, quão satisfeito você está com o serviço prestado neste atendimento?<br>
   Tipo de dado:
* **Comentários:** Texto ; Compartilhe conosco o que achar importante.<br>
   Tipo de dado:


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

