# Dmitry Matsuyshou
## Telephone +375(29)7757806, e-mail ivan6613d@gmail.com
## Currently I have been working as an economist for 3.5 years. I have 10 years of experience in the bank. I graduated from the STEPIK courses, I have been studying at the IIT BSUIR for almost a year. There is a desire to learn new things.
## Create an array of 100 integer elements. Fill it with random numbers ranging from A to B. Enter A and B from the keyboard (select their values ​​so as to get the correct result).Display the resulting array. For the resulting array, determine the number of repeated elements and their value.
### {
	int A = 0, B = 0;
	const int SIZE = 100;
	int arr[SIZE]{};

	cout << "Enter A " << endl;
	cin >> A;
	cout << "Enter B " << endl;
	cin >> B;
	cout << "Array" << endl;

	for (int i = 0; i < 100; i++)
	{
		arr[i] = A + rand() % (B - A + 1);
	}

	for (int i = 0; i < 100; i++)
	{
		cout << arr[i] << "\t";
		if (i + 1) % 10 == 0)
		{
			cout << endl;
		}
	}

	int RepetElem = 0, j = 0, k = 0;
	cout << "Repeat element " << endl;
	for (int i = 0; i < 100; i++)
	{
		RepetElem = arr[i];
		for (int j = i + 1; j < 100; j++)
		{
			if (RepetElem == arr[j])
			{
				cout << arr[j] << "\t";
				k++;
				if (k % 10 == 0)
				{
					cout << endl;
				}
				break;
			}
		}
	}
	cout << endl << "Value of repeat elements " << k << endl;
	_getwch();
} 

### No experience in IT. There are C ++, C #, OOP basics.
#### My level of english is about a2