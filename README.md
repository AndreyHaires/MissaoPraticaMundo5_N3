# Missão Prática – Mundo 5 – Nível 3
**Andrey Haertel Aires** - Matrícula: 2021.07.22851-2  
**Polo:** Centro - Palhoça – SC  
**Disciplina:** RPG0033 - TRATANDO A IMENSIDÃO DOS DADOS  
**Turma:** T 9001 – 5º Semestre Letivo  

[**Github Repository**](https://github.com/AndreyHaires/MissaoPraticaMundo5_N3)

## Descrição do Projeto
Neste projeto, foi desenvolvido um conjunto de práticas utilizando a linguagem Python e a biblioteca Pandas para manipulação de dados. A missão envolve a leitura, limpeza e transformação de um conjunto de dados em formato CSV, a fim de preparar as informações para análises futuras.

## Estrutura do Projeto
- **Ambiente de Desenvolvimento:** PyCharm
- **Projeto:** missão_nivel3
- **Conjunto de Dados:** dados.csv

## Etapas do Projeto

### 1. Importação da Biblioteca
Foi importada a biblioteca Pandas e renomeada como `pd` para facilitar o uso.

### 2. Leitura do Arquivo CSV
O caminho do arquivo CSV foi definido na variável `file_path`, com os seguintes parâmetros:
- **Separador:** ponto e vírgula (`;`)
- **Engine:** `python` da biblioteca Pandas
- **Encoding:** `utf-8`
- **Armazenamento:** A variável `data` armazena os dados lidos.

### 3. Verificação dos Dados
Utilizando o método `.info()`, foi possível verificar o número de entradas, nomes das colunas, contagem de valores nulos e tipos de dados.

### 4. Visualização de Dados
As cinco primeiras e últimas linhas do conjunto de dados foram impressas utilizando os métodos:
- `print(data.head(5))`
- `print(data.tail(5))`

### 5. Cópia do Conjunto de Dados
Uma cópia do conjunto de dados original foi criada usando o método `.copy()`, armazenada na variável `data_copia`.

### 6. Tratamento de Valores Nulos
- **Coluna 'Calories':** Todos os valores nulos foram substituídos por `0` utilizando o método `.fillna(0)`.
- **Coluna 'Date':** Valores nulos foram substituídos por `1900/01/01` com o método `.fillna()`.

### 7. Correções de Valores Específicos
- O valor da linha 22 da coluna 'Date' foi alterado para `NaN` com o método `.replace()`.
- A linha 26 da coluna 'Date', que estava fora do padrão, foi corrigida.

### 8. Transformação de Dados
A coluna 'Date' foi transformada para o formato datetime usando o método `pd.to_datetime()`.

### 9. Remoção de Registros Nulos
Os registros contendo valores nulos foram removidos com o método `.dropna()`.

### 10. Resultado Final
O DataFrame `data_copia` foi impresso, apresentando os dados após todas as alterações e limpezas.

## Conclusão
Este projeto proporcionou uma prática abrangente em manipulação de dados utilizando Python e Pandas, fundamental para futuras análises de dados.
