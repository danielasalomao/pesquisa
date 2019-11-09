# Pesquisa de Satisfação - TI

## QUAIS PERGUNTAS PODEM SER RESPONDIDAS?

Principais Relatórios:

* **Relatório da frequência geral dos alunos por disciplina, incluindo as seguintes informações:** campus

## DESCRICAO DOS DADOS

### TABELA FATO

#### FPESQUISA
* **ID_Processador:** Identificador do processador.<br>
   Tipo de dados: Número Decimal.
* **ID_Notificador:** Identificador do notificador.<br>
   Tipo de dados: Número Decimal.
* **ID_SSI:** Identificador da SSI(chamado).<br>
   Tipo de dados: Número Decimal.
* **Data_Criacao_SSI:** Armazena a data que a SSI foi aberta.<br>
   Tipo de dados: Qualquer.
* **Data_Encerramento_SSI:** Armazena a data que a SSI foi encerrada.<br>
   Tipo de dados: Qualquer.

### TABELAS DE DIMENSAO

#### DNOTIFICADOR: Armazena informacoes relativas ao notificador (pessoa que abre a SSI).<br>
* **ID_Notificador:** Identificador do notificador.<br>
   Tipo de dados: Número Decimal.
* **Nome:** Armazena nome do notificador.<br>
   Tipo de dados: Texto.
* **Departamento:** Armazena o departamento que o usuário pertence.<br>
   Tipo de dados: Texto.
* **Diretoria:** Armazena a diretoria que o funcionário trabalha.<br>
   Tipo de dados: Texto.
* **Empresa:** Armazena nome da empresa.<br>
   Tipo de dados: Texto.

#### DSSI: Armazena informacoes relativas a SSI (chamado).<br>
* **ID_SSI:** Identificador da SSI.<br>
   Tipo de dados: Número Decimal.
* **SSI:** Armazena o número da SSI aberta. <br>
   Tipo de dados: Número Inteiro.
* **Descricao:** Descreve a SSI.<br>
   Tipo de dados: Texto.

#### DPROCESSADOR: Armazena informacoes relativas ao processador (pessoa que atende a SSI).<br>
* **ID_Processador:** Identificador do processador.<br>
   Tipo de dados: Número Decimal.
* **Nome:** Armazena nome do funcionário.<br>
   Tipo de dados: Texto.
* **Equipe_suporte:** Armazena a equipe que o processador faz parte. Infra, Sistemas ou Suporte N1.<br>
   Tipo de dados: Texto.

#### DRESPOSTA: Armazena informacoes referentes ao preenchimento da pesquisa de satisfacao.<br>
* **ID_SSI:** Identificador da SSI.<br>
   Tipo de dados: Número Decimal.
* **SSI:** (Necessário??)<br>
   Tipo de dados: Número Inteiro.
* **Data_Resposta_Pesquisa:** Armazena a data em que a pesquisa foi respondida.<br>
   Tipo de dados: Qualquer.
* **Resolucao_Problema:** Seu problema foi resolvido neste atendimento? <br>
   Tipo de dados: Texto.
* **Agilidade_Atendimento:** Quão ágil foi a resolução do seu atendimento?<br>
   Tipo de dados: Texto.
* **Qualidade_Atendimento:** Quão bem atendido você foi?<br>
   Tipo de dados: Texto.
* **Satisfacao_Atendimento:** De 1 a 5, quão satisfeito você está com o serviço prestado neste atendimento?<br>
   Tipo de dados: Número Inteiro.
* **Comentários:** Compartilhe conosco o que achar importante.<br>
   Tipo de dados: Texto.


#### DCALENDARIO:
* **Data:** DD/MM/AAAA<br>
   Tipo de dados: Qualquer.
* **Ano:** AAAA<br>
   Tipo de dados: Número Inteiro.
* **Dia:** DD<br>
   Tipo de dados: Número Inteiro.
* **Mes:** MM<br>
   Tipo de dados: Número Inteiro.
* **Mes/Ano:** MM/AAAA<br>
   Tipo de dados: Texto.


## MODELAGEM DIMENSIONAL

### MODELO STAR SCHEMA

![Alt text](https://github.com/danielasalomao/pesquisa/blob/v1/Star_Schema.png)

