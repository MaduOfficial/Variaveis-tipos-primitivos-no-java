# Variaveis-tipos-primitivos-no-java

Anotações de Variáveis - Tipos Primitivos

                                                                    Variáveis - Tipos Primitivos

.Tipos Inteiros

.Tipos Ponto Flutuante

.Tipo Char

.Tipo Boolean

.Literais

_

Tipos Primitivos

>boolean

>Números

.Inteiro                      .Ponto Flutuante

.byte                         .float
.short                        .double
.int
.long
.char

Os pontos flutuantes são os números que possuem vírgula, e os números inteiros são os números inteiros mesmo.

                                                                              Inteiros

Tipos inteiros

byte > São números bem pequinininhos
short > São um pouco maiores que o byte
int > São um pouco maiores que o short
long > é maior que o int

                                                           Tipos inteiros


                                    |   Tipo   |Tamanho(bits)|    Intervalo de valores      |            |
                                    |__________|_____________|______________________________|____________|
                                    |          |             |                              |   7     7  |
                                    |   byte   |     8       |         -128 a 127           |-(2 ) a 2 -1|
                                    |__________|_____________|______________________________|____________|
                                    |          |             |                              |   15    15 |
                                    |   short  |     16      |      -32.768 a 32.767        |-(2 ) a 2 -1|
                                    |__________|_____________|______________________________|____________|
                                    |          |             |                              |   31    31 |
                                    |    int   |     32      |-2.147.483.648 a 2.147.483.647|-(2 ) a 2 -1|
                                    |__________|_____________|______________________________|____________|
                                    |          |             |-9.223.372.036.854.775.808 a  |   63    63 |
                                    |   long   |     64      |-9.223.372.036.854.775.807    |-(2 ) a 2 -1|
                                    |__________|_____________|______________________________|____________|

                                                                 
                                                                     Ponto Flutuante

float > Quando acabamos de escrever o nosso comando no float usamos f
EX: float saldo1 = 100.30f;

double > O double é mais útilizado pois não precisa colocar nsda no final do comando.
EX: double saldo2 = 100.30;

NOTA:Usamos o float e o double para poder representar números com vírgula como uma nota na prova ou um preço de alguma comida ou coisa.


                                                        Ponto Flutuante

                                                 |   Tipo   |Tamanho(bits)|
                                                 |__________|_____________|
                                                 |          |             |
                                                 |  float   |     32      |
                                                 |__________|_____________|
                                                 |          |             |
                                                 |  double  |     64      |
                                                 |__________|_____________|

                                                             char


char o = 'o';

char i = 'i';

-------------
cada letra no ASCII tem um valor como o "o" e o "i".

char o = 111;

char i = 105;
System.out.println("" +o+i);

Se eu printar na tela ele vai fomar um oi, temos que útilizar áspas vazias para formar um "oi" por que se não ele vai somar o 111 com 105.

                                                             Boolean

true > verdadeiro
false > falso

boolean verdadeiro = true;

boolean falso = false;

                                                        Tipos inteiros
                                                          
package com.madu.VariaveisInteiras;

public class VariaveisInteirasTeste1 {

	public static void main(String[] args) {
		
		byte idade01 = 20;
		
		short idade02 = 21;
		
		int idade03 = 22;
		
		long idade04 = 23;
		
		System.out.println("Valor variável idade01 = " + idade01);
		System.out.println("Valor variável idade02 = " + idade02);
		System.out.println("Valor variável idade03 = " + idade03);
		System.out.println("Valor variável idade04 = " + idade04);
	}

}


                                                       Ponto Flutuante

package com.madu.VariaveisPontoFlutuante;

public class VariaveisPontoFlutuanteTeste1 {

	public static void main(String[] args) {
		
		double valorPasssagem = 2.90;
		
		float valorTomate = 3.95f;
		
		System.out.println("Valor da passagem = " + valorPasssagem);
		
		System.out.println("Valor do tomate = " + valorTomate);
	}

}


                                                          Variáveis char

Se não colocarmos áspas fica assim

package com.madu.variaveisChar;

public class VariaveisCharTeste1 {

	public static void main(String[] args) {
		
		char o = 'o';
		
		char i = 'i';
		
		System.out.println(o+i);

	}

}


Também podemos fazer assim


package com.madu.variaveisChar;

public class VariaveisCharTeste1 {

	public static void main(String[] args) {
		
		char o = 111;		
		char i = 105;
		
		System.out.println(""+o+i);

	}

}



No console irá somar os valores do o e do i

Console:216



package com.madu.variaveisChar;

public class VariaveisCharTeste1 {

