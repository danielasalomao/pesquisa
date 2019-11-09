# Pesquisa de Satisfação - TI

## DESCRICAO DOS DADOS

### TABELA FATO

#### FPESQUISA
* **id_processador:**
* **id_notificador:**
* **id_ssi:**
* **data_criacao_ssi:** Data de abertura da SSI.<br>
* **data_encerramento_ssi:** Data de encerramento do chamado.<br>

### TABELAS DE DIMENSAO

#### DNOTIFICADOR: Armazena informacoes relativas ao notificador (pessoa que abre a SSI).<br>
* **id_notificador:** Número de identificacao do notificador.<br>
* **nome_notificador:** Nome do funcionário.<br>
* **departamento_notificador:** Departamento.<br>
* **diretoria_notificador:** Diretoria.<br>
* **empresa_notificador:** Empresa que o notificador trabalha.<br>

#### DSSI: Armazena informacoes relativas a SSI (chamado).<br>
* **id_ssi:** Código de identificacao da SSI.<br>
* **numero_ssi:** Número da SSI aberta.<br>
* **descricao_ssi:** Descricao do chamado.<br>

#### DPROCESSADOR: Armazena informacoes relativas ao processador (pessoa que atende a SSI).<br>
* **ID_Processador:** Número de identificacao do processador.<br>
* **Nome:** Nome.<br>
* **Equipe_suporte:** Equipe de suporte.<br>

#### DRESPOSTA: Armazena informacoes referentes ao preenchimento da pesquisa de satisfacao.<br>
* **Resolucao_problema:**<br>
* **Agilidade_atendimento:**<br>
* **Qualidade_atendimento:**<br>
* **Satisfacao_atendimento:**<br>
* **Data_resposta_pesquisa:**<br>
* **Comentários:** 

#### DCALENDARIO:
* **Ano:** AAAA
* **Data:** DD/MM/AAAA
* **Dia:** DD
* **Mes:** MM
* **Mes/Ano:** MM/AAAA


## MODELAGEM DIMENSIONAL

### MODELO STAR SCHEMA

![Alt text](https://github.com/danielasalomao/pesquisa/blob/v1/Star_Schema.png)

