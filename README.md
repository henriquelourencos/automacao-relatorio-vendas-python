# Automação de Sistemas e Processos com Python

## Sobre o projeto

Este projeto consiste em uma automação desenvolvida em Python com o objetivo de otimizar o processo de geração e envio de relatórios de vendas.

A proposta é automatizar uma atividade que normalmente seria realizada manualmente: acessar uma base de dados no Google Drive, baixar uma planilha Excel, calcular indicadores de vendas e enviar os resultados por e-mail.

O projeto foi desenvolvido como exercício prático de aplicação dos conhecimentos em Python e automação de processos.

## Funcionalidades

- Abertura automatizada do navegador Google Chrome.
- Acesso ao Google Drive.
- Localização e download da planilha de vendas.
- Leitura e processamento dos dados utilizando Pandas.
- Cálculo do faturamento total.
- Cálculo da quantidade de produtos vendidos.
- Preparação e envio automático de relatório pelo Gmail.

## Tecnologias e bibliotecas

| Tecnologia | Utilização |
|---|---|
| Python | Linguagem principal |
| PyAutoGUI | Automação de mouse e teclado |
| Pandas | Manipulação e análise de dados |
| Pyperclip | Manipulação da área de transferência |
| OpenPyXL | Leitura de arquivos Excel |
| Time | Controle de intervalos na execução |
| Pathlib | Localização do arquivo no computador |

## Como funciona

O processo é dividido em cinco etapas:

1. **Acesso ao Google Drive:** o navegador é aberto automaticamente e direcionado à pasta com os dados de vendas.
2. **Download da planilha:** o PyAutoGUI realiza a navegação e o download do arquivo Excel.
3. **Leitura dos dados:** o Pandas importa a planilha para análise.
4. **Cálculo dos indicadores:** são calculados o faturamento total e a quantidade de produtos vendidos.
5. **Envio do relatório:** o Python prepara o conteúdo e automatiza o envio pelo Gmail.

## Instalação

Clone este repositório:

```bash
git clone URL_DO_SEU_REPOSITORIO
```

Instale as dependências:

```bash
pip install pandas pyautogui pyperclip openpyxl
```

## Configuração e execução

Abra o arquivo `Projeto_Inicial.ipynb` utilizando o Jupyter Notebook ou VS Code.

Antes de executar, verifique:

- Se o link do Google Drive foi configurado corretamente na variável `link`.
- Se o Chrome está configurado para baixar arquivos na pasta Downloads do Windows.
- Se o arquivo Excel será salvo com o nome `Vendas - Dez.xlsx`.
- Se o endereço de e-mail de destino está configurado corretamente.
- Se as coordenadas do PyAutoGUI correspondem à resolução e à organização da sua tela.
- Se o Google Drive e o Gmail estão acessíveis no navegador.

O código utiliza `Pathlib` para localizar automaticamente a pasta Downloads do usuário e acessar a planilha baixada.

## Limitações conhecidas

A automação utiliza coordenadas fixas de mouse e teclado para interagir com o navegador. Portanto, mudanças na resolução da tela, na interface dos serviços ou na posição das janelas podem exigir ajustes no código.

Além disso, o arquivo Excel precisa estar disponível na pasta Downloads com o nome esperado pelo código.

## Objetivo de aprendizado

Este projeto faz parte da minha evolução prática em Python, com foco em automação de tarefas, manipulação de dados e integração de diferentes ferramentas para resolver problemas do cotidiano.

---

**Desenvolvido por Henrique Lourenço**

[GitHub](https://github.com/henriquelourencos)