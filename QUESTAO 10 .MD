EX 10 
#include <stdio.h>


void calcula_inss(float salario_bruto) {
    float inss = 0.0;

    if (salario_bruto <= 1320.00) {
        inss = salario_bruto * 0.075;
    } else if (salario_bruto <= 2571.29) {
        inss = (1320.00 * 0.075) + ((salario_bruto - 1320.00) * 0.09);
    } else if (salario_bruto <= 3856.94) {
        inss = (1320.00 * 0.075) + ((2571.29 - 1320.00) * 0.09) + ((salario_bruto - 2571.29) * 0.12);
    } else if (salario_bruto <= 7507.49) {
        inss = (1320.00 * 0.075) + ((2571.29 - 1320.00) * 0.09) + ((3856.94 - 2571.29) * 0.12) + ((salario_bruto - 3856.94) * 0.14);
    } else {
        inss = (1320.00 * 0.075) + ((2571.29 - 1320.00) * 0.09) + ((3856.94 - 2571.29) * 0.12) + ((7507.49 - 3856.94) * 0.14);
    }

    printf("O valor da contribuição ao INSS é: R$ %.2f\n", inss);
}

int main() {
    float salario_bruto;

   
    printf("Digite o salário bruto: ");
    scanf("%f", &salario_bruto);

    calcula_inss(salario_bruto);

    return 0;
}
