#include <stdio.h>
#include <stdbool.h>

int main(void )
{
	int count = 0;
	int pin;
	double balance = 50;
	int option;
	double deposit;
	double withdraw;
	int status=0;

	do{
		printf("Welcome to Citibank:\n");
		printf("Enter your Pin: **** \n");
		scanf("%d",&pin);

		if(pin == 1449)
		{
			printf("Welcome\n");
			status = 1;
			break;
		}
		count++;
	}
	while(count < 4);

	if(status ==1){
		printf("Valid pin\n");
		do{

			printf("Menu:\n 1.Balance\n 2.Change pin\n 3.Withdraw money\n 4.Deposit money\n 5.Exit\n");
			scanf("%d",&option);
			if (option == 1){
				printf("Your balance is: %lf\n",balance);
			}
			else if(option == 2){
				printf("Enter your new pin\n");
				scanf("%d",&pin);
				printf("Your new pin is %d\n",pin);
			}else if (option == 3){
				printf("How much would you like to deposit?\n");
				scanf("%lf",&deposit);
				balance = balance + deposit;
				printf("Your new balance is %.2lf\n",balance);
			}else if (option == 4) {
				printf("How much would you like to withdraw?\n");
				scanf("%lf",&withdraw);
				if(withdraw > balance) printf("Invalid\n");
				if(balance > 0)
					balance = balance - withdraw;
					printf("Your new balance is %lf\n", balance);
			}else if (option == 5){
				printf("Thank you for using Citibank!");
			}
		}
		while(option != 5);
		}else{
			printf("You are out of tries");

		}
		return 0;

	}
