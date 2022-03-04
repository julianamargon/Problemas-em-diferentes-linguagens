# Problemas-em-diferentes-linguagens
Soma de impares 
#include <stdio.h> (Partes obrigatórias do código)
int main()
{
    int x, y, soma, troca; (DECLARAÇÃO DAS VARIÁVEIS)    
    printf("Digite dois numeros: \n"); (SAÍDA)
    scanf("%d", &x); (ENTRADA)
    scanf("%d", &y); (ENTRADA)
	Forma alternativa scanf(“%d %d”, &x &y)
    	 
    if (x > y){    (Se x for maior que y, troque-os de lugar; a conta deve ser sempre crescente)
        	troca = x;
       	 x = y;
        	y = troca;
    	}
   soma = 0; (Sempre que usar a função soma, declare a soma=0)
    for(int i = x + 1; i < y; i++){ (declaração da variável i feita aqui int =i, pode fazer isso na fç FOR) 
        if(i % 2 != 0){
            soma = soma + i;
        }
    }
A função diz: para variável i = x+1 (não conta o X); e variável i menor que y (ou seja não conta o y); vá contando de 1 em 1 e some tods os valores nesse intervalo que quando i for dividido por 2 tenha resto diferente de zero, ou seja, seja um número ímpar)
        printf("SOMA DOS ÍMPARES = %d\n", soma);    
Escreva esses valores em tela com o valor que ficou gravado na variável soma, sob os comandos da função acima
    return 0;
}
