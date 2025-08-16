

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

## Criando List : 
Parecido com criar Array, só com uma sintaxe diferente 
EX: 
> List\<float\> lista_de_numeros_vazia;
> List\<int\> lista_de_numeros_cheia = new List\<int\>() {5,13,89,55};


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
Para criar funções, é preciso definir que tipo de dado ela vai retornar. (*Void* retorna nada)
EX: 
> void bixo_pule() {*codigo*} // não vai retornar nenhum valor
> int amostrar_vida_bixo() {*codigo*} // o tipo de dado que ela pode retornar é **somente** inteiro 


# Coisas : 
*  "Sou_arquivo.cs" , assim cria um arquivo C#.
*  Quando for criar uma variável, se você não definir sua visibilidade, ela naturalmente vai ser **private**
* 
