#include <stdio.h>

int main() {
    int entrada, destino;
    double valor, convertido;
    char continuar;

    do {
        printf("\n=== Conversor de Medidas ===\n");
        printf("Escolha a unidade a ser convertida:\n");
        printf("1 - Centímetro (cm)\n");
        printf("2 - Metro (m)\n");
        printf("3 - Quilômetro (km)\n");
        printf("4 - Milha (mi)\n");
        printf("Sua escolha: ");
        scanf("%d", &entrada);

        printf("Digite o valor a ser convertido: ");
        scanf("%lf", &valor);

        printf("Converter para:\n");
        printf("1 - Metro\n");
        printf("2 - Quilômetro\n");
        printf("3 - Milha\n");
        printf("Sua escolha: ");
        scanf("%d", &destino);

        switch (entrada) {
            case 1: 
                switch (destino) {
                    case 1:
                        convertido = valor / 100.0;
                        printf("%.2f cm = %.4f m\n", valor, convertido);
                        break;
                    case 2:
                        convertido = valor / 100000.0;
                        printf("%.2f cm = %.6f km\n", valor, convertido);
                        break;
                    case 3:
                        convertido = valor / 160934.4;
                        printf("%.2f cm = %.6f mi\n", valor, convertido);
                        break;
                    default:
                        printf("Opção inválida.\n");
                }
                break;

            case 2: 
                switch (destino) {
                    case 1:
                        printf("%.2f m = %.2f m\n", valor, valor);
                        break;
                    case 2:
                        convertido = valor / 1000.0;
                        printf("%.2f m = %.4f km\n", valor, convertido);
                        break;
                    case 3:
                        convertido = valor / 1609.344;
                        printf("%.2f m = %.6f mi\n", valor, convertido);
                        break;
                    default:
                        printf("Opção inválida.\n");
                }
                break;

            case 3: 
                switch (destino) {
                    case 1:
                        convertido = valor * 1000;
                        printf("%.2f km = %.2f m\n", valor, convertido);
                        break;
                    case 2:
                        printf("%.2f km = %.2f km\n", valor, valor);
                        break;
                    case 3:
                        convertido = valor / 1.609344;
                        printf("%.2f km = %.6f mi\n", valor, convertido);
                        break;
                    default:
                        printf("Opção inválida.\n");
                }
                break;

            case 4: 
                switch (destino) {
                    case 1:
                        convertido = valor * 1609.344;
                        printf("%.2f mi = %.2f m\n", valor, convertido);
                        break;
                    case 2:
                        convertido = valor * 1.609344;
                        printf("%.2f mi = %.4f km\n", valor, convertido);
                        break;
                    case 3:
                        printf("%.2f mi = %.2f mi\n", valor, valor);
                        break;
                    default:
                        printf("Opção inválida.\n");
                }
                break;

            default:
                printf("Opção inválida.\n");
        }

        printf("\nDeseja converter outro valor? (s/n): ");
        getchar();
        scanf("%c", &continuar);

    } while (continuar == 's' || continuar == 'S');

    printf("Programa encerrado.\n");

    return 0;

}
