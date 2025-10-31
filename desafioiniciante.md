#include <stdio.h>
int main(){

    char pais[10];
    char codigocarta [4];
    char nomecidade [10];
    int populacao;
    float area, PIB;
    int pontosturisticos;
    float densidadepopulacional, PIBPERCAPITA;


    char pais2[10];
    char codigocarta2 [4];
    char nomecidade2 [10];
    int populacao2;
    float area2, PIB2;
    int pontosturisticos2;
    float densidadepopulacional2, PIBPERCAPITA2;

    int atributo, atributo2;

printf("Vamos colocar os dados de sua primeira carta do super trunfo\n");
printf("Digite o nome do seu País: \n");
scanf("%s", pais);

printf("Digite o código da carta (Letra do País + Número de 01 a 04)\n");
scanf("%s", codigocarta);

printf("Digite o nome da cidade\n");
scanf("%s", nomecidade);

printf("Quantos habitantes tem na sua cidade?\n");
scanf("%d", &populacao);

printf("Qual a área da sua cidade?\n");
scanf("%f",&area);

printf("Qual o PIB da sua cidade?\n");
scanf("%f",&PIB);

printf("Quantos pontos turísticos existem na sua cidade?\n");
scanf("%d",&pontosturisticos);

densidadepopulacional = populacao / area;
PIBPERCAPITA = PIB / populacao;

printf("\n");
printf("\n");

printf("Vamos colocar os dados de sua segunda carta do super trunfo\n");
printf("Digite o nome do seu País: \n");
scanf("%s", pais2);

printf("Digite o código da carta (Letra do País + Número de 01 a 04)\n");
scanf("%s", codigocarta2);

printf("Digite o nome da cidade\n");
scanf("%s", nomecidade2);

printf("Quantos habitantes tem na sua cidade?\n");
scanf("%d", &populacao2);

printf("Qual a área da sua cidade?\n");
scanf("%f",&area2);

printf("Qual o PIB da sua cidade?\n");
scanf("%f",&PIB2);

printf("Quantos pontos turísticos existem na sua cidade?\n");
scanf("%d",&pontosturisticos2);

densidadepopulacional2 = populacao2 / area2;
PIBPERCAPITA2 = PIB2 / populacao2;

printf("\n");
printf("\n");
printf("\n");

printf("Carta 1\n");
printf("País: %s\n", pais);
printf("Código: %s\n", codigocarta);
printf("Nome da cidade: %s\n", nomecidade);
printf("Quantidade de habitantes: %d mil\n", populacao);
printf("Área: %f Km²\n", area);
printf("PIB: %f Bilhões de Reais\n", PIB);
printf("Pontos turísticos: %d\n", pontosturisticos);
printf("Densidade populacional = %f\n", densidadepopulacional);
printf("PIB per capita = %f\n", PIBPERCAPITA);

printf("\n");
printf("\n");
printf("\n");

printf("Carta 2\n");
printf("País: %s\n", pais2);
printf("Código: %s\n", codigocarta2);
printf("Nome da cidade: %s\n", nomecidade2);
printf("Quantidade de habitantes: %d mil\n", populacao2);
printf("Área: %f Km²\n", area2);
printf("PIB: %f Bilhões de Reais\n", PIB2);
printf("Pontos turísticos: %d\n", pontosturisticos2);
printf("Densidade populacional = %f\n", densidadepopulacional2);
printf("PIB per capita = %f\n", PIBPERCAPITA2);

printf("Comparação de cartas (Atributo: população!) \n");
if (populacao > populacao2){
    printf("Carta 1 venceu\n");
} else {
    printf("Carta 2 venceu\n");
}
}
