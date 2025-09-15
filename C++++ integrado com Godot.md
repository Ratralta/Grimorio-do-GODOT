DOCUMENTAÇÃO DO GODOT + C# :
https://docs.godotengine.org/pt-br/4.x/tutorials/scripting/c_sharp/c_sharp_basics.html



Com "GD.funcao_qualquer", você consegue usar todas as funções do Godot, mesmo usando c#

# Conceitos Básicos
## Partes Base de um script 
Quando você cria um script relacionado a um [Node](link_Nodes_godot.md), eles seguem o conceito de [classes derivadas](link_Class.md), onde o script que você ligou ao Node É uma classe derivada da classe Node. (**Nodes** são vistos como classes no c#.)

Similar ao "void static Main(){}", que faz seu código ser rodado normalmente, aqui existem 2 iniciadores do seu script, sendo eles : 
* **public override void \_Ready() {}** : Tudo que está dentro dele só vai ser lido quando a node especifico for adicionado na [Cena](link_Cenas_Godot).

* **public override void \_Process(double delta) {}** : Tudo que está dentro dele vai ser lido ACADA frame que passa do jogo. ("delta é os frames que estão passando)