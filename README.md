#include <iostream>
using namespace std;

int main()
{
	setlocale(LC_ALL, "ru");
	int x;
q:
	cout << "ты червяк?\n1 - да\n2 - нет" << endl;
	cin >> x;
	switch (x)
	{
	case 1:
		cout << "попался, червяк" << endl;
		break;
	case 2:
		cout << "ну ладно, пока поверю" << endl;
		break;
	default:
		cout << "давай без глупостей" << endl << endl;
		goto q;
		break;
	}
}
