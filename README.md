# Módulo 5 - Ficha de Trabalho FP02

Este repositório contém a resolução da Ficha de Trabalho FP02 do Módulo 5, que abrange conceitos básicos de **HTML** para a criação de formulários e **PHP** para o processamento de dados submetidos e manipulação de estruturas de dados.
## Estrutura do Projeto

O projeto é composto por dois ficheiros principais:

| Ficheiro | Descrição |
| :--- | :--- |
| `form.html` | Contém os formulários HTML para a submissão de dados para o Exercício 1 (lista de itens) e o Exercício 3 (cálculo de média). |
| `lista.php` | Ficheiro PHP responsável por receber os dados submetidos, processar a lógica dos exercícios e apresentar os resultados. |

## Funcionalidades Implementadas

O ficheiro `lista.php` implementa a lógica para três exercícios distintos:

### 1. Exercício 1: Lista de Itens

**Objetivo:** Receber 5 itens de texto de um formulário e apresentá-los numa lista não ordenada.

*   **Entrada:** 5 campos de texto (`item1` a `item5`) submetidos via método `POST` a partir de `form.html`.
*   **Processamento:** Os itens são recolhidos e armazenados num *array* em PHP.
*   **Saída:** Os itens são iterados e apresentados numa lista `<ul>` na página.

### 2. Exercício 2: Tabela de Turma

**Objetivo:** Apresentar uma lista de alunos e respetivas idades numa tabela HTML.

*   **Entrada:** Um *array* associativo `$turma` codificado no ficheiro `lista.php` com nomes de alunos e idades.
*   **Processamento:** O *array* é percorrido para gerar as linhas e colunas de uma tabela HTML.
*   **Saída:** Uma tabela HTML com duas colunas (Nome e Idade).

### 3. Exercício 3: Cálculo de Média e Classificação

**Objetivo:** Receber 5 notas, calcular a média e classificar o resultado com base em critérios definidos.

*   **Entrada:** 5 campos numéricos (`nota1` a `nota5`) submetidos via método `POST` a partir de `form.html`.
*   **Processamento:**
    *   As notas são somadas e a média é calculada.
    *   A classificação é determinada com base na seguinte lógica:
        *   Média < 10: **Reprovado**
        *   10 ≤ Média ≤ 13: **Satisfaz**
        *   14 ≤ Média ≤ 17: **Bom**
        *   Média > 17: **Excelente**
*   **Saída:** A média calculada e a classificação correspondente.

## Como Executar o Projeto

Uma vez que o projeto utiliza PHP, é necessário um ambiente de servidor web com suporte a PHP (como Apache ou Nginx).

### Pré-requisitos

*   Um servidor web local (por exemplo, XAMPP, MAMP, WAMP ou Laragon).
*   PHP instalado e configurado.

### Passos de Execução

1.  **Clone o repositório** (ou descompacte os ficheiros) para o diretório raiz do seu servidor web (ex: `htdocs` no XAMPP).
2.  **Aceda ao formulário** no seu navegador, navegando para o caminho do ficheiro `form.html` no seu servidor local (ex: `http://localhost/m5-fp02/form.html`).
3.  **Preencha os formulários** e clique em "Enviar" para que o ficheiro `lista.php` processe os dados e apresente os resultados.
