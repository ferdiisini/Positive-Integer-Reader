#include <conio.h>
#include <ctype.h>
#include <math.h>
#include <stdio.h>
#include <stdlib.h>
#include <string.h>


int main() {
	char str[10];
	char strclone[10];
	int alphabet = 0;
	int number = 0;
	int numflag = 0;
	int negative = 1;
	int negativeflag = 0;
	int removedot = 0;
	int i;
	scanf("%s", &str);
	while (numflag != 1) {
		for (i = 0; str[i] != '\0'; i++) {
			// check for alphabets and other chars
			if (ispunct(str[i]) != 0 || isalpha(str[i]) != 0) {
				alphabet++;
			}
		}
		//check for '-'
		if ((str[0]) == '-' && alphabet == 1) {
			if(strlen(str)==1){
			alphabet++;
			}
			alphabet--;
			negative = -1;
			negativeflag = 1;
		}
		if ((str[i]) == '.' && alphabet == 1) {
			if(strlen(str)==1){
			alphabet++;
			}
			alphabet--;
			removedot++;
		}
		if (alphabet > 0) {
			printf("\nInvalid option! Please enter an interger!\n");
			printf("Enter a number : ");
			scanf("%s", &str);
			alphabet = 0;
		}
		else {
			numflag = 1;
		}
	}

	for (i = 0; str[i] != '\0'; i++) {
		if (negativeflag == 1) {
			strclone[i] = str[i + negativeflag];
		}
		else {
			strcpy(strclone, str);
		}
	}
	for (i = 0; str[i] != '\0'; i++){
		
	}
	
	strrev(strclone);
	for (i = 0; strclone[i] != '\0'; i++) {
		number = (strclone[i] - 48) * pow(10, i) + number;
	}
	number = number * negative;
	numflag = 0;
	return number;
}
