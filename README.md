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
* **ID_Notificador**
* **Nome**
* **Departamento**
* **Diretoria**
* **Empresa**

#### DSSI: Armazena informacoes relativas a SSI (chamado).<br>
* **ID_SSI:** Código de identificacao da SSI.<br>
* **SSI:** Número da SSI aberta.<br>
* **Descricao:** Descricao do chamado.<br>

#### DPROCESSADOR: Armazena informacoes relativas ao processador (pessoa que atende a SSI).<br>
* **ID_Processador:** Número de identificacao do processador.<br>
* **Nome:** Nome.<br>
* **Equipe_suporte:** Equipe de suporte.<br>

#### DRESPOSTA: Armazena informacoes referentes ao preenchimento da pesquisa de satisfacao.<br>
* **ID_SSI**
* **SSI** (Necessário?)
* **Data_Resposta_Pesquisa** 
* **Resolucao_Problema:** Seu problema foi resolvido neste atendimento? 
* Tipo de Dado: Texto
* **Agilidade_Atendimento:** Quão ágil foi a resolução do seu atendimento?
* **Qualidade_Atendimento:** Quão bem atendido você foi?
* **Satisfacao_Atendimento:** De 1 a 5, quão satisfeito você está com o serviço prestado neste atendimento?
* **Comentários:** Compartilhe conosco o que achar importante.


#### DCALENDARIO:
* **Ano:** AAAA
* **Data:** DD/MM/AAAA
* **Dia:** DD
* **Mes:** MM
* **Mes/Ano:** MM/AAAA


## MODELAGEM DIMENSIONAL

### MODELO STAR SCHEMA

![Alt text](https://github.com/danielasalomao/pesquisa/blob/v1/Star_Schema.png)

