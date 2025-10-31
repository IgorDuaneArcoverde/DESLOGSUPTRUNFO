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

//aqui é a parte do desafio iniciante
printf("Comparação de cartas (Atributo: população!) \n");
if (populacao > populacao2){
    printf("Carta 1 venceu\n");
} else {
    printf("Carta 2 venceu\n");
}
//aqui a parte do desafio intermediario
printf("### Escolha o atributo de comparação entre as duas cartas ###\n");
printf("1 - Nome do país.\n");
printf("2 - População.\n");
printf("3 - Área.\n");
printf("4 - PIB.\n");
printf("5 - Número de pontos turísticos.\n");
printf("6 - Densidade demográfica.\n");
scanf("%d", &atributo);

printf("### RESULTADO ###\n");

switch (atributo){
case 1:
    printf("Atributo 1: Nome do País\n");
    printf("%s e %s\n", pais, pais2 );
    printf("Não há vencedores\n");
    break;
case 2:
printf("Atributo 2: Número de habitantes: \n");
printf("%d vs %d \n", populacao, populacao2);
if (populacao == populacao2){
    printf("Empate!");
}   else if(populacao > populacao2){
        printf("Carta 1 venceu!\n");
        } else {
        printf("Carta 2 venceu!\n");
        }
    break;
case 3:
printf("Atributo 3: Área: \n");
printf("%f vs %f \n", area, area2);
if (area == area2){
    printf("Empate!");
}   else if(area > area2){
        printf("Carta 1 venceu!\n");
        } else {
        printf("Carta 2 venceu!\n");
        }
    break;
case 4:
printf("Atributo 4: PIB: \n");
printf("%f vs %f \n", PIB, PIB2);
if (PIB == PIB2){
    printf("Empate!");
}   else if(PIB > PIB2){
        printf("Carta 1 venceu!\n");
        } else {
        printf("Carta 2 venceu!\n");
        }
    break;
case 5:
printf("Atributo 5: número de pontos turísticos: \n");
printf("%d vs %d \n", pontosturisticos, pontosturisticos2);
if (pontosturisticos == pontosturisticos2){
    printf("Empate!");
}   else if(pontosturisticos > pontosturisticos2){
        printf("Carta 1 venceu!\n");
        } else {
        printf("Carta 2 venceu!\n");
        }
    break;
case 6:
printf("Atributo 6: Densidade demográifca: \n");
printf("%f vs %f \n", densidadepopulacional, densidadepopulacional2);
if (densidadepopulacional2 == densidadepopulacional){
    printf("Empate!");
}   else if(densidadepopulacional < densidadepopulacional2){
        printf("Carta 1 venceu!\n");
        } else {
        printf("Carta 2 venceu!\n");
        }
    break;
default:
    printf("opção inválida!\n");
    break;
}
//Aqui a parte do nivel mestre
printf("\n");
printf("\n");
printf("\n");

printf("### Escolha o primeiro atributo de comparação entre as duas cartas ###\n");
printf("1 - Nome do país.\n");
printf("2 - População.\n");
printf("3 - Área.\n");
printf("4 - PIB.\n");
printf("5 - Número de pontos turísticos.\n");
printf("6 - Densidade demográfica.\n");
scanf("%d", &atributo);

printf("### Escolha o segundo atributo de comparação entre as duas cartas ###\n");
printf("1 - Nome do país.\n");
printf("2 - População.\n");
printf("3 - Área.\n");
printf("4 - PIB.\n");
printf("5 - Número de pontos turísticos.\n");
printf("6 - Densidade demográfica.\n");
scanf("%d", &atributo2);

printf("### RESULTADO ###\n");

