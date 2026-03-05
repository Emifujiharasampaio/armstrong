# armstrong
#include <stdio.h>

int main() {
    int num, original, dig, soma = 0;

    printf("Digite um numero: ");
    scanf("%d", &num);

    original = num;

    while(num > 0) {
        dig = num % 10;
        soma = soma + (dig*dig*dig);
        num = num / 10;
    }

    if(soma == original)
        printf("Numero de Armstrong\n");
    else
        printf("Nao e Armstrong\n");

    return 0;
}
