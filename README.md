🚀 Funcionalidades

Leitura de Dados: Importa informações de clientes (Nome, CPF, Valor, Vencimento) de um arquivo dados_cpf.xlsx.

Automação Web: Utiliza Selenium para navegar e interagir com a aplicação web de consulta de CPF desenvolvida em OutSystems (https://gabriel-bueno.outsystemscloud.com/ConsultaCpf/).

Consulta de Status: Insere o CPF de cada cliente no campo de pesquisa e aciona o botão para verificar o status.

Coleta de Informações: Captura o status de pagamento (e, se "Em Dia", a data e método de pagamento).

Geração de Relatório: Salva todas as informações processadas em uma nova planilha Planilha_fechamento.xlsx, incluindo o status final e detalhes de pagamento.

⚙️ Utilizações

Python: Linguagem principal do script.

Selenium WebDriver: Para automação da interação com o navegador web.

OpenPyXL: Para leitura e escrita de dados em arquivos Excel.

Google Chrome: Navegador utilizado para a automação (requer ChromeDriver compatível).

OutSystems: A plataforma low-code na qual o sistema de consulta de CPF foi desenvolvido.

💻 Como Usar

Pré-requisitos
Certifique-se de ter o Python instalado e as seguintes bibliotecas:

pip install selenium openpyxl
Você também precisará do ChromeDriver compatível com a sua versão do Google Chrome.

Configuração
dados_cpf.xlsx: Crie uma planilha Excel com o nome dados_cpf.xlsx na mesma pasta do script. Ela deve conter as colunas: Nome, cpf, valor e vencimento (na primeira linha).

Exemplo:
| Nome  | cpf         | valor | vencimento |
| :---- | :---------- | :---- | :--------- |
| João  | 123.456.789-01 | 100.00 | 2023-12-31 |
| Maria | 987.654.321-09 | 50.50 | 2024-01-15 |

Planilha_fechamento.xlsx: O script criará ou atualizará este arquivo. Se não existir, ele será gerado automaticamente.

Execução
Basta executar o script Python:

python seu_script_principal.py
O navegador Chrome será aberto automaticamente, e o script começará a processar os CPFs. Ao finalizar, o arquivo Planilha_fechamento.xlsx será salvo com os resultados.
