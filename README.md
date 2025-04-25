#include <stdio.h>

int main() {
    int n;

    printf("Gib eine positive ganze Zahl ein: ");
    scanf("%d", &n);

    if (n <= 0) {
        printf("Bitte eine positive Zahl größer als 0 eingeben.\n");
        return 1;
    }

    while (n != 1) {
        printf("%d -> ", n);
        if (n % 2 == 0) {
            n = n / 2;
        } else {
            n = 3 * n + 1;
        }
    }

    printf("1\n");
    return 0;
}
