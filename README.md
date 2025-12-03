# 🔍 Automação de Consulta de Status de CPF (RPA Web)

Este script Python foi desenvolvido para automatizar a consulta de status de pagamento de clientes em um sistema web, utilizando dados de uma planilha Excel e gerando um relatório final detalhado.

---

## 🚀 Funcionalidades Principais

O script executa um ciclo de automação web, integrando dados de entrada e saída:

* **Leitura de Dados**: Importa as informações de clientes (Nome, CPF, Valor e Vencimento) do arquivo **`dados_cpf.xlsx`**.
* **Automação Web**: Utiliza o **Selenium WebDriver** para navegar e interagir com a aplicação de consulta de CPF desenvolvida em OutSystems (URL: `https://gabriel-bueno.outsystemscloud.com/ConsultaCpf/`).
* **Consulta de Status**: Insere o **CPF** de cada cliente no campo de pesquisa da aplicação web e aciona o botão de consulta.
* **Coleta de Informações**: Captura o status de pagamento exibido na tela e, se o status for "**Em Dia**", extrai também a data e o método de pagamento correspondentes.
* **Geração de Relatório**: Salva todas as informações processadas em uma nova planilha chamada **`Planilha_fechamento.xlsx`**, incluindo o status final e os detalhes do pagamento.

---

## ⚙️ Tecnologias Utilizadas

Esta solução de automação é construída sobre as seguintes ferramentas e plataformas:

* **Python**: A linguagem de programação principal do script.
* **Selenium WebDriver**: Framework essencial para a automação da interação com o navegador web (cliques, preenchimento de campos, navegação).
* **OpenPyXL**: Biblioteca para manipulação de arquivos Excel, usada tanto para a leitura do arquivo de entrada (`dados_cpf.xlsx`) quanto para a escrita do relatório final (`Planilha_fechamento.xlsx`).
* **Google Chrome**: O navegador utilizado para a automação (requer o **ChromeDriver** compatível).
* **OutSystems**: A plataforma low-

* 
