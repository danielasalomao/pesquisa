# Pesquisa de Satisfação - TI

## 5.2 DECISÕES DE PROJETO

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
* **id_processador:** Número de identificacao do processador.<br>
* **nome_processador:** Nome.<br>
* **equipe_suporte_processador:** Equipe de suporte.<br>

#### DRESPOSTA: Armazena informacoes referentes ao preenchimento da pesquisa de satisfacao.<br>
* **pesquisa_resolucao_problema:**<br>
* **pesquisa_agilidade_resolucao:**<br>
* **pesquisa_qualidade_atendimento:**<br>
* **pesquisa_nivel_satisfacao:**<br>
* **pesquisa_data_resposta:**<br>
* **pesquisa_comentario:** 

#### DCALENDARIO:





![Alt text]https://github.com/danielasalomao/pesquisa/blob/v2/Modelo_Star_Schema.png

