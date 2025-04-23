<h1>📊 Dashboard de Vendas - BikeWorld</h1>

<p>A <strong>BikeWorld</strong> é uma empresa brasileira que nasceu da paixão por pedalar. Fundada por dois amigos ciclistas, ela rapidamente se tornou referência na venda de bicicletas e acessórios esportivos, atendendo clientes em todo o país.</p>

<p>Com o crescimento acelerado, surgiram dúvidas estratégicas fundamentais:</p>
<ul>
  <li>Quem são nossos clientes mais valiosos?</li>
  <li>Qual vendedor está realmente performando?</li>
  <li>Quais produtos devem ser priorizados em campanhas?</li>
  <li>Existe sazonalidade no nosso faturamento?</li>
</ul>

<p>Para responder a essas perguntas, foi desenvolvido um <strong>dashboard interativo</strong> usando Power BI, consolidando dados de vendas, clientes, produtos e performance comercial. Todos os dados foram organizados e extraídos a partir de um banco de dados <strong>PostgreSQL</strong>, garantindo robustez e confiabilidade nas análises.</p>

<section>
  <h2>🧩 Como os dados estão organizados?</h2>
  <img src="./relacionamento.png" alt="Modelo de Relacionamento entre Tabelas">
  <p>O modelo de dados utilizado para construir o dashboard foi estruturado no formato de <strong>Data Warehouse</strong>, utilizando o banco de dados <strong>PostgreSQL</strong>. Ele segue a abordagem de esquema estrela, onde a tabela de fatos <code>fato_vendas</code> centraliza as informações de vendas e se conecta a diversas tabelas dimensionais.</p>
  <p>As principais tabelas são:</p>
  <ul>
    <li><strong>fato_vendas</strong>: contém as métricas de vendas, como quantidade, desconto, valor total e chaves para cliente, produto, vendedor e tempo.</li>
    <li><strong>dimensao_cliente</strong>: armazena dados dos clientes, como nome, sexo, estado e status.</li>
    <li><strong>dimensao_produto</strong>: contém informações sobre os produtos vendidos.</li>
    <li><strong>dimensao_vendedor</strong>: traz os dados dos vendedores, essenciais para avaliar a performance individual.</li>
    <li><strong>dimensao_tempo</strong>: facilita a análise temporal, organizando os dados por data, mês, dia da semana e ano.</li>
    <li><strong>cubo_vendas</strong>: estrutura agregada usada para análises específicas por produto, estado e cliente.</li>
    <li><strong>kpi</strong>: armazena metas e valores realizados por mês, permitindo avaliação de performance geral da empresa.</li>
  </ul>
  <p>Esse modelo relacional garante integridade e flexibilidade nas análises, permitindo que o Power BI realize cruzamentos e filtros dinâmicos entre diferentes perspectivas do negócio.</p>
</section>
  
<section>
  <h2>👥 Quem são nossos clientes?</h2>
  <img src="./clientes.png" alt="Dashboard Clientes">
  <p>O dashboard mostra que clientes com status <strong>Silver</strong> geram a maior parte da receita da BikeWorld. Isso sugere que o foco em fidelização vale a pena. A distribuição de gênero é quase igual, com leve predominância masculina. <strong>Diana Baptista</strong> aparece como a principal compradora, sendo um ótimo exemplo de cliente premium. Geograficamente, os clientes estão concentrados nas regiões Sul e Sudeste, indicando um potencial para expansão em outras regiões.</p>
</section>

<section>
  <h2>🧑‍💼 Quais vendedores estão se destacando?</h2>
  <img src="./vendedores.png" alt="Dashboard Vendedores">
  <p>O vendedor <strong>Capitolino Bahia</strong> é o destaque absoluto em performance, liderando em volume de vendas mês após mês. Já <strong>Tobias Furtado</strong> tem desempenho inferior, o que pode indicar necessidade de treinamento ou realocação de tarefas. Observando os meses, percebemos uma clara sazonalidade, com picos de vendas concentrados em junho e novembro. Isso indica oportunidades para campanhas promocionais bem posicionadas.</p>
</section>

<section>
  <h2>🚲 Quais produtos mais vendem?</h2>
  <img src="./produtos.png" alt="Dashboard Produtos">
  <p>A <strong>Bicicleta Altools Stroll Aro 26</strong> lidera as vendas, combinando preço competitivo e promoções frequentes. Produtos com maior desconto tendem a ter melhor desempenho, evidenciando a sensibilidade do cliente ao preço. Em contraste, modelos como a <strong>Gometws Endorphine 6.1</strong>, com preço elevado e poucos descontos, tiveram menor saída. Essas informações orientam tanto o planejamento do mix de produtos quanto a precificação.</p>
</section>

<section>
  <h2>📈 Quando mais vendemos?</h2>
  <img src="./vendas.png" alt="Dashboard Vendas">
  <p>A curva de vendas revela picos nos meses de <strong>junho e julho</strong>, coincidindo com campanhas sazonais e maior procura por atividades ao ar livre no inverno. Produtos com ticket médio mais alto se mantêm estáveis ao longo do ano, enquanto itens mais acessíveis são mais sensíveis à sazonalidade. Isso permite à BikeWorld planejar estoques e campanhas de maneira estratégica.</p>
</section>

<p>📝 Com este dashboard, a BikeWorld passou a tomar decisões mais assertivas, baseadas em dados. Ele se tornou uma ferramenta essencial para o planejamento comercial, marketing e gestão de estoque. Um pedal mais seguro rumo ao crescimento 🚴‍♂️.</p>
</body>
</html>
