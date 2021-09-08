**<h1>Challenge de BI - 1ª Semana - Alura</h1>**
<br>
<h2>Dashboard de Logística</h2>
<p>A pessoa que gerencia a área de logística da AluraShop está enfrentando algumas mudanças em sua área por conta do aumento da demanda dos serviços de logística no período da pandemia. 
Ela quer manter a qualidade de seu serviço, mas para isso precisa acompanhar constantemente as métricas do seu departamento para tomar as melhores decisões.</p>
<br>
<h2>Base de Dados</h2>
<p>A base de dados consiste em quatro arquivos csv com a seguinte estrutura:</p>

<p><b>Tabela Pedidos</b></p>
<ul>
<li>Data do pedido
<li>Data de entrega
<li>Data previsão entrega
<li>ID pedido
<li>Latitude
<li>Longitude
<li>UF da entrega
<li>ID Produto
<li>Quantidade
<li>ID veículo
</ul>

<p><b>Tabela Produtos</b></p>
<ul>
<li>ID Produto
<li>Categoria Produto
<li>Valor
</ul>

<p><b>Tabela Estoque</b></p>
<ul>
<li>ID produto
<li>Data atualização
<li>Quantidade
</ul>

<p><b>Tabela Veículos<p></b>
<ul>
<li>ID veículo
<li>Tipo
<li>Status
</ul>

<p>A tabela de pedidos e estoque são tabelas de fatos e as restantes são dimensões.

<br>

<h1>Ferramentas Utilizadas no Projeto</h1>
<p>Foi utilizado apenas o Power BI para o desenvolvimento do Dashboard e uma paleta de cores para tornar o dashboard acessível a pessoas que possuem daltonismo</p>

<br>

<h1>Tratamento dos Dados</h1>
<p><b>Tabela Pedidos</b></p>
<ul>
<li>Alteração na tipagem dos dados, colocado a tipagem correta
<li>Transformação da coluna 'data previsão' em data.
</ul>

<p><b>Tabela Produtos</b></p>
<ul>
<li>Alteração na tipagem dos dados, colocado a tipagem correta
<li>Separação do ID e Categoria, criando uma coluna nova
<li>Remoção do Underscore
<li>Primeira letra de cada palavra maiúscula na coluna 'categoria'
</ul>

<p><b>Tabela Estoque</b></p>
<ul>
<li>Alteração na tipagem dos dados, colocado a tipagem correta
<li>Ajuste da coluna 'data atualização'
</ul>

<p><b>Tabela Veículos<p></b>
<ul>
<li>Alteração na tipagem dos dados, colocado a tipagem correta
</ul>

<br>

<h1>Métricas</h1>
<ul>
<li>Entregas no prazo
<li>Entregas atrasadas
<li>Veículos disponíveis para entrega
<li>S2D - Ship to door
<li>Índice de ocorrências por estado
<li>Média do estoque
<li>Estoque disponível por Categoria  
</ul>

<br>

<h1>Relacionamentos</h1>

<ul>
<li>Pedidos(n) - (1)Produtos = muitos para um (n-1)
<li>Pedidos(n) - (1)Veiculos = muitos para um (n-1)
<li>Produtos(1) - (n)Estoque = um para muitos (1-n)
</ul>

<br>

<h1>Link do Dashboard</h1>
https://app.powerbi.com/view?r=eyJrIjoiYjZhN2UwNWItMzlmNC00MTU2LWIxMTMtMGNlYzRiMjczYjlmIiwidCI6Ijk0NjZmMmYwLTI4ZmQtNDYxMi04MjhkLTQ0YzdlNzU4MDA3OCJ9
