<h1> Modelagem de banco de dados - entidades, relacionamentos e atributos: </h1>

<h1> Aula 01: Banco de Dados </h1>
<p> A modelagem de dados é um processo onde se tem a concepção dos dados. Os dados são levantados, tratados e estruturados para, assim ter uma boa base para a construção do banco de dados e evitar diversos problemas.</p>
 
<h2> <b> Modelagem Conceitual: </b> </h2>
<p>• Baseia-se no mais <b>alto nível</b> e deve ser usada para entender os requisitos do sistema, pois explora as estruturas e conceitos de negócio. </p>

<h2> <b> Modelagem Lógica: </b> </h2>
<p>• É criado para realizar a descrição de como os dados serão armazenados no sistema. Nesse modelo, descrevemos as entidades, os atributos, as chaves primárias e estrangeiras e os seus relacionamentos.</p>

<h2> <b> Modelagem Física: </b> </h2>
<p>• É criado para descrever as tabelas, suas colunas e os relacionamentos. O modelo físico utiliza uma linguagem padrão para realizar sua representação: a linguagem SQL, utilizada para trabalhar com banco de dados relacionais.</p>

<h2> <b> SGBD: </b> </h2>
<p>• O SGBD (Sistema de gerenciamento de banco de dados) é frequentemente confundido com o próprio banco de dados. No entanto o SGBD é um sistema que gerencia os dados podendo incluir, alterar, ou até fazer consultas, através de uma interface mais amigável para o usuário. O SGBD trabalha mais perto do <b>baixo nível</b>.</p>

<hr>

<h2> <b>Software a ser utilizado: _BrModelo (Usei o Lucidchat online)</b> </h2>

<hr> <br>

<h1> Aula 02: Modelo entidade relacionamento </h1>

<h2> <b>Mini-mundo: </b> </h2>
<p> • Mini-mundo é considerado uma das etapas mais importantes do processo de modelagem dos dados, pois, através desta etapa, entendemos como o banco de dados será estruturado. Mini-mundo é uma abstração de uma pequena parte do mundo real, que é de grande interesse para uma aplicação.</p> 

<h2> <b>MER: </b> </h2>
<p> • O MER (Modelo Entidade Relacionamento) é um modelo conceitual usado para descrever os objetos (entidades) com suas características (atributos) e como elas se relacionam entre si (relacionamento).

<h2> <b>DER: </b> </h2>
<p> • O DER (Diagrama Entidade Relacionamento) é a representação gráfica do modelo conceitual (MER). O DER ajuda a visualizar as informações em  situações práticas.

<h2> <b>Importância da entrevista: </b> </h2>
<p> • Uma das etapas mais importantes do processo de modelagem de dados é a entrevista com os clientes, na qual serão identificadas as regras de negócio do projeto. A entrevista dará todo o direcionamento ao nosso projeto. Através dela, conhecemos todos os detalhes do negócio e podemos estruturar os próximos passos. </p>

<hr> <br>

<h1> Aula 03: Entidades </h1>

<h2> <b> O que são Entidades? </b> </h2>
<p> • A Entidade é um objeto único no mundo real, pode ser tanto um objeto, quanto uma pessoa. Podemos ter entidades abstratas ou concretas. Clientes e Carros são concretos, já um Departamento de Vendas é abstrato. </p>

<h2> <b> Diferença entre Entidade forte e fraca: </b> </h2>
<p> • A Entidade Forte existe independentemente de outra entidade, já a fraca depende de uma outra entidade. Exemplo: Em uma empresa com funcionário e dependente do funcionário, os dois são entidades, mas o funcionário é forte e o dependente é fraco.</p>
<p> • A Entidade Forte possui um atributo exclusivo que é chamado de <b>chave primária</b>. As Entidades Fracas não possuem chave primária
<p style="font-style: italic;"> Obs: A entidade <b>forte</b> é representada por um <b>retângulo</b>. A entidade <b>fraca</b> é representa por um <b>retângulo duplo</b>.</p>

<div align="center" style="text-align: center;">
    <img style= "border: 4px solid black;"src="https://user-images.githubusercontent.com/69658602/188220164-682376ab-f76d-4e03-9211-924aa6d7dbed.png">
