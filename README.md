Include <stdio.h>

Void quick_sort(int[],int,int);

Int partition(int[],int,int);

Int main()

{

	Int a[50],n,i;

	Printf(“How many elements?”);

	Scanf(“%d”,&n);

	Printf(“\nEnter array elements:”);

	For(i=0;i<n;i++)

		Scanf(“%d”,&a[i]);	

	Quick_sort(a,0,n-1);

	Printf(“\nArray after sorting:”);

	For(i=0;i<n;i++)

		Printf(“%d “,a[i]);

	Return 0;		

}

Void quick_sort(int a[],int l,int u)

{

	Int j;

	If(l<u)

	{

		J=partition(a,l,u);

		Quick_sort(a,l,j-1);

		Quick_sort(a,j+1,u);

	}

}

Int partition(int a[],int l,int u)

{

	Int v,i,j,temp;

	V=a[l];

	I=l;

	J=u+1;

	Do

	{

		Do

			I++;		

		While(a[i]<v&&i<=u);

		Do

			j--;

		while(v<a[j]);

			if(i<j)

		{

Temp=a[i];

A[i]=a[j];

A[j]=temp;

}

}

While (i<j);

A[l]=a[j];

A[j]=v;

Return (j);

}