	public static void main(String[] args) {
		
		char o = 'o';
		
		char i = 'i';
		
		System.out.println(""+o+i);

	}

}


Mas se colocarmos áspas duplas forma um oi no console.

Console:oi


package com.madu.variaveisChar;

public class VariaveisCharTeste1 {

	public static void main(String[] args) {
		
		//char o = 'o';
		//char i = 'i';
		
		char o = 111;	
		
		char i = 105;
		
		char interrogacão = 0X00E1; // valor '?'
		
		System.out.println(""+o+i+interrogacão);

	}

}


Console:oi?


                                                       VariaveisBoolean


package com.madu.VariaveisBoolean;

public class VariaveisBooleanTeste {

	public static void main(String[] args) {
		
		boolean verdadeiro = true;
		
		boolean falso = false;
		
		System.out.println("O valor de verdadeiro é " + verdadeiro);
		System.out.println("O valor de false é " + falso);
	}

}


Console: O valor de verdadeiro ? true
         O valor de false ? false


No dia a dia de um prigramador usamos bastante verdadeiro e falso, char, int e long, variáveis de ponto flutuante double e float.   

                                      
                                                            Curiosidade

Imagine uma entrvista de emprego no java, quando alguém for entrevistar um candidato.



package com.madu.curiosidadeInt.teste;

public class CuriosidadeIntTeste1 {

	public static void main(String[] args) {
		
		int var1 = 2147483647;
		
		int var2 = 100;
		
		System.out.println(var1 + var2);
	}

}



Pergunta:O que você acha que aconteceria se eu somar duas variáveis, sendo que a primeira variável está no valor maximo?

Essa é um tipo de pergunta pegadinha numa entrevista de emprego java.

Console:-2147483549

Alguns candidatos tendem a dizer que vai dar erro, mas vimos que não deu erro, o que aconteceu é que o código é como uma roleta se somarmos um em ves de 100
vai dar -2.147.483.648


package com.madu.curiosidadeInt.teste;

public class CuriosidadeIntTeste1 {

	public static void main(String[] args) {
		
		int var1 = 2147483647;
		
		int var2 = 1;
		
		System.out.println(var1 + var2);
	    
	}

}


Console:-2147483648


Resaposta: Os numeros no java funcionam que nem uma roleta, no momento em que eu pego o limite e somo alguma coisa ele vai voltar para os números negativos.
isso é para byte, short, int e long e para qualquer tipo inteiro no java.


                                                                 Literais

O que acontece que java tem uma outra coisa chamada de literais

int idade1 = 20;

long idade2 = 20l;

A gente viu ali que no exemplo de inteiro que eu podia declarar qualquer coisa, mas se você quiser deixar explícito o valor que você tá colocando ali é um
long você usa um l no final, da mesma forma que você utiliza o f para o float, por que toda vez que a gente declara um inteiro no java por padrão o
inteiro que eu falo de byte, short, int e long por padrão ele é um int, então padrão aí literais no java int.


double d1 = 123.4;

//mesmo valor que d1, mas em notação científica
double d2 = 1.234e2;

float f1 = 123.4f


a mesma coisa é com o dooble por padrão a gente sempre declara um double mas se você quiser especificar você tem que botar ali o f no final do floa,
outra curiosidade o double e o float eles aceitam a votação científica.


                                                                Literais
                                                      Hexadecimais, Octais, Binários

int decVal = 26;

int hexVal = 0xla;

int octVal = 032;

int binVal = 0b11010; // JDK 7

Um valor decimal é um valor em que a gente tá acostumado valor 26, o valor Hexadecimal a gente precisa botar um 0 e um x 0 x para indicar que é um
decimal e aí a gente coloca o 1a, que seria o valor do 26 em um Hexadecimal, e o Octal a gente começa com 0, então se a gente começar um inteiro
com 0 ele vai ter um valor octal no caso 32 é igual 26 que é igual a 1a de um dexadecimal, e o Binário também, o Binário você começa com 0b aí
o b também é minúsculo de acordo com o gosto do freguês, só o Binário é apenas a partir do java 7 tá.


                                                                Literais
                                                            Pode e não pode


long creditCardNumber = 1234_5678_9012_3456L;
long cpf = 101_134_156_68L;
float pi = 3.14_15F;
long hexBytes = oxFF_EC_DE_5E;
long hexWOrds = 0xCAFE_BABE;
long maxLong = ox7fff_ffff_ffff_ffffL;
byte nybbles = 0b0010_0101;
long bytes = 0b11010010_01101001_10010100_10010010;

