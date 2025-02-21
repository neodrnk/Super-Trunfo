#include <stdio.h>
#include <locale.h>

int main() {
    setlocale(LC_ALL, "Portuguese");

    char estado1, estado2;
    char cidade1[100], cidade2[100], codigodacarta1[4], codigodacarta2[4];
    int npt1, npt2, vencedorPop;
    float area1, area2, pib1, pib2, densPop1, densPop2, pibPerCapita1, pibPerCapita2, inversoDensPop1, inversoDensPop2, SuperPoder1, SuperPoder2;
    unsigned int pop1, pop2;

    printf("Digite seu estado (letra de 'A' a 'H'): ");
    scanf(" %c", &estado1);

    printf("Digite o código da carta (ex: A01, B03): ");
    scanf("%3s", codigodacarta1);
    getchar();

    printf("Digite o nome da cidade: ");
    fgets(cidade1, sizeof(cidade1), stdin);

    printf("Digite a População da cidade: ");
    scanf("%u", &pop1);

    printf("Digite a Área (em km²) da cidade: ");
    scanf("%f", &area1);

    printf("Digite o PIB da cidade: ");
    scanf("%f", &pib1);

    printf("Digite o Número de Pontos Turísticos: ");
    scanf("%d", &npt1);
    getchar();

    printf("\nDigite seu estado (letra de 'A' a 'H'): ");
    scanf(" %c", &estado2);

    printf("Digite o código da carta (ex: A01, B03): ");
    scanf("%3s", codigodacarta2);
    getchar();

    printf("Digite o nome da cidade: ");
    fgets(cidade2, sizeof(cidade2), stdin);

    printf("Digite a População da cidade: ");
    scanf("%u", &pop2);

    printf("Digite a Área (em km²) da cidade: ");
    scanf("%f", &area2);

    printf("Digite o PIB da cidade: ");
    scanf("%f", &pib2);

    printf("Digite o Número de Pontos Turísticos: ");
    scanf("%d", &npt2);

    densPop1 = (float) pop1 / area1;
    densPop2 = (float) pop2 / area2;
    pibPerCapita1 = pib1 / (float) pop1;
    pibPerCapita2 = pib2 / (float) pop2;
    inversoDensPop1 = area1 / (float) pop1;
    inversoDensPop2 = area2 / (float) pop2;

    SuperPoder1 = (pop1 + area1 + pib1 + npt1 + pibPerCapita1 + inversoDensPop1);
    SuperPoder2 = (pop2 + area2 + pib2 + npt2 + pibPerCapita2 + inversoDensPop2);

    printf("\n===== Carta 1 =====\n");
    printf("Estado: %c\n", estado1);
    printf("Código: %s\n", codigodacarta1);
    printf("Nome da Cidade: %s", cidade1);
    printf("População: %u habitantes\n", pop1);
    printf("Área: %.2f km²", area1);
    printf("PIB: %.2f\n", pib1);
    printf("Número de Pontos Turísticos: %d\n", npt1);
    printf("Densidade Populacional: %.2f\n", densPop1);
    printf("PIB per capita: %.2f\n", pibPerCapita1);
    printf("Super Poder: %.2f\n", SuperPoder1);

    printf("\n===== Carta 2 =====\n");
    printf("Estado: %c\n", estado2);
    printf("Código: %s\n", codigodacarta2);
    printf("Nome da Cidade: %s", cidade2);
    printf("População: %u habitantes\n", pop2);
    printf("Área: %.2f km²\n", area2);
    printf("PIB: %.2f\n", pib2);
    printf("Número de Pontos Turísticos: %d\n", npt2);
    printf("Densidade Populacional: %.2f\n", densPop2);
    printf("PIB per capita: %.2f\n", pibPerCapita2);
    printf("Super Poder: %.2f\n", SuperPoder2);

    printf("\n===== Resultados das Comparações =====\n");

    vencedorPop = pop1 > pop2 ? 1 : 0;
    printf("População: Carta 1 (%u) vs Carta 2 (%u) -> Vencedor: %d\n", pop1, pop2, vencedorPop);
    printf("Área: Carta 1 (%.2f km²) vs Carta 2 (%.2f km²) -> Vencedor: %d\n", area1, area2, area1 > area2 ? 1 : 0);
    printf("PIB: Carta 1 (%.2f) vs Carta 2 (%.2f) -> Vencedor: %d\n", pib1, pib2, pib1 > pib2 ? 1 : 0);
    printf("Número de Pontos Turísticos: Carta 1 (%d) vs Carta 2 (%d) -> Vencedor: %d\n", npt1, npt2, npt1 > npt2 ? 1 : 0);
    printf("Super Poder: Carta 1 (%.2f) vs Carta 2 (%.2f) -> Vencedor: %d\n", SuperPoder1, SuperPoder2, SuperPoder1 > SuperPoder2 ? 1 : 0);

    return 0;
}
