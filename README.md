# Cospro-8
  #include<stdio.h>

int main(void)
{
	int num = 0;
	int i = 2;
	int j = 0;
	int cnt = 0;
	int sum = 0;
	printf("1-num까지의 계차 수열의 합을 구하세요 num 을 입력하세요:");
	scanf_s("%d", &num);
	printf("\n\n\nfor문 이용\n\n\n");
	
	for (i =2; i <= num;i+=j)
	{
		
		j += 1;
		sum += i;
		
		printf("cnt = %2d, j= %2d , i= %3d, sum = %d\n", cnt,j , i,sum);
		
	}

	printf("\n\n\nwhile문 이용 \n\n\n");
	i = 2; //i 초기화
	sum = 0;
	j = 0;
	while (i<=num)
	{

		j += 1;
		
		sum += i;

		printf("cnt = %2d, j= %2d , i= %3d, sum = %d\n", cnt, j, i, sum);
		i = i + j;
	}

	printf("\n\n\ndo while문 이용 \n\n\n");
	i = 2; //i 초기화
	sum = 0;
	j = 0;
	do
	{

		j += 1;

		sum += i;

		printf("cnt = %2d, j= %2d , i= %3d, sum = %d\n", cnt, j, i, sum);
		i = i + j;
	} while (i <= num);
	return 0;
}
/*
//sum += i ;
//printf("cnt = %2d, j= %2d , i= %3d, sum = %d\n", cnt, j, i, sum);

for (cnt =1; cnt < num;cnt++)
	{
		if(num>=cnt) break;
		j += 1;
		i += j;
		sum += i;

		printf("cnt = %2d, j= %2d , i= %3d, sum = %d\n", cnt,j , i,sum);

	}

*/
/*
	int num = 0;
	int i = 0;
	int sum = 0;
	printf("1-num까지의 합을 구하세요 num을 입력하세요 :");
	scanf_s("%d", &num);
	printf("\n\n\nfor문 이용\n\n\n");
	for (i = 1; i <= num;i++)
	{
		//sum = sum + 1;
		sum += i;
		//printf("%d %d\n", i, sum);


		printf("%d + ", i);
	}

	printf("\b\b = %d\n\n\n", sum); //backspace를 이용하여 + 지우기


	printf("\n\n\nwhile문 이용 \n\n\n");
	i = 1; //i 초기화
	sum = 0;
	while (i <= num)
	{
		//sum = sum + 1;
		sum += i;
		//printf("%d %d\n", i, sum);
		printf("%d + ", i);
		i++;


	}

	printf("\b\b = %d\n\n\n", sum); //backspace를 이용하여 + 지우기

	printf("\n\n\ndo while문 이용 \n\n\n");
	i = 1; //i 초기화
	sum = 0;
	do
	{
		//sum = sum + 1;
		sum += i;
		//printf("%d %d\n", i, sum);
		printf("%d + ", i);
		i++;


	} while (i <= num);

	printf("\b\b = %d\n\n\n", sum); //backspace를 이용하여 + 지우기


	return 0;
*/
