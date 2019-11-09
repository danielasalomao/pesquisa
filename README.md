# Pesquisa de Satisfação - TI

## DESCRICAO DOS DADOS

### TABELA FATO

#### FPESQUISA
* **ID_Processador**<br>
   Tipo de dados:
* **ID_Notificador**<br>
   Tipo de dados:
* **ID_SSI**<br>
   Tipo de dados:
* **Data_Criacao_SSI:** Data de abertura da SSI.<br>
   Tipo de dados:
* **Data_Encerramento_SSI:** Data de encerramento do chamado.<br>
   Tipo de dados:

### TABELAS DE DIMENSAO

#### DNOTIFICADOR: Armazena informacoes relativas ao notificador (pessoa que abre a SSI).<br>
* **ID_Notificador:** <br>
   Tipo de dados: Número Decimal
* **Nome:** <br>
   Tipo de dados: Texto
* **Departamento:** <br>
   Tipo de dados: Texto
* **Diretoria:** <br>
   Tipo de dados: Texto
* **Empresa:** <br>
   Tipo de dados: Texto

#### DSSI: Armazena informacoes relativas a SSI (chamado).<br>
* **ID_SSI:** <br>
   Tipo de dados: Número Decimal
* **SSI:** <br>
   Tipo de dados: Número Inteiro
* **Descricao:** <br>
   Tipo de dados: Texto

#### DPROCESSADOR: Armazena informacoes relativas ao processador (pessoa que atende a SSI).<br>
* **ID_Processador:** <br>
   Tipo de dado: Número Decimal
* **Nome:** <br>
   Tipo de dado: Texto
* **Equipe_suporte:** Infra, Sistemas, Suporte N1.<br>
   Tipo de dado: Texto

#### DRESPOSTA: Armazena informacoes referentes ao preenchimento da pesquisa de satisfacao.<br>
* **ID_SSI:** <br>
   Tipo de dado: Número Decimal
* **SSI:** (Necessário??)<br>
   Tipo de dado: Número Inteiro
* **Data_Resposta_Pesquisa:** <br>
   Tipo de dado:
* **Resolucao_Problema:** Seu problema foi resolvido neste atendimento? <br>
   Tipo de dado: Texto
* **Agilidade_Atendimento:** Quão ágil foi a resolução do seu atendimento?<br>
   Tipo de dado: Texto
* **Qualidade_Atendimento:** Quão bem atendido você foi?<br>
   Tipo de dado: Texto
* **Satisfacao_Atendimento:** De 1 a 5, quão satisfeito você está com o serviço prestado neste atendimento?<br>
   Tipo de dado: Número Inteiro
* **Comentários:** Compartilhe conosco o que achar importante.<br>
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

