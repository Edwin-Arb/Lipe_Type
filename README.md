#include<iostream>
using namespace std;

void main()
{
	setlocale(LC_ALL, "ru");

	int sybol_count;
	char sybol;
	int line_type;
	int index = 0;

	cout << "Введите количество символом: " << endl;
	cin >> sybol_count;

	cout << "Введите символ:" << endl;
	cin >> sybol;

	cout << "Введите тип линии" << endl
		<< "1.Вертикальная" << endl
		<< "2.Горизонтальная" << endl;
	cin >> line_type;

	if (line_type!=1 && line_type!=2)
	{
		cout << "Не корректный тип линии!" << endl;
			return;
	}

	while (index<sybol_count)
	{
		if (line_type==1)
		{
			cout << sybol << endl;
		}
		if (line_type==2)
		{
			cout << sybol;
		}
		index++;
	}
	cout << endl << endl;
}
