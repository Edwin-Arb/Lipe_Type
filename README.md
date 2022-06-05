#include<iostream>
using namespace std;

void main()
{
	setlocale(LC_ALL, "ru");

	int sybol1count;
	char sybol;
	int lineType;
	int index = 0;
	
	cout << "Введите количетсво символов: " << endl;
	cin >> sybol1count;

	cout << "Введите символ: " << endl;
	cin >> sybol;

	cout << "Выберите тип линии: " << endl
		<< "1. Горизонтальный " << endl
		<< "2. Вертикальный" << endl;
	cin >> lineType;

	if (lineType!=1&&lineType!=2)
	{
		cout << "Не корректный тип линии!" << endl;
		return;
	}
	while (index<sybol1count)
	{
		if (lineType == 1)
		{
			cout << sybol;
		}
		if (lineType==2)
		{
			cout << sybol<<endl;
		}	
		index++;	
	}
	cout << endl << endl;
