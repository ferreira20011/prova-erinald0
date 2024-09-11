EX 9
#include <stdio.h>


void calcula_irrf(float salario_bruto) {
    float irrf = 0.0;

    if (salario_bruto <= 2112.00) {
        irrf = 0.0;
    } else if (salario_bruto <= 2826.65) {
        irrf = (salario_bruto * 0.075) - 158.40;
    } else if (salario_bruto <= 3751.05) {
        irrf = (salario_bruto * 0.15) - 370.40;
    } else if (salario_bruto <= 4664.68) {
        irrf = (salario_bruto * 0.225) - 651.73;
    } else {
        irrf = (salario_bruto * 0.275) - 884.96;
    }

    printf("O valor do IRRF a ser pago é: R$ %.2f\n", irrf);
}

int main() {
    float salario_bruto;

    
    printf("Digite o salário bruto: ");
    scanf("%f", &salario_bruto);

    calcula_irrf(salario_bruto);

    return 0;
}
