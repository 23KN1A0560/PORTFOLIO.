# PORTFOLIO
#include <stdio.h>

void aboutMe() {
    printf("\n=== About Me ===\n");
    printf("Hello! I'm a developer passionate about C programming and software development.\n");
}

void projects() {
    printf("\n=== My Projects ===\n");
    printf("1. Calculator – A basic arithmetic calculator using C.\n");
    printf("2. File Manager – A simple file operations utility.\n");
}

void contact() {
    printf("\n=== Contact Me ===\n");
    printf("Email: your.email@example.com\n");
}

int main() {
    int choice;

    while (1) {
        printf("\n--- Portfolio Menu ---\n");
        printf("1. About Me\n");
        printf("2. Projects\n");
        printf("3. Contact\n");
        printf("4. Exit\n");
        printf("Enter your choice: ");
        scanf("%d", &choice);

        switch (choice) {
            case 1:
                aboutMe();
                break;
            case 2:
                projects();
                break;
            case 3:
                contact();
                break;
            case 4:
                printf("Exiting...\n");
                return 0;
            default:
                printf("Invalid choice. Please try again.\n");
        }
    }

    return 0;
}
