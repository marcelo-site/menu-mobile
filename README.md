# Menu mobile
 ## menu mobile wordpress só com Htmlç5 e CSS3

 Para começar oe entendimento de como foi construido e funciona esser código vamos para os links:

 1. Google fonts/icons para nossas imagens:
 https://fonts.google.com/icons/

 2. Para criar nosso botão de ofertas usei o plugin: Themify – WooCommerce Product Filter
 https://wordpress.org/plugins/themify-wc-product-filter/

 1. Agora para cursos indico os canais para começar cursoemvideo e cfbcursos para uma continuação com intuito de chegar à uma fase básica-intermédiaraia, segue os links: 
 https://www.youtube.com/c/CursoemV%C3%ADdeo
 https://www.youtube.com/c/cfbcursos

 sem falar nas indicaçoes da w3.org (orgão oficial para a HTML), w3schools e MDN da mozila que é tão popular que dispoensa apresentações:

 https://www.w3.org/
 https://www.w3schools.com/
 https://developer.mozilla.org/pt-BR/


 ### Começando de verdade

Para montar esse projeto na sua parte funcional eu usei os conceitos da HTML as tags: a, input e label e CSS foram: visibility e @media pelo menos as principais.
agora vamos entender o negocio  para cada redirecionamento para onde você quer seja na mesma pagina ou em outra página usamos a tag: a , ela se encontra onde você ver assim <"a class="ancor" href="#">. onde tem a # você coloca seu link, colocando o link no lugar da "#"(atenção não exclua as aspas) você deve colocar um texto depois desse sinal  e antes do próximo < , esse texto será aquele texto que aprece no link que serve para chamar o visitante para clicar nele (um exemplo se fosse um link para ser direcionado para os produtos em promoções estaria escrito mais ou menos assim: promocao ou ofertas).

Vamos ao começo do codigo HTML tem umas palavras dizendo: "escondido" e a segunda palavra "fantasma". a primeira representa uma seção que será escondida e só será apresentada quando toca  naquele "botão" escrito: "MENU" no canto inferior direito da tela, agora o que tem fantasma não será apresentado, pelo menos não essa seção que ele se encontra, mas será recuperada só a função e redirecionada lá pra aqule botão escrito: "OFERTAS" tai uma boa oportunidade para testar shortcodes e direcionar para essa caixinha criada com esse menu, se perceber nesse botõzinho "OFERTAS" existe um  "for="alguma coisa digitada" e lá no começo do código tem uma div com o id: fantasma (tá escrito assim: div=id"fantasma") tem um shortcode que se aplicado em um pagina, não ai, mas em um parte que ele for visivel e atualizando vai aperecer um input, clicando em cima dele para inspecionar vai ter acesso á uma caixa lateral no navegador e nela vai ter informações sobre ele o mais importante é o que tiver associado ao id, essa parte importante ela vai aparecer entre as aspas do elemnto id="aqui" , o que tiver ai dentro dessas aspas é o importante deve ser copiado e colocado no meio das aspas do for="aqui" do label for="" que aparece depois de  div e antes do texto OFERTAS fazendo isso quando clicar no botão ofertas é como se tivesse clicando naquele input gerado pelo shortcode, que nesse caso por estar dentro daquela div que será escondida, nem vamos ver para clicar. se conseguiu entender esse é fácil de entender o botão "MENU" a lógica é igual a difernça é que nesse caso usamos um id="" mas facil de achar nesse caso é o id="click" (olhe no começo do código HTML, nas primeiras linhas) esse botão escrito MENU ele apresenta e esconde essa div que tem o id="escondido" e tem outros elemnetos tipo svg ai é fácil de trabalhar para quem sabe trabalahar com fontes importadas  é só aplicar a mesma lógica. eu fiz diretamente no corpo da página baxei o arquivo no repositorio do google, um arquivo especial para navegador eu escolhi abrir no vscode copiei tudo que apareceu e colei dentro de uma div pronto, é o que precisa fazer se quiser mudar a imagem (veja só a imagem é tudo isso que aparece entre as tags svg e svg).

outra coisa que é bom comentar é sobre o @media lá do CSS ele configura comportamento de acordo o tamanho da tela os (min-widht:) e (max-widht:) o primeiro determina a largura minima e o segundo a largura máxima da tela que vocé escolheu para as acões que viram dentro dos {} logo após eo último @media tem um comando display:none isso é para esconder em dipositivos com largura igual ou maior a que tiver especificaficada em (min-width:) se já usa um plugin pra isso e puder usar aqui acho que é melhor, pq o plugin usa um tamanho para considerar celular, tablet e desktop e aqui vai ser usado outro então vai da escolha, escolhendo o plugin é só apagar essas linhas do ultimo @media