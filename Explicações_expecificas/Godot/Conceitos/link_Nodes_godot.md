# Conceito de Nodes :
* **Nodes** são todos os componentes que representa seu jogo, eles podem ser o sprite de alguma coisa ATÉ a caixa de colisão de um inimigo. 

* Os nodes possuem :
	* Nome.
	* Propriedades (São ajustadas no [Inspetor](link_Nodes_Inspetor)).
	* Podem conter funções.
	* Podem ser Nodes filhos ou Nodes pais de outros Nodes.

* Quando possui uma grande cadeia de nodes interligados uns aos outros, se chama de árvore de nodes (ou *tree*). 

* Você pode adicionar **Scripts** nos nodes para eles passarem a ter códigos. Geralmente você vai ter que configurar os nodes no **Inspetor** para funcionarem do jeito que você quer, como por exemplo : 
-- Se você quiser colocar um sprite 2D, você precisa colocar o node [sprite 2D](node_Sprite2D), e também precisa definir a imagem que será usada como sprite no **[Inspetor](link_Nodes_Inspetor)**.
EX:
![](inspetor_node_sprite2D.png)

Um exemplo mais pratico, digamos que você quer criar um personagem, para isso, seria necessário um **node pai** para simbolizar o personagem ([CharacterBody2D](node_CharacterBody2D)), o node da **colisão** ([CollisionShape2D](node_CollisionShape2D)), para saber aonde ele interage com o mundo E o node do **sprite** ([Sprite2D](node_Sprite2D)), para ver ele andando pelo mundo.   
EX: 
![](nodes_exemplo_personagem.png)

# Nodes Pais Supremos : 
## Nodes Control
==CONCEITO==: Tem como foco, coisas relacionadas a HUD do player

==EXEMPLOS DE NODES CONTROL==: 
------ [Label](node_Label) : É uma área de texto que aparece na tela

## Nodes Spatial
==CONCEITO==: Tem como foco, nodes relacionados a espaço 3D, como criar cubos 

==EXEMPLOS DE NODES SPATIAL==: 
------ Lorem ipsolon Dolor

## Nodes 2D
==CONCEITO==: Lorem ipsolon Dolor

==EXEMPLOS DE NODES 2D==:  
------ Lorem Ipsolon Dolor 

# Tipos de Nodes : 
## Nodes Body : 
==CONCEITO== : É 

==DEPENDENCIAS==: Todos os nodes body PRECISAM de um node de colisão.

==EXEMPLOS DE NODES BODY==: 
------ [CharacterBody2D](node_CharacterBody2D) 

------ [StaticBody2D](node_StaticBody2D) 