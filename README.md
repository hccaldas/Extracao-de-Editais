# Extração de Editais do PNCP

Este projeto realiza a extração de dados de editais disponíveis na API do Portal Nacional de Contratações Públicas (PNCP) e salva os resultados em um arquivo Excel.

## Funcionalidades

- Faz requisições à API do PNCP para buscar editais.
- Extrai informações como título, descrição e link dos editais.
- Suporta paginação para coletar dados de várias páginas.
- Salva os dados extraídos em um arquivo Excel (`editais_pncp.xlsx`).

## Requisitos

- Python 3.7 ou superior
- Bibliotecas Python:
  - `requests`
  - `pandas`
  - `openpyxl` (para salvar o arquivo Excel)

## Instalação

1. Clone este repositório ou copie os arquivos para o seu ambiente local.
2. Instale as dependências necessárias:
   ```bash
   pip install requests pandas openpyxl


  Como Usar

  python extração.py

O script fará requisições à API do PNCP e salvará os dados extraídos em um arquivo Excel chamado editais_pncp.xlsx.
Estrutura do Projeto

    extração.py: Script principal que realiza a extração de dados e salva no Excel.
    editais_pncp.xlsx: Arquivo Excel gerado com os dados extraídos.

Personalização
    
Para alterar o número de páginas a serem extraídas, edite a seguinte linha no código:

    if pagina > 5:  # Limitar a 5 páginas
    break
    
Substitua 5 pelo número desejado de páginas.

Para ajustar os campos extraídos, edite as chaves acessadas no JSON:

Exemplo de Saída
O arquivo Excel gerado (editais_pncp.xlsx) terá o seguinte formato:

Título	Descrição	Link
Edital nº 16/2025	Registro de preço para aquisição de materiais esportivos	https://pncp.gov.br/compras/01616270000194/2025/16
Aviso de Contratação Direta nº 13/2025	Contratação de empresa para execução de concurso público	https://pncp.gov.br/compras/15389596000130/2025/11
Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

Licença
Este projeto está licenciado sob a licença MIT. Consulte o arquivo LICENSE para mais informações.


  
