2EX
#include <stdio.h>

int verificarAnoBissexto() {
    int ano;
    printf("Digite um ano: ");
    scanf("%d", &ano);

    if ((ano % 4 == 0 && ano % 100 != 0) || (ano % 400 == 0)) {
        return 1; // Retorna 1 se o ano for bissexto
    }
   

int main() {
    int resultado = verificarAnoBissexto();

    if (resultado == 1) {
        printf("O ano é bissexto.\n");
    } else {
        printf("O ano não é bissexto.\n");
    }

    return 0;
}
