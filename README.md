**Lídia De Mario (190008558)**



1) Escreva um programa na linguagem C que leia 3 notas de um aluno e calcule e exiba a média aritmética das 3 notas. Cada nota é um número real com uma casa decimal. A média deve ser exibida neste mesmo formato. OBS.: Não é necessário validar a entrada. 

```c
#include <stdio.h>
#include <stdlib.h>

int main() {
	
	
      float primeiranota, segundanota, terceiranota, media;
	
	printf ("Insira sua primeira nota = ");
	scanf ("%f",&primeiranota);

	printf ("\n\nInsira sua segunda nota = ");
	scanf ("%f",&segundanota);

	printf ("\n\nInsira sua terceira nota = ");
	scanf ("%f",&terceiranota);
	
	media = (primeiranota+segundanota+terceiranota)/3;
	
	printf ("\n\nA media final e = %0.1f", media);

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
	
	float area; 
	float pi = 3.14;
	float raio;
	
	printf ("Insira o valor do raio = ");	
	scanf ("%f",&raio);
	
	area = pi*pow(raio,2);
	
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
	
	int ra = 9;
	int numero;
	int resto;
	
	printf ("Insira um numero inteiro = ");	
	scanf ("%d", &numero);
	
	resto = numero % ra;
	
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
	
	int primeiramao;
	int segundamao;
	
		
	printf ("Insira a primeira mao (de 0 ate 4) = ");	
	scanf ("%d", &primeiramao);
	
	printf ("\n\nInsira a segunda mao (de 0 ate 4) = ");	
	scanf ("%d", &segundamao);
	
			
	if ((primeiramao == 0 && segundamao == 1)||(primeiramao == 0 && segundamao == 2)||(primeiramao == 1 && segundamao == 0)||(primeiramao == 2 && segundamao == 0))
	{
		printf ("\n\n0");
	}
	else if ((primeiramao == 1 && segundamao == 2)||(primeiramao == 1 && segundamao == 3)||(primeiramao == 2 && segundamao == 1)||(primeiramao == 3 && segundamao == 1))
	{
		printf ("\n\n1");
	}
		
	else if ((primeiramao == 2 && segundamao == 3)||(primeiramao == 2 && segundamao == 4)||(primeiramao == 3 && segundamao == 2)||(primeiramao == 4 && segundamao == 2))
	{
		printf ("\n\n2");
        }
	else if ((primeiramao == 3 && segundamao == 4)||(primeiramao == 3 && segundamao == 0)||(primeiramao == 4 && segundamao == 3)||(primeiramao == 0 && segundamao == 3))
	{
		printf ("\n\n3");
	}
	else if ((primeiramao == 4 && segundamao == 0)||(primeiramao == 4 && segundamao == 1)||(primeiramao == 0 && segundamao == 4)||(primeiramao == 1 && segundamao == 4))
	{
		printf ("\n\n4");
	}
	else if (primeiramao == segundamao)
	{
		printf ("\n\nempate");
	}
	else if (primeiramao > 4) 
	{
		printf ("\n\nprimeira mao invalida");
	}
	else if (segundamao > 4)
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

	int litros, recipiente50l, recipiente20l, recipiente10l, recipiente5l, recipiente2l;  
	
	printf( "Insira a quantidade de litros: " );	
	scanf( "%d", &litros );

	if (litros<5)
	{
		printf ("Pedido abaixo do limite minimo");
		
		return 1;
	}

	recipiente2l = 0;
	if ( litros%5 == 1 || litros %5 == 3 )
	{
		litros -= 4;
		recipiente2l = 2;
	}
	
	
	recipiente50l = litros / 50;  
	litros = litros % 50;  
	recipiente20l = litros / 20; 
	litros = litros % 20;
	recipiente10l = litros / 10; 
	litros = litros % 10;
	recipiente5l = litros / 5;  
	litros = litros % 5;  
	recipiente2l = recipiente2l + litros / 2;  
	
	printf( "50l = %d\n", recipiente50l );
	printf( "20l = %d\n", recipiente20l );
	printf( "10l = %d\n", recipiente10l );
	printf( "5l = %d\n", recipiente5l );
	printf( "2l = %d\n", recipiente2l );

	return 0;
}
```

7) Escreva um programa em linguagem C que verifique se o ano formado pelos quatro últimos algarismos de seu RA é ou não um ano bissexto, utilizando a definição dada. OBS.: Cada aluno deverá utilizar seu próprio RA. Este não deve ser solicitado pelo programa. 

```c
#include <stdio.h>  

int main()
{
	int ra = 8558;
	
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

![](https://i.imgur.com/be1EKx1.png)
A formula usada para construir a tabela-verdade é uma Contingencia

9) Escreva um programa em Português Estruturado que leia o ano de nascimento de uma pessoa e calcule e exiba a sua idade. 
![](https://i.imgur.com/GYp6I7E.png)

10) Escreva um programa em pseudocódigo e outro na linguagem C que peçam ao usuário para entrar com os três lados de um triângulo e escreva a área desse triângulo. O programa deverá também validar a entrada do usuário, ou seja, deverá verificar se os três valores de entrada satisfazem à condição de existência de um triângulo: “Cada lado do triângulo deve ser menor que a soma dos outros dois”.

Linguagem C:

```c
#include <stdio.h>
#include <stdlib.h>
#include <math.h>

int main() {
	
	float lado1, lado2, lado3, areatotal, semip;
	
	printf ("Digite o valor do primeiro lado = ");
	scanf ("%f",&lado1);

	printf ("\n\nDigite o valor do segundo lado = ");
	scanf ("%f",&lado2);

	printf ("\n\nDigite o valor do terceiro lado = ");
	scanf ("%f",&lado3);
	
	if ( lado1 < (lado2 + lado3) && lado2 < (lado1 + lado3) && lado3 < (lado1 + lado2) ) {
		
		semip = ( lado1 + lado2 + lado3 ) / 2;
		
		areatotal = sqrt ( semip * (semip - lado1) * (semip - lado2) * (semip - lado3) );
	
		printf("\n\nA area total do triangulo e = %0.2f", areatotal);
		
		return 0;
		
	}
	else {
		
		
		printf ("\n\nO triangulo e invalido.");
		
		return 1;
		
	}
	
}
```

Pseudocódigo:

![](https://i.imgur.com/gQ3KIxD.png)
