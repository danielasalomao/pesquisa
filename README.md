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
* **ID_Notificador:** Número Decimal
* **Nome:** Texto
* **Departamento:** Texto
* **Diretoria:** Texto
* **Empresa:** Texto

#### DSSI: Armazena informacoes relativas a SSI (chamado).<br>
* **ID_SSI:** Número Decimal.
* **SSI:** Número Inteiro.
* **Descricao:** Texto.

#### DPROCESSADOR: Armazena informacoes relativas ao processador (pessoa que atende a SSI).<br>
* **ID_Processador:** Número Decimal.
* **Nome:** Texto.
* **Equipe_suporte:** Texto ; Infra, Sistemas, Suporte N1.

#### DRESPOSTA: Armazena informacoes referentes ao preenchimento da pesquisa de satisfacao.<br>
* **ID_SSI:** Número Decimal
* **SSI:** Número Inteiro (Necessário??)
* **Data_Resposta_Pesquisa:** 
* **Resolucao_Problema:** Texto ; Seu problema foi resolvido neste atendimento? 
* **Agilidade_Atendimento:** Texto ; Quão ágil foi a resolução do seu atendimento?
* **Qualidade_Atendimento:** Texto ; Quão bem atendido você foi?
* **Satisfacao_Atendimento:** Número Inteiro ; De 1 a 5, quão satisfeito você está com o serviço prestado neste atendimento?
* **Comentários:** Texto ; Compartilhe conosco o que achar importante.


#### DCALENDARIO:
* **Ano:** AAAA
* **Data:** DD/MM/AAAA
* **Dia:** DD
* **Mes:** MM
* **Mes/Ano:** MM/AAAA


## MODELAGEM DIMENSIONAL

### MODELO STAR SCHEMA

![Alt text](https://github.com/danielasalomao/pesquisa/blob/v1/Star_Schema.png)

