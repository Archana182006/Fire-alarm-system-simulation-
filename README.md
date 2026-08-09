#include <stdio.h>

int main() {
    int smoke, temperature, flame;

    printf("===== FIRE ALARM SYSTEM SIMULATION =====\n");

    printf("\nEnter smoke level (0 = No Smoke, 1 = Smoke Detected): ");
    scanf("%d", &smoke);

    printf("Enter temperature level (0 = Normal, 1 = High): ");
    scanf("%d", &temperature);

    printf("Enter flame status (0 = No Flame, 1 = Flame Detected): ");
    scanf("%d", &flame);

    printf("\n----- SYSTEM STATUS -----\n");

    if (smoke == 1 || temperature == 1 || flame == 1) {
        printf("WARNING! Fire detected!\n");
        printf("Fire Alarm: ON\n");
        printf("Buzzer: ON\n");
        printf("Emergency Alert: ACTIVE\n");
    } 
    else {
        printf("Environment is safe.\n");
        printf("Fire Alarm: OFF\n");
        printf("Buzzer: OFF\n");
    }

    return 0;
}
