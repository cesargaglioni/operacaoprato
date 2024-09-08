Este repositório contém o código utilizado para realizar uma análise exploratória de dados (EDA) sobre os avistamentos de OVNIs relatados na Operação Prato, uma das investigações mais conhecidas sobre fenômenos aéreos no Brasil.

Descrição
A análise visa explorar características dos avistamentos de OVNIs, focando em detalhes como formas, cores, e sua distribuição geográfica e temporal. O objetivo principal é identificar padrões e correlações entre os dados observados e visualizar de maneira clara a frequência de avistamentos com determinadas características.

Estrutura do Repositório
bash
Copiar código
.
├── dados-op.csv                # Arquivo de dados dos avistamentos de OVNIs
├── analise_formas_cores.ipynb   # Notebook Jupyter com a análise de formas e cores de OVNIs
├── analise_geografica.ipynb     # Notebook Jupyter com a análise geográfica (mapas de calor e distribuição por estado)
├── README.md                    # Este arquivo
├── requirements.txt             # Dependências do projeto
Arquivo de Dados
dados-op.csv: Contém os relatos de avistamentos de OVNIs, com colunas como REG Nº, CIDADE, ESTADO, FORMA (TAXONOMIA), COR (TAXONOMIA), LATITUDE, LONGITUDE, entre outras.
Análises Realizadas
Distribuição Temporal dos Relatos:

Análise da frequência de avistamentos ao longo do tempo, observando padrões por ano, mês, e hora do dia.
Análise de Formas e Cores:

Contagem e visualização das formas e cores relatadas de OVNIs, usando as colunas FORMA (TAXONOMIA) e COR (TAXONOMIA). Foram removidos valores irrelevantes para a análise geométrica (como descrições narrativas) para focar em dados objetivos.
Gráficos de barras com a frequência de cada forma e cor, além de gráficos de calor para analisar correlações.
Análise Geográfica:

Geração de mapas interativos com a distribuição de avistamentos por estados e cidades, além de mapas de calor utilizando coordenadas de latitude e longitude.
Filtragem de Valores Específicos:

Alguns valores fora do escopo da análise (descrições detalhadas demais ou ambíguas, como "Quadrada, semelhante ao automóvel OPALA (Cor opaca)") foram removidos para garantir a qualidade dos dados.
Como Usar
Clone o repositório:

bash
Copiar código
git clone https://github.com/seu-usuario/operacao-prato-analysis.git
Instale as dependências:

bash
Copiar código
pip install -r requirements.txt
Execute os notebooks:

Abra o Jupyter Notebook e execute os notebooks analise_formas_cores.ipynb e analise_geografica.ipynb para reproduzir a análise.
Opcional: Modifique o arquivo de dados dados-op.csv para incluir novas colunas ou ajustar os dados de entrada.

Dependências
As principais bibliotecas utilizadas incluem:

Pandas: Manipulação de dados
Seaborn: Visualização de dados
Matplotlib: Criação de gráficos
GeoPandas: Análise geográfica e visualização de mapas
Folium: Mapas interativos (para análises geográficas)
Jupyter Notebook: Para visualização e execução dos notebooks de análise
Para instalar todas as dependências, execute:

bash
Copiar código
pip install -r requirements.txt
Contribuindo
Se você deseja contribuir com o projeto, por favor, siga os seguintes passos:

Crie um fork do repositório.
Crie um branch com sua feature (git checkout -b minha-feature).
Faça commit das suas alterações (git commit -m 'Adicionei minha feature').
Envie para o branch (git push origin minha-feature).
Abra um Pull Request.
Licença
Este projeto está licenciado sob a licença MIT. Para mais detalhes, veja o arquivo LICENSE.

