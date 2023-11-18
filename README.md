# study
#include<stdio.h>
int main()
{
	int a[10];
	int b[20];
	int cot=1;
	for (int i = 0;i < 10;i++) {
		scanf("%d", &a[i]);
	}
	b[0] = a[0];
	for (int t = 0;t < 10;t++) {
		int ret = 1;
		for (int n = 0;n < cot;n++) {
			if (b[n] == a[t]) {
				ret = 0;
			}
		}
		if (ret == 1) {
			b[cot] = a[t];
			cot++;
		}
	}
	for (int e = 0;e < cot;e++) {
		printf("%d", b[e]);
	}
	return 0;
}
