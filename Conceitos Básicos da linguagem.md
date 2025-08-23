

# Variáveis :
## Criando Variáveis :
Para criar uma variável, é preciso definir seu tipo, o nome, E não obrigatoriamente, um valor e sua visibilidade (Normalmente ela vai ser privada).
EX: 
> int hp_do_bixo = 12;
> float  speed_do_bixo = 3.6f;  ---- > *Talvez do "f" para definir que é um float*
> bool bixo_vivo = true;

## Criando Array : 
Coloque o tipo de dado da array antes de colocar seu nome.
EX:
> int[] array_de_pedras ;
> string[] nome_das_pedras = new string[] = {"João", "Gustavo Lima", "Rauã"};

"array_name.Lenght" , retorna tantos itens a **array** tem.
## Criando List : 
Parecido com criar Array, só com uma sintaxe diferente 
EX: 
> List\<float\> lista_de_numeros_vazia;
> List\<int\> lista_de_numeros_cheia = new List\<int\>() {5,13,89,55};

"lista_name.Count" , retorna tantos itens a **lista** tem 
# Lações de Repetições 
## Foreach :
É tipo o for, só que o valor do *i* assume o valor da posição que ele está na coleção. (é tipo o for do pyton)
EX: 
> foreach (int i in array_de_int) {*codigo*}
> bool (bool i in lista_de_true_ou_false) {*codigo*}

## For :
Possui uma condição para ser repetido, e seu *i* retorna só um numero.
EX: 
> for(int i=0 ; i<5 ; i++)
> for(int i=0 ; i< array_de_int.Lenght ; i++)

# Funções : 
Para criar funções, é preciso definir que tipo de dado ela vai retornar, caso queira criar parâmetros, é preciso definir o tipo de dados deles . (*Void* retorna nada)
EX: 
> void bixo_pule() {*codigo*} // não vai retornar nenhum valor
> int amostrar_vida_bixo() {*codigo*} // o tipo de dado que ela pode retornar é **somente** inteiro 
> float teste_de_lista(list\<float> \_lista) {*codigo*} // tem parâmetro uma lista do tipo float, retorna um float

# Class e Objetos: 
## Class
Para criar uma class, é só criar, nada demais. 
EX: 
>Class Pessoa
 {
	string Nome = "Cauã Rocha Falcão";
	int Idade = 176; 
	public void acao_falar_nome() // pode ser acessada por um objeto baseado nele  
	{
	Console.WriteLine($"Meu nome é {nome}");
	}
 }
 // Assim você criou um class.

Você pode alguns parâmetros na hora de criar um objeto usando uma classe, para isso, crie um public, com o nome da classe com parênteses, e dentro do parênteses, especifique os valores que você quer pedir. (Não esqueça de colocar o tipo de variável)
EX:
```cs
class Pessoa
{
	string Nome; // não possue valor 
	
	public Pessoa(string _nome) // constructor 
	{
	Nome = _nome;
	}
	
	public void acao_falar_nome()
	{
	Console.WriteLine($"Meu nome é {Nome}");
	}
}

class Program // COMEÇANDO O PROGRAMA
{
    static void Main() // COMEÇANDO O PROGRAMA
    {
        Pessoa pessoa_new = new Pessoa("Falcão Lima"); // OBJETO
        pessoa_new.acao_falar_nome();
    }
}
```


Algumas palavras chaves que você pode adicionar as suas classes para dar a elas algumas propriedades extras são:
	* **Static :**  Colocando isso na classe ou em suas variáveis, vai fazer com que você não precise criar um objeto para acessar seus métodos/atributos.    
## Objeto 
Para criar um objeto, você precisa de uma "class" para ele se basear, então colocando o nome do class, nome do objeto recebendo **new** class(), você cria um objeto.
EX:
>Class_name objeto_1 = new Class_name(); // criou um objeto
```
class Pessoa
{
	string Nome = "Cauã Rocha Falcão";
	int Idade = 176; 
	public void acao_falar_nome() // pode ser acessada por um objeto baseado nele  
	{
	Console.WriteLine($"Meu nome é {Nome}");
	}
}

class Program // COMEÇANDO O PROGRAMA
{
    static void Main() // COMEÇANDO O PROGRAMA
    {
        Pessoa pessoa_new = new Pessoa(); // OBJETO
        pessoa_new.acao_falar_nome();
    }
}
```
# Coisas : 
## Criando arquivo C++++
Para criar um arquivo c#, você precisa ter abaixado:
> .net framework.
> extensão "C#" do Visual Studio Code.
> extensão "C# Dev Kit" do Visual Studio Code.

Com eles abaixados , vá no Cropto de Comando, e use o comando ==dotnet new console -n NomeDoFolder==, assim vai criar uma pasta aonde você pode mexer com o C#.

## Template de código C++++
```
class Program 
{
    static void Main() 
    {
	Console.WriteLine("Hello World!");
    }
}
```
## Sobre a visibilidade das variáveis 

## Conceitos Básicos 
*  "Sou_arquivo.cs" , assim cria um arquivo C#.
*  Quando for criar uma variável, se você não definir sua visibilidade, ela naturalmente vai ser **private**
* Assim como as bibliotecas do pyton, o C# também possui, só que são tratados como "Classes".

