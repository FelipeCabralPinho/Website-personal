# Website-personal
Site pessoal que reúne minhas análises de jogos, visual novels e animes publicadas no Medium. A página funciona como um portfólio/vitrine: cada card mostra a capa, o título e um resumo do texto, e ao clicar na imagem o visitante é redirecionado para o artigo completo no Medium.

Textos disponíveis:
Rance Series — O Sublime Lado da Perversão	Série de jogos Rance, da Alice Soft
Uma Musume — Nascidas para Correr	Série e animação Uma Musume, da Cygames
Tsukihime — A Piece of Blue Glass Moon	Tsukihime Remake — Near Side of the Moon, de Kinoko Nasu
Kara no Kyoukai — Além das Fronteiras	Kara no Kyoukai, de Kinoko Nasu
Dies Irae — ‘Assim Falou Dies Irae’
Mordred Pendragon — Desilusão e Realização

Todos os textos estão no meu perfil: medium.com/@Feripe

Tecnologias:
- HTML5 para a estrutura da página
- CSS3 para o estilo e o layout
- Google Fonts (fonte Poppins)

Não há JavaScript, frameworks nem dependências para instalar: é um site estático.

Como foi construído:
Cada análise é um card (<div class="card">) com uma imagem, um título e uma descrição curta.
A imagem fica dentro de uma âncora (<a href' >), então clicar nela abre o artigo no Medium.
O layout em duas colunas é feito com float: os cards com a classe left vão para a esquerda e os com right para a direita, e o clear faz cada card descer na sua coluna.
O display: flow-root faz cada card conter a imagem flutuante, permitindo o espaçamento correto entre eles.
As imagens usam aspect-ratio e object-fit: cover para ficarem todas com o mesmo tamanho e proporção, sem distorcer.
O body usa flexbox em coluna para manter o rodapé sempre no fim da página.
Uma media query (max-width: 680px) deixa o site responsivo: no celular os cards ocupam a largura toda, com a imagem em cima e o texto embaixo.
