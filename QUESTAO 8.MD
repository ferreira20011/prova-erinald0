EX 8
#include <stdio.h>


void calcula_imposto(float salario) {
    float imposto;

    if (salario > 5000.00) {
        imposto = salario * 0.20;
    } else {
        imposto = salario * 0.10;
    }

    printf("O valor do imposto a ser pago é: R$ %.2f\n", imposto);
}

int main() {
    float salario;

 
    printf("Digite o valor do salário: ");
    scanf("%f", &salario);

    calcula_imposto(salario);

    return 0;
}
