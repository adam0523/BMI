# BMI
#include<iostream>
int main()
//BMI
{
	double weight, height, BMI;
	std::cout << "enter your height(cm):\n";
	std::cin >> height;
	std::cout << "enter your weight(kg):\n";
	std::cin >> weight;
	height = height / 100.0;
	BMI = weight / (height*height);
	std::cout << "BMI is:" << BMI;
	if (BMI < 18.5)
		std::cout << "  underweight  ";
	else if (18.5 <= BMI && BMI < 24.9)
		std::cout << "  normal  ";
	else if (25.0 <= BMI && BMI < 29.9)
		std::cout << "  Overweight  ";
	else if (30.0 <= BMI)
		std::cout << "  Obese  ";
	system("pause");
	return 0;
}
