EX 14
#include <stdio.h>


int main() {
    int turno;
 
    printf("Informe o turno do dia (1 para manhã, 2 para tarde, 3 para noite): ");
    scanf("%d", &turno);

   
    if (turno == 1) {
        printf("Bom dia!\n");
    } else if (turno == 2) {
        printf("Boa tarde!\n");
    } else if (turno == 3) {
        printf("Boa noite!\n");
    } else {
        printf("Erro: Turno inválido.\n");
    }

    return 0;
}