No java se você quizer para ajudar na leitura do programa você também pode separar os seus números com underscore é o trasinho em baixo, então por
por exemplo no  número do cartão de crédito pra ficar mais legível você utiliza o underscore para separar no cpf também útiliza um underscore
o pi por exemplo que é aquele número no brandão 33. blá blá blá,se você quiser separar também pode a mesma coisa com os numeros hexadecimais ali no
no caso do hexBytes e hexWorlds é a mesma coisa para o 0x7fff, ou a mesma coisa também para binários, então é só um exemplo que você podeutilizar
underscore, isso é do java 7.

O que eu não posso fazer com o underscore

//Não pode colocar underscore perto de ponto
float pi1 = 3_.1415F;
//Não pode colocar underscore perto de ponto
float pi2 = 3._1415F;
//Não pode colocar underscore perto de sufixos (L)
long cpf = 101_134_156_68_L;

//identificador, não é literal
int x1 = _52;
//OK (decimal literal)
int x2 = 5_2;
//Não pode colocar underscore no final de um literal
int x3 = 52_;
// OK (decimal literal)
int x4 = 5_______2;

//Não pode colocar underscore perto de prefixos (0x)
int x5 = 0_x52;
//Não pode colocar underscore no começo de números
int x6 = 0x_52;
//OK (hexadecagono literal)
int x7 = 0x5_2;
//Não pode colocar underscore no final de números
int x8 = 0x52_;


                                                                                     Piadinha

Essa é só uma piadinha, é um assunto para a próxima aula.


package com.madu.Piadinha;

public class PiadinhaTeste {
	
	int Oct31 = 031;
	
	int Dec25 = 25;
	
	System.out.println(Oct31 == Dec25);
}

Console:true

Eles tem o mesmo valor

                                                                                  Escape - char


                                                |   Sequência de escape  |        Descrição         |
                                                |________________________|__________________________|
                                                |                        |                          |
                                                |           \t           |           tab            |
                                                |________________________|__________________________|
                                                |                        |                          |
                                                |           \b           |         backspace        |
                                                |________________________|__________________________|
                                                |                        |                          |
                                                |           \n           |         nova linha       |
                                                |________________________|__________________________|
                                                |                        |                          |
                                                |           \r           |     retorno de carro     |
                                                |________________________|__________________________|
                                                |                        |                          |
                                                |           \f           |    avanço de página      |
                                                |________________________|__________________________|
                                                |                        |                          |
                                                |           \'           |       aspas simples      |
                                                |________________________|__________________________|
                                                |                        |                          |
                                                |           \"           |       aspas duplas       |
                                                |________________________|__________________________|
                                                |                        |                          |
                                                |           \\           |      barra invertida     |
                                                |________________________|__________________________|
                                                |                        |                          |
                                                |           \ddd         |      constante octal     |
                                                |________________________|__________________________|
                                                |                        |                          |
                                                |           \uxxxx       |   constante hexadecimal  |
                                                |________________________|__________________________|


Essas sequências são muito úteis na hora de formatar o output do nosso programa, os programadores usam mais o tab, o \n, o \r, aspas simples, aspas duplas
e barra invertida que é o que a gente útiliza no nosso dia a dia, a constante hexadecimal é mais para trabalhar com qr code.

Curiosidade1:

package com.madu.SequenciaEscape;

public class SequenciaEscapeTeste {

	public static void main(String[] args) {
		
		//"Hello, World!"
		System.out.print("\"Hello, World!\"");
	}

}

Console:Hello, World!



package com.madu.SequenciaEscape;

public class SequenciaEscapeTeste {

	public static void main(String[] args) {
		
		//"Hello, World!"
		System.out.print("\"Hello, World!\"\n\r");
	}

}


Se adicionarmos esses dois código System.out.print("\"Hello, World!\"\n\r"); / System.out.print("\"Hello, World!\"");    a gente pode clicar na linha de baixo.


Curiosidade2:Eu que ro incurtar o 1\4




package com.madu.SequenciaEscape;

public class SequenciaEscapeTeste {

	public static void main(String[] args) {
		
		//"Hello, World!"
		System.out.print("\"Hello, World!\"\n\r");
		// 1\4
		System.out.print("1\4");
	}

}

Console:Hello, World!

        1


vimos que só fez output do 1 para fazermos output do 1\4 precisamos adicionar duas \\


package com.madu.SequenciaEscape;

public class SequenciaEscapeTeste {

	public static void main(String[] args) {
		
		//"Hello, World!"
		System.out.print("\"Hello, World!\"\n\r");
		// 1\4
		System.out.print("1\\4");
	}

}


Console:"Hello, World!"

         1\4
