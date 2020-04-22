**Guilherme De Mario**

**RA 190008557**

1) Escreva um programa na linguagem C que leia 3 notas de um aluno e calcule e exiba a média aritmética das 3 notas. Cada nota é um número real com uma casa decimal. A média deve ser exibida neste mesmo formato. OBS.: Não é necessário validar a entrada. 

```c
#include <stdio.h>
#include <stdlib.h>

int main() {
	
	// ==================================
	// DECLARACOES DE VARIAVEIS
	// ==================================

	float nota1, nota2, nota3, media;
	
	// ==================================
	// ENTRADA
	// ==================================

	printf ("Insira a primeira nota = ");
	scanf ("%f",&nota1);

	printf ("\n\nInsira a segunda nota = ");
	scanf ("%f",&nota2);

	printf ("\n\nInsira a terceira nota = ");
	scanf ("%f",&nota3);
	
	// ==================================
	// PROCESSAMENTO
	// ==================================

	media = (nota1+nota2+nota3)/3;
	
	// ==================================
	// SAIDA
	// ==================================

	printf ("\n\nSua media final e = %0.1f", media);

	return 0;

}
```

2) Escreva um programa na linguagem C que leia o valor do raio r de um círculo e exiba a sua área. A área de um círculo de raio r é dada pela fórmula: Área = π . r2 
Nesta fórmula, considere o valor de π igual a 3,14.

```c
#include <stdio.h>
#include <stdlib.h>
#include <math.h>

int main() {
	
	// ==================================
	// DECLARACOES DE VARIAVEIS
	// ==================================
	
	float area; 
	float pi = 3.14;
	float raio;
	
	// ==================================
	// ENTRADA
	// ==================================
	
	printf ("Insira o valor do raio = ");	
	scanf ("%f",&raio);
	
	// ==================================
	// PROCESSAMENTO
	// ==================================
	
	area = pi*pow(raio,2);
	
	// ==================================
	// SAIDA
	// ==================================
	
	printf ("\n\nSua area e = %0.1f", area);
	
	return 0;
}
```

3) Escreva um programa que leia um número inteiro qualquer e verifique se é múltiplo do algarismo de maior valor do seu RA. Após a verificação, deve ser exibida mensagem informando se o número lido é ou não é múltiplo. 
Como exemplo do que é “o algarismo de maior valor do seu RA”, considere o RA 200001365. Ele é formado pelos algarismos 2, 0, 1, 3, 6 e 5. Entre esses algarismos, o de maior valor é o 6.
 
```c
#include <stdio.h>
#include <stdlib.h>
#include <math.h>

int main() {
	
	// ==================================
	// DECLARACOES DE VARIAVEIS
	// ==================================
  	 
	int ra = 9;
	int numero;
	int resto;
	
	// ==================================
	// ENTRADA
	// ==================================
	
	printf ("Insira um numero inteiro aqui = ");	
	scanf ("%d", &numero);
	
	// ==================================
	// PROCESSAMENTO
	// ==================================
	
	resto = numero % ra;
	
	// ==================================
	// SAIDA
	// ==================================
	
	if (resto == 0) {
		printf ("O numero %d e multiplo de %d", numero, ra);
		
	}
	else {
		printf ("O numero %d nao e multiplo de %d", numero, ra);
	}  
  	
	return 0;
}
```

4) Escreva um programa em linguagem C que receba dois números inteiros representando a duas “mãos” escolhidas por dois jogadores. O programa deverá imprimir o número representando a 2 “mão” do jogador ganhador. Caso os jogadores escolham a mesma “mão”, o programa deverá escrever “empate”.

```c
#include <stdio.h>
#include <stdlib.h>
#include <math.h>

int main() {
	
	// ==================================
	// DECLARACOES DE VARIAVEIS
	// ==================================
	
	int mao1;
	int mao2;
	
	// ==================================
	// ENTRADA
	// ==================================
	
	printf ("Insira a primeira mao aqui (de 0 ate 4) = ");	
	scanf ("%d", &mao1);
	
	printf ("\n\nInsira a segunda mao aqui (de 0 ate 4) = ");	
	scanf ("%d", &mao2);
	
	// ==================================
	// PROCESSAMENTO E SAIDA
	// ==================================	
		
	if ((mao1 == 0 && mao2 == 1)||(mao1 == 0 && mao2 == 2)||(mao1 == 1 && mao2 == 0)||(mao1 == 2 && mao2 == 0))
	{
		printf ("\n\n0");
	}
	else if ((mao1 == 1 && mao2 == 2)||(mao1 == 1 && mao2 == 3)||(mao1 == 2 && mao2 == 1)||(mao1 == 3 && mao2 == 1))
	{
		printf ("\n\n1");
	}
		
	else if ((mao1 == 2 && mao2 == 3)||(mao1 == 2 && mao2 == 4)||(mao1 == 3 && mao2 == 2)||(mao1 == 4 && mao2 == 2))
	{
		printf ("\n\n2");
        }
	else if ((mao1 == 3 && mao2 == 4)||(mao1 == 3 && mao2 == 0)||(mao1 == 4 && mao2 == 3)||(mao1 == 0 && mao2 == 3))
	{
		printf ("\n\n3");
	}
	else if ((mao1 == 4 && mao2 == 0)||(mao1 == 4 && mao2 == 1)||(mao1 == 0 && mao2 == 4)||(mao1 == 1 && mao2 == 4))
	{
		printf ("\n\n4");
	}
	else if (mao1 == mao2)
	{
		printf ("\n\nempate");
	}
	else if (mao1 > 4) 
	{
		printf ("\n\nprimeira mao invalida");
	}
	else if (mao2 > 4)
	{ 
		printf ("\n\nsegunda mao invalida");
	}	
		
	return 0;
	
}
```

