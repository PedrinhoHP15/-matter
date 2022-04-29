# -matter

#include <stdio.h>

void Decimal_para_bin(int numero_decimal){
	int i, j;
	int bin[100] = {0};

	for(i = 0; numero_decimal != 0; i++){
	    bin[i] = numero_decimal % 2;
		numero_decimal = numero_decimal / 2;
	}
	for(j = i; j >= 0; j--){
		printf("%d", bin[j]);
	}
}
 
int main(){
	int numero;
    printf("Digite um numero: ");
	scanf("%d", &numero);
	 	
	Decimal_para_bin(numero);
 	
	return 0;
 }
