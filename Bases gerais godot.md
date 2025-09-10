# Conceitos básicos da engine (Godot)
## Interface do Godot :
* A área de visualização do seu projeto se chama **Palco**. 
EX: 
![](palco_exemplo.png)

* Os arquivos do seu projeto (como scripts, cenas e ETC), ficaram guardados no [FilseSystem](link_arquivos_salvos.md).
EX:
![](arquivos_do_projeto_exemplo.png)
## Conceitos do godot : 
### Outras coisas 
Os projetos do godot podem ser divididos em três partes, **2D** ,**3D** e **SCRIPT**.

Todo o código fica dentro de "cenas", que tem que ser salvas nos arquivos.

Nodes "CSG" criam formas geométricas 3D
### Cenas, Nodes e scripts 

#### Cenas : 
* As coisas do seu projetos ficam guardados dentro de **Cenas**, E toda cena possui um **Node** raiz.
#### Nodes : 

**Nodes** são todos os componentes que representa seu jogo, eles podem ser o sprite de alguma coisa ATÉ a caixa de colisão de um inimigo, você pode adicionar **Scripts** nos nodes para eles passarem a ter códigos.
Geralmente você vai ter que configurar os nodes no **Inspetor** para funcionarem do jeito que você quer, como por exemplo : 
-- Se você quiser colocar um sprite 2D, você precisa colocar o node [sprite 2D](node_Sprite2D), e também precisa definir a imagem que será usada como sprite no **Inspetor**.
EX:
![](inspetor_node_sprite2D.png)

Um exemplo mais pratico, digamos que você quer criar um personagem, para isso, seria necessário um **node pai** para simbolizar o personagem ([CharacterBody2D](node_CharacterBody2D)), o node da **colisão** ([CollisionShape2D](node_CollisionShape2D)), para saber aonde ele interage com o mundo E o node do **sprite** ([Sprite2D](node_Sprite2D)), para ver ele andando pelo mundo.   
EX: 
![](nodes_exemplo_personagem.png)

#### Scripts : 
* **Scripts** é aonde você vai colocar os códigos do seu jogo, eles são salvos em arquivos, ficando no [FileSystem](link_arquivos_salvos.md)

# Dicas da engine (Godot)
"Shift + F", faz com que a câmera entre no modo primeira pessoa 

# Coisas sobre a engine (Godot)
Todo "node", pode ser editado no "Inspetor", no canto superior direito 