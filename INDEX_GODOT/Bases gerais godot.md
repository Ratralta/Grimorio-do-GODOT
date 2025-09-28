# Conceitos básicos da engine (Godot)
## Interface do Godot :
* A área de visualização do seu projeto se chama **Palco**. 
EX: 
![](hud_palco_exemplo.png)

* Os arquivos do seu projeto (como scripts, cenas e ETC), ficaram guardados no [FilseSystem](link_arquivos_salvos.md).
EX:
![](hud_arquivos_do_projeto_exemplo.png)

* Quando você clicar em um **node**, vai aparecer o [Inspetor de nodes](link_Nodes_Inspetor.md). 
EX: 
![](inspetor_node_sprite2D.png)

* Você consegue ver a documentação de um node apertando em **doc** no **inpetor** do node. 
EX: 
![](hud_abrir_documentacao_dos_nodes.png)
## Conceitos do godot : 
### Outras coisas 
Os projetos do godot podem ser divididos em três partes, **2D** ,**3D** e **SCRIPT**.

Todo o código fica dentro de "cenas", que tem que ser salvas nos arquivos.

Nodes "CSG" criam formas geométricas 3D
### Cenas, Nodes e scripts 

#### Cenas : 
* As coisas do seu projetos ficam guardados dentro de **Cenas**, elas são salvos como arquivos que ficam no [gerencador de arquivos](link_arquivos_salvos.md). Toda cena possui um [Node](link_Nodes_godot.md) raiz.

* E toda cena possui um **Node** raiz.
#### Nodes : 
* **Nodes** são todos os componentes que representa seu jogo, eles podem ser o sprite de alguma coisa ATÉ a caixa de colisão de um inimigo.
* Os nodes possuem :
	* Nome.
	* Propriedades do node (São ajustadas no [Inspetor](link_Nodes_Inspetor)).
	* Variáveis próprias.  
	* Podem conter funções.
	* Podem ser Nodes **filhos** ou Nodes **pais** de outros Nodes, podendo fazer uma **arvore de nodes** (Tree).
 As **propriedades** e as **funções** dos nodes são organizados dentro de **sessões**, que são esses bagulhos da imagem a baixo, existem **sessões globais**, e sessões especificas de um node :  
![](inspetor_node_Sessoes.png)
* Quando possui uma grande cadeia de nodes interligados uns aos outros, se chama de árvore de nodes (ou *tree*). 

* Nodes podem ser salvos como **recursos**. 

* Você pode abrir a documentação de um node, através desse botão aqui que fica no **Inspetor** : 
![](hud_abrir_documentacao_dos_nodes.png)

* Você pode adicionar **Scripts** nos nodes para eles passarem a ter códigos. Geralmente você vai ter que configurar os nodes no **Inspetor** para funcionarem do jeito que você quer, como por exemplo : 
-- Se você quiser colocar um sprite 2D, você precisa colocar o node [sprite 2D](node_Sprite2D), e também precisa definir a imagem que será usada como sprite no **[Inspetor](link_Nodes_Inspetor)**.
EX:
![](inspetor_node_sprite2D.png)

Um exemplo mais pratico, digamos que você quer criar um personagem, para isso, seria necessário um **node pai** para simbolizar o personagem ([CharacterBody2D](node_CharacterBody2D)), o node da **colisão** ([CollisionShape2D](node_CollisionShape2D)), para saber aonde ele interage com o mundo E o node do **sprite** ([Sprite2D](node_Sprite2D)), para ver ele andando pelo mundo.   
EX: 
![](nodes_exemplo_personagem.png)

#### Scripts : 
* **Scripts** é aonde você vai colocar os códigos do seu jogo, eles são salvos em arquivos, ficando no [FileSystem](link_arquivos_salvos.md)

# Dicas da engine (Godot)
* Se você estiver em um **palco 3D** , se você apertar Shift + F", faz com que a câmera entre no modo primeira pessoa.

* Você pode adicionar descrições ao node, através do inspetor. 
EX: 
![](inspetor_node_descrisoes.png)
# Coisas sobre a engine (Godot)
Todo "node", pode ser editado no "Inspetor", no canto superior direito 

