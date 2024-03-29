# Pesquisa de Satisfação - TI - Power BI
---

### INTRODUÇÃO E MOTIVAÇÃO
---
O setor de TI visa colaborar com a melhoria do atendimento de solicitações e incidentes para uma empresa melhor. Sabendo-se dos desafios para gerenciar o atendimento dentro de uma empresa e visando unir as informações relativas a funcionários, departamentos, diretorias, SSI's e respostas da pesquisa de satisfação em um mesmo local, ficamos motivados com o desenvolvimento do projeto. O projeto "Pesquisa de Satisfação - TI - Power BI" tem como objetivo gerenciar todas as informações das atividades de atendimento do setor de TI. Deverá gerar um conjunto de relatórios que por sua vez atenderá os anseios da empresa.

### INFORMAÇÕES
---
O projeto proposto conterá as informações aqui detalhadas. Dos notificadores serão armazenados o nome, departamento, diretoria e empresa. Das SSI's serão armazenados o número e a descrição. Dos processadores serão armazenados o nome e a equipe de suporte. Cada SSI pode ter vários processadores auxiliando no seu atendimento e cada processador pode estar envolvido em vários atendimentos. Os dados relativos a pesquisa de satisfação que serão armazenados são as respostas para 4 perguntas do formulário e comentário(opcional) respondidos pelo notificador. É importante destacar que cada SSI atendida gera um link para responder a pesquisa, e o processador avaliado será o que encerrou a SSI. Um notificador também pode abrir várias SSI's, caso seja necessário, mas não precisa obrigatoriamente responder a todas pesquisas.


### QUAIS PERGUNTAS PODEM SER RESPONDIDAS?
---
* **Principais Relatórios:**
    - Indice de resolução do problema atendido pelo setor de TI.
    - Indice de resolucao do problema atendido por cada equipe de suporte.
    - Indice de agilidade no atendimento do setor de TI.
    - Indice de agilidade no atendimento por equipe de suporte.
    - Indice de qualidade no atendimento do setor de TI.
    - Indice de qualidade no atendimento por equipe de suporte.
    - Indice de satisfação no atendimento do setor de TI.
    - Indice de satisfação no atendimento por equipe de suporte.
    - Quantidade de pesquisas respondidas por cada setor.
    - Quantidade de SSI's abertas/ encerradas por cada setor.
    - Notificadores que mais respondem pesquisa de satisfação.
    - Processadores melhores avaliados pelo atendimento.
 
### TABELA DE DADOS 

* [Formulário](https://www.google.com.br/)
* [Tabela](https://www.google.com.br/)


### DESCRIÇÃO DOS DADOS
---
#### TABELA FATO

##### FPESQUISA
* **ID_Processador:** Identificador do processador.<br>
    - Tipo de dados: Número Decimal.
* **ID_Notificador:** Identificador do notificador.<br>
    - Tipo de dados: Número Decimal.
* **ID_SSI:** Identificador da SSI(chamado).<br>
    - Tipo de dados: Número Decimal.
* **Data_Criacao_SSI:** Armazena a data que a SSI foi aberta.<br>
    - Tipo de dados: Qualquer.
* **Data_Encerramento_SSI:** Armazena a data que a SSI foi encerrada.<br>
    - Tipo de dados: Qualquer.

#### TABELAS DE DIMENSÃO

##### DNOTIFICADOR: Armazena informacoes relativas ao notificador (pessoa que abre a SSI).<br>
* **ID_Notificador:** Identificador do notificador.<br>
    - Tipo de dados: Número Decimal.
* **Nome:** Armazena nome do notificador.<br>
    - Tipo de dados: Texto.
* **Departamento:** Armazena o departamento que o usuário pertence.<br>
    - Tipo de dados: Texto.
* **Diretoria:** Armazena a diretoria que o funcionário trabalha.<br>
    - Tipo de dados: Texto.
* **Empresa:** Armazena nome da empresa.<br>
    - Tipo de dados: Texto.

##### DSSI: Armazena informacoes relativas a SSI (chamado).<br>
* **ID_SSI:** Identificador da SSI.<br>
    - Tipo de dados: Número Decimal.
* **SSI:** Armazena o número da SSI aberta. <br>
    - Tipo de dados: Número Inteiro.
* **Descricao:** Descreve a SSI.<br>
    - Tipo de dados: Texto.

##### DPROCESSADOR: Armazena informacoes relativas ao processador (pessoa que atende a SSI).<br>
* **ID_Processador:** Identificador do processador.<br>
    - Tipo de dados: Número Decimal.
* **Nome:** Armazena nome do funcionário.<br>
    - Tipo de dados: Texto.
* **Equipe_suporte:** Armazena a equipe que o processador faz parte. Infra, Sistemas ou Suporte N1.<br>
    - Tipo de dados: Texto.

##### DRESPOSTA: Armazena informacoes referentes ao preenchimento da pesquisa de satisfacao.<br>
* **ID_SSI:** Identificador da SSI.<br>
    - Tipo de dados: Número Decimal.
* **SSI:** (Necessário??)<br>
    - Tipo de dados: Número Inteiro.
* **Data_Resposta_Pesquisa:** Armazena a data em que a pesquisa foi respondida.<br>
    - Tipo de dados: Qualquer.
* **Resolucao_Problema:** Seu problema foi resolvido neste atendimento? <br>
    - Tipo de dados: Texto.
* **Agilidade_Atendimento:** Quão ágil foi a resolução do seu atendimento?<br>
    - Tipo de dados: Texto.
* **Qualidade_Atendimento:** Quão bem atendido você foi?<br>
    - Tipo de dados: Texto.
* **Satisfacao_Atendimento:** De 1 a 5, quão satisfeito você está com o serviço prestado neste atendimento?<br>
    - Tipo de dados: Número Inteiro.
* **Comentários:** Compartilhe conosco o que achar importante.<br>
    - Tipo de dados: Texto.


#### DCALENDARIO:
* **Data:** DD/MM/AAAA<br>
    - Tipo de dados: Qualquer.
* **Ano:** AAAA<br>
    - Tipo de dados: Número Inteiro.
* **Dia:** DD<br>
    - Tipo de dados: Número Inteiro.
* **Mes:** MM<br>
    - Tipo de dados: Número Inteiro.
* **Mes/Ano:** MM/AAAA<br>
    - Tipo de dados: Texto.


### MODELO DIMENSIONAL
---
#### STAR SCHEMA

![Alt text](https://github.com/danielasalomao/pesquisa/blob/v1/Star_Schema.png)