</div>
<br>

<h2 align="center"> Entidades Fortes e Fracas do projeto: </h2>
<div style="text-align: center;">
    <img style= "border: 4px solid black; height: 300px;"src="https://user-images.githubusercontent.com/69658602/188223520-eda49fef-ace7-4172-8747-bdb23ab51850.png">
</div>
<hr>
<br>

<h1> Aula 04: Diagrama entidade relacionamento</h1>

<h2> <b> Tipos de relacionamento: </b> </h2>
<p> • Relacionamento Binário: Relacionamento entre <b> 2 </b> entidades.</p>
<p> • Relacionamento Ternário: Relacionamento entre <b> 3 </b> entidades.</p>
<p> • Relacionamento N-ário: Relacionamento entre <b> 4 </b> entidades.</p>

<h2> <b> Cardinalidade: Relação entre as entidades</b> </h2>
<h3> <b> Tipos de Cardinalidade </b> </h3>
<p> • <b> Cardinalidade 1:1.</b> Acontece quando cada ocorrência da entidade A se relaciona com somento uma ocorrência da entidade B. </p>
<p> • <b> Cardinalidade 1:N.</b> Quando cada ocorrência da entidade A se relaciona com mais de uma ocorrência da entidade B. </p>
<p> • <b> Cardinalidade N:M. </b> Quando mais de uma ocorrência da entidade A se relaciona com mais de uma ocorrência da entidade B.</p>

<h2 align="center"> Representando os relacionamentos no DER: </h2>
<div style="text-align: center;">
    <img style= "border: 4px solid black; height: 300px;"src="https://user-images.githubusercontent.com/69658602/188504806-05fdffc8-f276-467b-8550-8c38808ad9a8.png">
</div>

<h2> Entidade Associativa: </h2>
<p> • Todo relacionamento n:m pode ser entendido como uma entidade, essa entidade é denominada associativa, pois elas representam um fato, um relacionamento muitos-para-muitos. A entidade associativa faz a intermediação entre as entidades.</p>
<div style="text-align: center;">
    <img style= "border: 4px solid black; height: 300px;"src="https://user-images.githubusercontent.com/69658602/188505690-9e5db2bf-ab8b-46be-a39b-7c2951024d4c.png">
</div>
<hr>
<br>

<h1> <b> Aula 05: Atributos </b> </h1>

<h2> <b> O que são Atributos? </b> </h2>
<p> • Atributos são as características das Entidades.</p>
<p> • Não existe entidade sem um atributo.</p>

<h2> <b> Tipos de Atributo: </b> </h2>
<p> • Simples (atômico ou valor único, não pode ser dividido em partes menores para formar outros atributos). </p>
<p> • Composto (Pode ser dividido em partes menores para representar outros atributos. Endereço com cidade, rua, cep).</p>
<p> • Multivalorado (Mais de um valor).</p>
<p> • Armazenados (Um atributo que você pode armazenar, por exemplo uma data de nascimento).</p>
<p> • Derivados (Depende de outro atributo ou entidade para existir, como idade e data de nascimento).</p>
<p> • Null.</p>
<p> • Obrigatório (Not Null).</p>
<p> • Opcional (Null).</p>
<p> • Chave (Utilizado para identificar de forma única uma entidade. Exemplo: Código de um produto).</p>

<p style="font-style: italic;"> Obs: A chave que sai da entidade forte e chega na entidade fraca é denominada <b> chave estrangeira </b>.</p>

<h2> <b> Chave primária: </b> </h2>
<p> • Nunca se repete.</p>
<p> • Não pode ser nulo.</p>
<p> • Só entidades fortes possuem chave primária.</p>
<p> • Na representação pintamos de preto.</p>
<p> • Em entidades fracas temos a chave parcial, mas também temos que colocar a chave primária da entidade forte relacionada. Exemplo: Cod_cliente em "Pedido".</p>

<h2 align="center"> Modelagem final: </h2>
<div style="text-align: center;">
    <img style= "border: 4px solid black; height: 300px;"src="https://user-images.githubusercontent.com/69658602/188716106-228bbaed-5ee3-405a-b997-c2fbdb987779.png">
</div>

<hr>