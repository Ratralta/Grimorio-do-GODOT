

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
> int amostrar_vida_bixo() {*codigo*} // o tipo de dado que ela pode retornar é **somente inteiro** 
> float teste_de_lista(list\<float> \_lista) {*codigo*} // tem parâmetro uma lista do tipo float, **retorna um float**

# Class e Objetos : 
## Class
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

Você também pode atribuir valores a um objeto quando for criar ele, caso já exista uma class pra ele se basear.
EX: 
```cs 
class Galinhas
{
    public string nome {get;set;}
    public int idade {get;set;}
    public bool compravel {get;set;}
}
class Program
{
    static void Main(string[] args)
    {
        Galinhas galinha_de_ouro = new Galinhas
        {
            nome = "Gustavo",
            idade = 9,
            compravel = true,
        };
        Console.WriteLine("Nome dessa galinha é " + galinha_de_ouro.nome);
    }
}
```

## Criando variáveis dentro de um class
Quando for criar um variável para um class, é recomendado fazer o uso de uma "feature" do c#, o {get;set;}
\--- **O que é {get;set?}**
get e set permitem adicionar algumas "propriedades" na hora de definir um valor para uma variável de um class/stuct. **Recomenda-se usar isso mesmo que você não queira  nenhuma propriedade especial para sua variável.**

EXEMPLO USANDO SEM DEFINIR NENHUMA PROPRIEDADE ESPECIAL: 
```c# 
class Pessoa
{
	string nome {get;set;} // mesma coisa que "string nome;"
	float tamanho {get;set;} // mesma coisa que "float tamanho;"
}



class Program 
{
    static void Main(string[] args) 
    {
	Console.WriteLine("Hello World!");
    }
}
```

\--- **Usando get/set com propriedades**





EXEMPLO USANDO DEFININDO UMA PROPRIEDADE ESPECIAL: 
```cs
class Galinhas
{
    public string nome { get; set;} // sem propriedade
    private int _idade; // valor "cobaia" que será usado na variavel "idade"
    public int idade
    {
        get { return _idade; } // mesma coisa que "int idade;"
        set // adicionando uma "propriedade" na hora de "setar" um valor a esta variavel, essa "propriedade" será lida quando a variavel receber um valor(value)
        {
            if (value < 0)
            {
               Console.WriteLine("Não existe idade menor que zero");
                _idade = 0;
            }
            else
            {
                Console.WriteLine("Idade ok");
                _idade = value;
            }
        }
    }
}
class Program
{
    static void Main(string[] args)
    {
        Galinhas galinha = new Galinhas();
        galinha.nome = "Felipe";
        galinha.idade = -30;
        Console.WriteLine("a idade dessa galinha é : " + galinha.idade);
        // vai aparecer no console :
        // > Não existe idade menor que zero
        // > a idade dessa galinha é : 0
    }
}
```
# Structs : 


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
    static void Main(string[] args) 
    {
	Console.WriteLine("Hello World!");
    }
}
```
## Sobre a visibilidade das variáveis 

## Memoria das Coisas
### Stack : 
É um local de memoria onde o computador oferece uma quantia limitada de memoria, as coisas guardadas nele são guardadas diretamente. 
As coisas são :
- int.
- bools.
- floats.
- chars.
- structs.

Quando você cria uma variável, ela é armazenada no stack.
### Heap :
É um local de memoria onde o computador oferece quanta memoria o "heap" precisar, ele guarda os dados dele como um "apartamento", cada andar tem sua "ID", aonde cada *coisa* é guardada.
As coisas são : 
* classes.
* arrays.
* lists.
* coleções.
* string? 

Quando você cria um objeto duma Class, as informações deste objeto vão para um "andar" no "heap" , enquanto o objeto em si se torna uma "ID" para acessar seu "andar".
- ID do objeto é guardado no "stack".
- Informações do objeto é guardado em um "andar" no "heap".

EX:
```c#
class Pessoa
{
    public string nome;
    public int idade;
}

class Program
{
    static void Main(string[] args)
    {
        Pessoa pes1 = new Pessoa();
        Pessoa pes2 = new Pessoa();
          
        pes1.nome = "Ronaldo Prompt";
        pes1.idade = 120;

        pes2.nome = "Cropto Silva";
        pes2.idade = 20;

        Console.WriteLine(pes1.nome);
    }
}
```
![](heap_explicacao_1.png)
SE VOCÊ FIZER :
> pes1 = pes2;
   pes1.idade += 1;
   Console.WriteLine(pes2.idade);

Na teoria era pra retornar 20 , mais na pratica retorna 21. POR QUE pes1 recebeu a "ID" de pes2, tendo acesso ao seu "andar" do "apartamento", então quando mexe no valor de pes1, mexe também no de pes2, alias ambos estão agora no mesmo "andar". 
EX:
![](heap_explicacao_2.png)








## Conceitos Básicos 
*  "Sou_arquivo.cs" , assim cria um arquivo C#.
*  Quando for criar uma variável, se você não definir sua visibilidade, ela naturalmente vai ser **private**
* Assim como as bibliotecas do pyton, o C# também possui, só que são tratados como "Classes".