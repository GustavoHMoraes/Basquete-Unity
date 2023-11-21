# Basquete-Unity
Carlos Alarcon e Gustavo Henrique

# links
https://drive.google.com/file/d/1F0Sp0MQeXjokMQQk9S0L_7tMIDU3lqCQ/view?usp=sharing

# Colisores
1.Static Collider<br>
2.Rigidbody Collider<br>
3.Kinematic Rigidbody Collider<br>
4.Static Trigger Collider<br>
5.Rigidbody Trigger Collider<br>
6.Kinematic Rigidbody Trigger Collider<br>
# Cenas
<h2>Essas cenas foram criadas para demonstrar os tipos de colisores do unity de um jeito divertido, simulando uma partida de basquete</h2>
<img src ="img/cena1.png">
<img src ="img/cena2.png">
<h2>O jogo consiste em acertar a cesta 2 vezes, enquanto ela se move, tornando o jogo mais dificil.
<br>
A cena 1 foi inteiramente montada com objetos feitos no blender, para simular um ginasio de basquete, com arquibancadas, até banners de titúlos de campeonatos.
</h2>

# Hud e Menu
<img src ="img/menui.png"> <br>
<img src ="img/hud.png"><br>
<img src ="img/fim.png"><br>

Os menus e a hud foram feitos com o gameObject canvas, panel e buttons.
<img src ="img/cMenu.png"><br>

Este codigo define um menu com três métodos:

Jogar(): Carrega a cena "SampleScene" quando o botão "Jogar" é pressionado.
VoltarMenu(): Carrega a cena "menu" quando o botão "VoltarMenu" é pressionado.
Sair(): Encerra a aplicação quando o botão "Sair" é pressionado.

<img src ="img/cHud.png"><br>

Este codigo contabiliza quando a bola atinge a cesta e altera o número de cestas feitas

# Script

Codígo que faz a cesta se mover:<br>
<img src ="img/cesta.png"><br>
Ele utiliza uma variável de velocidade e uma posição limite em Z para mudar a direção do movimento quando o objeto ultrapassa esses limites. No método Update(), verifica-se a posição do objeto e atualiza o movimento com base na direção e na velocidade, permitindo que o objeto se mova para frente e para trás no eixo Z.
<br>
Codígo de movimentação utilizado na bola:<br>
<img src ="img/movimentacao.png"><br>
O código permite mover um objeto com base nas teclas  (W, S, D, A, Espaço) que estam associadas a uma direção de movimento (frente, trás, direita, esquerda, salto). A função Movimento é chamada para aplicar o movimento ao objeto usando transform.Translate. O código redefine o vetor de movimento para zero após cada movimento, o que pode afetar a continuidade de certos movimentos, como saltos, uma vez que as componentes do vetor são zeradas.
<br>
Codígo para alternar a fase depois de 2 cestas:<br>
<img src ="img/altcena.png"><br>
Este script controla uma contagem de colisões de um objeto com a tag "Player". Ele incrementa uma variável chamada bola cada vez que ocorre uma colisão. Quando essa variável atinge o valor de 2, o script carrega uma nova cena especificada pela variável Segfase usando SceneManager.LoadScene. Isso pode representar um sistema de contagem para passar para a próxima fase do jogo após duas colisões com este objeto.
<br>
Codígo para mostrar a mensagem:<br>
<img src ="img/msn.png">
<img src ="img/areatexto.png"><br>
Este script faz com que apareça uma mensagem enquanto você está em um trigger collider.

# Static Collider
É um colisor que irá ficar estatico, ele foi utilizado na quadra, arquibancadas e paredes do ginasio, além das paredes invisíves que limitam a área de movimento da bola(jogador).<br>
<img src ="img/static.png">

# Rigidbody Collider
É um colisor combinado com um Rigidbody, ele foi utilizado principalmente na bola, para dar fisica à ela.<br>
<img src ="img/bola.png">

# Kinematic Rigidbody Collider
É um colisor combinado com um rigidbody com a opção kinematic ativada para ser controlado por script, foi utilizado para a cesta.<br>
<img src ="img/cestaobj.png">

# Static Trigger Collider
É um colisor estatico com a opção de trigger ativado, ele foi utilizado na área onde aparece o texto.<br>
<img src ="img/statictrigger.png">

# Rigidbody Trigger Collider e Kinematic Rigidbody Trigger Collider
Esses são colisores combinados com rigidbody com a opção de trigger e kinematic, e eles foram utilizados no cubo que conta as cestas para passar de fase.<br>
<img src ="img/cube.png">
