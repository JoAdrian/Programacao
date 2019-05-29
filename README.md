#include <stdio.h>
#include <string.h>

struct matriz{
    int linhas;
    int colunas;
    float x[50][50];
};
struct matriz a, b, c;
void mat(struct matriz m){
    int i, j;
    for(i = 0; i < m.linhas; i++){
        for(j = 0; j < m.colunas; j++){
            printf("%f", m.x[i][j]);
        }
        printf("\n");
    }
}
void mat2(struct matriz m){
    int i, j;
    for(i = 0; i < m.linhas; i++){
        for(j = 0; j < m.colunas; j++){
            printf("%f", m.x[i][j]);
        }
        printf("\n");
    }
}

int main()
{
    int i, j;

    printf("Digite a quantidade de linhas:\n");
    scanf("%d", &a.linhas);
    printf("Digite a quantidade de colunas:\n");
    scanf("%d", &a.colunas);
    printf("Digite os elementos da matriz:\n");
    for(i = 0; i < a.linhas; i++){
        for(j = 0; j< a.colunas; j++){
            printf("Digite um numero:\n");
            scanf("%d", &a.x[i][j]);
        }
    }
    printf("A matriz a e:\n");
    mat(a.linhas, a.colunas);

    printf("Digite a quantidade de linhas:\n");
    scanf("%d", &b.linhas);
    printf("Digite a quantidade de colunas:\n");
    scanf("%d", &b.colunas);
    printf("Digite os elementos da matriz:\n");
    for(i = 0; i < b.linhas; i++){
        for(j = 0; j< b.colunas; j++){
            printf("Digite um numero:\n");
            scanf("%d", &b.x[i][j]);
        }
    }
    printf("A matriz b e:\n");
    mat2(b.linhas, b.colunas);
    return 0;
}
