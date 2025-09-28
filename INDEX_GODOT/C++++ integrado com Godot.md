DOCUMENTAÇÃO DO GODOT + C# :
https://docs.godotengine.org/pt-br/4.x/tutorials/scripting/c_sharp/c_sharp_basics.html



Com "GD.funcao_qualquer", você consegue usar todas as funções do Godot, mesmo usando c#

# Conceitos Básicos :
## Partes Base de um script : 
Caso você crie um script anexado a um [Node](link_Nodes_godot.md), eles seguem o conceito de [classes derivadas](link_Class.md), aonde a classe derivada possui o **nome do arquivo**, enquanto a classe base é o [Tipo de node](link_Nodes_godot) que seu script está anexado.
EX: 
```godot_+_c#
using Godot;
using System;

public partial class primeiro_script : CharacterBody2D
{
// partial --> palavra chave de um class
// primeiro_script --> nome do arquivo 
// CharacterBody2D --> Tipo de node que esse script ESTÁ ligado

    public override void _Ready()
    {
    GD.Print("Hello World !!!")
    }
}
```

Similar ao "void static Main(){}", que faz seu código ser rodado normalmente, aqui existem 2 iniciadores do seu script, sendo eles : 
* **public override void \_Ready() {}** : Tudo que está dentro dele só vai ser lido quando a node especifico for adicionado na [Cena](link_Cenas_Godot).

* **public override void \_Process(double delta) {}** : Tudo que está dentro dele vai ser lido ACADA frame que passa do jogo. ("delta é os frames que estão passando)



## Erros comuns :
* **NÃO** é possível alterar o valor de uma propriedade de um [node](link_Nodes_godot) direto com c#, é preciso criar uma variável antes, e atribuir o valor da propriedade que você que mudar com o dessa variável criada. 
EX:
```godot_+_c#
var newPosition = Position; // pega valores de "Position"
newPosition.X = 100.0f; // muda valor do "newPosition"
Position = newPosition; // atribui "Position" para um novo valor "newPosition"
```
# Praticas de Jogo :
## Mexendo na posição do personagem : 
