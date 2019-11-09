# Pesquisa de Satisfação - TI

## DESCRICAO DOS DADOS

### TABELA FATO

#### FPESQUISA
* **ID_Processador:**
* **ID_Notificador:**
* **ID_SSI:**
* **Data_Criacao_SSI:** Data de abertura da SSI.<br>
* **Data_Encerramento_SSI:** Data de encerramento do chamado.<br>

### TABELAS DE DIMENSAO

#### DNOTIFICADOR: Armazena informacoes relativas ao notificador (pessoa que abre a SSI).<br>
* **ID_Notificador
* **Nome
* **Departamento
* **Diretoria:**
* **Empresa:

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

