#include <unistd.h>
#include <stdio.h>
int
main ()
{
  int a[10] = { 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 };
  int somaFilho = 0, somaPai = 0, n, i;
  n = fork ();

  if (n > 0)
    {
      for (i = 0; i < 10; i++)
	{
	  if (a[i] % 2 == 0)
	    somaPai = somaPai + a[i];
	}
      printf("Processo Pai \n");
      printf("Soma do Processo pai e %d \n",somaPai);
    }

  else
    {
      for (i = 0; i < 10; i++)
	{
	  if (a[i] % 2 != 0)
	    somaFilho = somaFilho + a[i];
	}
      printf("Processo filho \n");
      printf("Soma dos Processos e %d \n", somaFilho);
      
    }
  return 0;
}