5) Escreva um programa em linguagem C que peça ao usuário para entrar com uma quantidade do produto (em litros). O programa deverá determinar e imprimir a quantidade de recipientes de cada capacidade, necessária para envasar essa quantidade solicitada, de modo a minimizar a quantidade total de recipientes. Caso a quantidade solicitada seja inferior a 5 litros, o programa deverá informar “Pedido abaixo do limite mínimo”.

```c
#include <stdio.h>  

int main()
{
	
	// ==================================
	// DECLARACOES DE VARIAVEIS
	// ==================================
	
	int litros, recipiente50, recipiente20, recipiente10, recipiente5, recipiente2;  
	
	// ==================================
	// ENTRADA
	// ==================================


	printf( "Insira a quantidade de litros: " );	
	scanf( "%d", &litros );

	// ==================================
	// PROCESSAMENTO
	// ==================================
	
	if (litros<5)
	{
		printf ("Pedido abaixo do limite minimo");
		
		return 1;
	}

	recipiente2 = 0;
	if ( litros%5 == 1 || litros %5 == 3 )
	{
		litros -= 4;
		recipiente2 = 2;
	}
	
	
	recipiente50 = litros / 50;  
	litros = litros % 50;  
	recipiente20 = litros / 20; 
	litros = litros % 20;
	recipiente10 = litros / 10; 
	litros = litros % 10;
	recipiente5 = litros / 5;  
	litros = litros % 5;  
	recipiente2 = recipiente2 + litros / 2;  
	
	// ==================================
	// SAIDA
	// ==================================

	printf( "50l = %d\n", recipiente50 );
	printf( "20l = %d\n", recipiente20 );
	printf( "10l = %d\n", recipiente10 );
	printf( "5l = %d\n", recipiente5 );
	printf( "2l = %d\n", recipiente2 );

	return 0;
}
```

7) Escreva um programa em linguagem C que verifique se o ano formado pelos quatro últimos algarismos de seu RA é ou não um ano bissexto, utilizando a definição dada. OBS.: Cada aluno deverá utilizar seu próprio RA. Este não deve ser solicitado pelo programa. 

```c
#include <stdio.h>  

int main()
{
	// ==================================
	// DECLARACOES DE VARIAVEIS
	// ==================================
	
	int ra = 8557;
	
	// ==================================
	// PROCESSAMENTO E SAIDA
	// ==================================
	
	if (ra%400 == 0)
	{
		printf ("O ano %d e bissexto", ra);
		
	}
	else 
	{

		if (ra%4 == 0 && ra%100 != 100)
		{
			printf ("O ano %d e bissexto", ra);			
		} 	 
		else
		{
			printf ("O ano %d nao e bissexto", ra);
		}
	
	}
	
	return 0;
}
```

8) Tabela Verdade

![](https://i.imgur.com/iuzpvPO.png)

9) Escreva um programa em Português Estruturado que leia o ano de nascimento de uma pessoa e calcule e exiba a sua idade. 

```
inicio

    inteiro anoNascimento, idade

    escreva("Digite o ano em que nasceu:")
    leia(anoNascimento)

    idade <- (2020-anoNascimento)

    escreva("Voce tem ", idade, " anos")

fimalgoritmo
```

10) Escreva um programa em pseudocódigo e outro na linguagem C que peçam ao usuário para entrar com os três lados de um triângulo e escreva a área desse triângulo. O programa deverá também validar a entrada do usuário, ou seja, deverá verificar se os três valores de entrada satisfazem à condição de existência de um triângulo: “Cada lado do triângulo deve ser menor que a soma dos outros dois”.

Linguagem C:

```c
#include <stdio.h>
#include <stdlib.h>
#include <math.h>

int main() {
	
	// ==================================
	// DECLARACOES DE VARIAVEIS
	// ==================================
	
	float a, b, c, area, s;
	
	// ==================================
	// ENTRADA
	// ==================================

	printf ("Digite o primeiro lado = ");
	scanf ("%f",&a);

	printf ("\n\nDigite o segundo lado = ");
	scanf ("%f",&b);

	printf ("\n\nDigite o terceiro lado = ");
	scanf ("%f",&c);
	
	// ==================================
	// PROCESSAMENTO E SAIDA
	// ==================================
	
	if ( a < (b + c) && b < (a + c) && c < (a + b) ) {
		
		// calcular semiperimetro
		s = ( a + b + c ) / 2;
		
		// calcular area
		area = sqrt ( s * (s - a) * (s - b) * (s - c) );
		
		// saida
		printf("\n\nA area do triangulo e igual a = %0.2f", area);
		
		return 0;
		
	}
	else {
		
		// erro
		printf ("\n\nEsse triangulo e invalido.");
		
		return 1;
		
	}
	
}
```

Pseudocódigo:

![](https://i.imgur.com/rX0G5P3.png)