if(atributo == atributo2){
    printf("A escolha de atributos deve ser diferente!\n");
}   else {
        switch (atributo){
        case 1:
                printf("Atributo 1: Nome do País\n");
                printf("%s e %s\n", pais, pais2 );
                printf("Não há vencedores\n");
        break;
        case 2:
        printf("Atributo 2: Número de habitantes: \n");
        printf("%d vs %d \n", populacao, populacao2);
        if (populacao == populacao2){
            printf("Empate!");
        }   else if(populacao > populacao2){
                printf("Carta 1 venceu!\n");
                } else {
                printf("Carta 2 venceu!\n");
                }
            break;
        case 3:
        printf("Atributo 3: Área: \n");
        printf("%f vs %f \n", area, area2);
        if (area == area2){
            printf("Empate!");
        }   else if(area > area2){
                printf("Carta 1 venceu!\n");
                } else {
                printf("Carta 2 venceu!\n");
                }
            break;
        case 4:
        printf("Atributo 4: PIB: \n");
        printf("%f vs %f \n", PIB, PIB2);
        if (PIB == PIB2){
            printf("Empate!");
        }   else if(PIB > PIB2){
                printf("Carta 1 venceu!\n");
                } else {
                printf("Carta 2 venceu!\n");
                }
            break;
        case 5:
        printf("Atributo 5: número de pontos turísticos: \n");
        printf("%d vs %d \n", pontosturisticos, pontosturisticos2);
        if (pontosturisticos == pontosturisticos2){
            printf("Empate!");
        }   else if(pontosturisticos > pontosturisticos2){
                printf("Carta 1 venceu!\n");
                } else {
                printf("Carta 2 venceu!\n");
                }
            break;
        case 6:
        printf("Atributo 6: Densidade demográifca: \n");
        printf("%f vs %f \n", densidadepopulacional, densidadepopulacional2);
        if (densidadepopulacional2 == densidadepopulacional){
            printf("Empate!");
        }   else if(densidadepopulacional < densidadepopulacional2){
                printf("Carta 1 venceu!\n");
                } else {
                printf("Carta 2 venceu!\n");
                }
            break;
        default:
            printf("opção inválida!\n");
            break;
        }
        switch (atributo2){
        case 1:
                printf("Atributo 1: Nome do País\n");
                printf("%s e %s\n", pais, pais2 );
                printf("Não há vencedores\n");
        break;
        case 2:
        printf("Atributo 2: Número de habitantes: \n");
        printf("%d vs %d \n", populacao, populacao2);
        if (populacao == populacao2){
            printf("Empate!");
        }   else if(populacao > populacao2){
                printf("Carta 1 venceu!\n");
                } else {
                printf("Carta 2 venceu!\n");
                }
            break;
        case 3:
        printf("Atributo 3: Área: \n");
        printf("%f vs %f \n", area, area2);
        if (area == area2){
            printf("Empate!");
        }   else if(area > area2){
                printf("Carta 1 venceu!\n");
                } else {
                printf("Carta 2 venceu!\n");
                }
            break;
        case 4:
        printf("Atributo 4: PIB: \n");
        printf("%f vs %f \n", PIB, PIB2);
        if (PIB == PIB2){
            printf("Empate!");
        }   else if(PIB > PIB2){
                printf("Carta 1 venceu!\n");
                } else {
                printf("Carta 2 venceu!\n");
                }
            break;
        case 5:
        printf("Atributo 5: número de pontos turísticos: \n");
        printf("%d vs %d \n", pontosturisticos, pontosturisticos2);
        if (pontosturisticos == pontosturisticos2){
            printf("Empate!");
        }   else if(pontosturisticos > pontosturisticos2){
                printf("Carta 1 venceu!\n");
                } else {
                printf("Carta 2 venceu!\n");
                }
            break;
        case 6:
        printf("Atributo 6: Densidade demográifca: \n");
        printf("%f vs %f \n", densidadepopulacional, densidadepopulacional2);
        if (densidadepopulacional2 == densidadepopulacional){
            printf("Empate!");
        }   else if(densidadepopulacional < densidadepopulacional2){
                printf("Carta 1 venceu!\n");
                } else {
                printf("Carta 2 venceu!\n");
                }
            break;
        default:
            printf("opção inválida!\n");
            break;
        }
    }

float valor1carta1 = 0, valor1carta2 = 0, valor2carta1 = 0, valor2carta2 = 0;

switch(atributo){
case 1 : valor1carta1 = 0; valor1carta2 = 0;
break;
case 2 : valor1carta1 = populacao; valor1carta2 = populacao2; 
break;
case 3 : valor1carta1 = area; valor1carta2 = area2;
break;
case 4 : valor1carta1 = PIB; valor1carta2 = PIB2;
break;
case 5: valor1carta1 = pontosturisticos; valor1carta2 = pontosturisticos2;
break;
case 6: valor1carta1 = densidadepopulacional; valor1carta2 = densidadepopulacional2;
break;
default: printf("Operação inválida!\n");
}

switch(atributo2){
case 1 : valor2carta1 = 0; valor2carta2 = 0;
break;
case 2 : valor2carta1 = populacao; valor2carta2 = populacao2; 
break;
case 3 : valor2carta1 = area; valor2carta2 = area2;
break;
case 4 : valor2carta1 = PIB; valor2carta2 = PIB2;
break;
case 5: valor2carta1 = pontosturisticos; valor2carta2 = pontosturisticos2;
break;
case 6: valor2carta1 = densidadepopulacional; valor2carta2 = densidadepopulacional2;
break;
default: printf("Operação inválida!\n");
}

float somacarta1 = valor1carta1 + valor2carta1; 
float somacarta2 = valor1carta2 + valor2carta2;

printf("\n");
printf("###VENCEDOR DA RODADA!!!###\n");
printf("\n");
printf("País da Carta 1: %s\n", pais);
printf("País da Carta 2: %s\n\n", pais2);
printf("\n");
printf("Atributos comparados: %d e %d\n", atributo, atributo2);
printf("\n");
printf("Carta 1 - %s\n", pais);
printf("  Atributo %d: %.2f\n", atributo, valor1carta1);
printf("  Atributo %d: %.2f\n", atributo2, valor2carta1);
printf("  Soma total:  %.2f\n\n", somacarta1);
printf("\n");
printf("\n");
printf("Carta 2 - %s\n", pais2);
printf("  Atributo %d: %.2f\n", atributo, valor1carta2);
printf("  Atributo %d: %.2f\n", atributo2, valor2carta2);
printf("  Soma total:  %.2f\n", somacarta2);
printf("\n");
printf("\n");

if(somacarta1 > somacarta2){
    printf("Vitória da carta 1!\n");
} else if(somacarta1 < somacarta2){
    printf("Vitória da carta 2!\n");
} else {
    printf("Empate na rodada!!");
}
return 0;
}

