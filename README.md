# Calculator-not-perfect-
first calculator(not perfect)(calcul.h)
#pragma once
#include<iostream>
#include <math.h>
#include <string>

int x = 0;
int c = 0;
int y = 0;

 

int Sumb(int x, int y);
int Minus(int x, int y);
int Division(int x, int y);
int Multiplication(int x, int y);
int SQRT(int x);
int Pop(int x);


namespace Calcul {

	using namespace System;
	using namespace System::ComponentModel;
	using namespace System::Collections;
	using namespace System::Windows::Forms;
	using namespace System::Data;
	using namespace System::Drawing;

 



	
	
	/// <summary>
	/// Сводка для Calcul
	/// </summary>
	public ref class Calcul : public System::Windows::Forms::Form
	{
	public:
		 
		Calcul(void)
		{
			InitializeComponent();
			//
			//TODO: добавьте код конструктора
			//
		}

	protected:
		/// <summary>
		/// Освободить все используемые ресурсы.
		/// </summary>
		~Calcul()
		{
			if (components)
			{
				delete components;
			}
		}
	private: System::Windows::Forms::TextBox^  textBox1;
	protected:

	private: System::Windows::Forms::Button^  button2;
	private: System::Windows::Forms::Button^  button3;
	private: System::Windows::Forms::Button^  button4;
	private: System::Windows::Forms::Button^  button5;
	private: System::Windows::Forms::Button^  button6;
	private: System::Windows::Forms::Button^  button7;
	private: System::Windows::Forms::Button^  button8;
	private: System::Windows::Forms::Button^  button9;
	private: System::Windows::Forms::Button^  button10;
	private: System::Windows::Forms::Button^  button11;
	private: System::Windows::Forms::Button^  button12;
	private: System::Windows::Forms::Button^  button13;
	private: System::Windows::Forms::Button^  button14;
	private: System::Windows::Forms::Button^  button15;
	private: System::Windows::Forms::Button^  button16;
	private: System::Windows::Forms::Button^  button17;
	private: System::Windows::Forms::Button^  button18;
	/*private: System::Diagnostics::PerformanceCounter^  performanceCounter1;*/


	private:
		/// <summary>
		/// Обязательная переменная конструктора.
		/// </summary>
		System::ComponentModel::Container ^components;

#pragma region Windows Form Designer generated code
		/// <summary>
		/// Требуемый метод для поддержки конструктора — не изменяйте 
		/// содержимое этого метода с помощью редактора кода.
		/// </summary>
		void InitializeComponent(void)
		{
			this->textBox1 = (gcnew System::Windows::Forms::TextBox());
			this->button2 = (gcnew System::Windows::Forms::Button());
			this->button3 = (gcnew System::Windows::Forms::Button());
			this->button4 = (gcnew System::Windows::Forms::Button());
			this->button5 = (gcnew System::Windows::Forms::Button());
			this->button6 = (gcnew System::Windows::Forms::Button());
			this->button7 = (gcnew System::Windows::Forms::Button());
			this->button8 = (gcnew System::Windows::Forms::Button());
			this->button9 = (gcnew System::Windows::Forms::Button());
			this->button10 = (gcnew System::Windows::Forms::Button());
			this->button11 = (gcnew System::Windows::Forms::Button());
			this->button12 = (gcnew System::Windows::Forms::Button());
			this->button13 = (gcnew System::Windows::Forms::Button());
			this->button14 = (gcnew System::Windows::Forms::Button());
			this->button15 = (gcnew System::Windows::Forms::Button());
			this->button16 = (gcnew System::Windows::Forms::Button());
			this->button17 = (gcnew System::Windows::Forms::Button());
			this->button18 = (gcnew System::Windows::Forms::Button());
			this->SuspendLayout();
			// 
			// textBox1
			// 
			this->textBox1->Dock = System::Windows::Forms::DockStyle::Top;
			this->textBox1->Font = (gcnew System::Drawing::Font(L"Microsoft Sans Serif", 20.25F, System::Drawing::FontStyle::Regular, System::Drawing::GraphicsUnit::Point,
				static_cast<System::Byte>(204)));
			this->textBox1->Location = System::Drawing::Point(0, 0);
			this->textBox1->Name = L"textBox1";
			this->textBox1->Size = System::Drawing::Size(361, 38);
			this->textBox1->TabIndex = 0;
			this->textBox1->Text = L"0";
			this->textBox1->TextAlign = System::Windows::Forms::HorizontalAlignment::Right;
			this->textBox1->TextChanged += gcnew System::EventHandler(this, &Calcul::textBox1_TextChanged);
			// 
			// button2
			// 
			this->button2->Location = System::Drawing::Point(31, 51);
			this->button2->Name = L"button2";
			this->button2->Size = System::Drawing::Size(75, 40);
			this->button2->TabIndex = 2;
			this->button2->Text = L"CLEAR";
			this->button2->UseVisualStyleBackColor = true;
			this->button2->Click += gcnew System::EventHandler(this, &Calcul::button2_Click);
			// 
			// button3
			// 
			this->button3->Location = System::Drawing::Point(112, 51);
			this->button3->Name = L"button3";
			this->button3->Size = System::Drawing::Size(75, 39);
			this->button3->TabIndex = 3;
			this->button3->Text = L"SQRT";
			this->button3->UseVisualStyleBackColor = true;
			this->button3->Click += gcnew System::EventHandler(this, &Calcul::button3_Click);
			// 
			// button4
			// 
			this->button4->Location = System::Drawing::Point(193, 231);
			this->button4->Name = L"button4";
			this->button4->Size = System::Drawing::Size(75, 41);
			this->button4->TabIndex = 4;
			this->button4->Text = L"/";
			this->button4->UseVisualStyleBackColor = true;
			this->button4->Click += gcnew System::EventHandler(this, &Calcul::button4_Click);
			// 
			// button5
			// 
			this->button5->Location = System::Drawing::Point(31, 231);
			this->button5->Name = L"button5";
			this->button5->Size = System::Drawing::Size(75, 41);
			this->button5->TabIndex = 5;
			this->button5->Text = L"*";
			this->button5->UseVisualStyleBackColor = true;
			this->button5->Click += gcnew System::EventHandler(this, &Calcul::button5_Click);
			// 
			// button6
			// 
			this->button6->Location = System::Drawing::Point(193, 51);
			this->button6->Name = L"button6";
			this->button6->Size = System::Drawing::Size(75, 40);
			this->button6->TabIndex = 6;
			this->button6->Text = L"-";
			this->button6->UseVisualStyleBackColor = true;
			this->button6->Click += gcnew System::EventHandler(this, &Calcul::button6_Click);
			// 
			// button7
			// 
			this->button7->Location = System::Drawing::Point(29, 96);
			this->button7->Name = L"button7";
			this->button7->Size = System::Drawing::Size(75, 41);
			this->button7->TabIndex = 7;
			this->button7->Text = L"1";
			this->button7->UseVisualStyleBackColor = true;
			this->button7->Click += gcnew System::EventHandler(this, &Calcul::button7_Click);
			// 
			// button8
			// 
			this->button8->Location = System::Drawing::Point(112, 96);
			this->button8->Name = L"button8";
			this->button8->Size = System::Drawing::Size(75, 41);
			this->button8->TabIndex = 2;
			this->button8->Text = L"2";
			this->button8->UseVisualStyleBackColor = true;
			this->button8->Click += gcnew System::EventHandler(this, &Calcul::button8_Click);
			// 
			// button9
			// 
			this->button9->Location = System::Drawing::Point(193, 96);
			this->button9->Name = L"button9";
			this->button9->Size = System::Drawing::Size(75, 41);
			this->button9->TabIndex = 9;
			this->button9->Text = L"3";
			this->button9->UseVisualStyleBackColor = true;
			this->button9->Click += gcnew System::EventHandler(this, &Calcul::button9_Click);
			// 
			// button10
			// 
			this->button10->Location = System::Drawing::Point(29, 143);
			this->button10->Name = L"button10";
			this->button10->Size = System::Drawing::Size(75, 39);
			this->button10->TabIndex = 10;
			this->button10->Text = L"4";
			this->button10->UseVisualStyleBackColor = true;
			this->button10->Click += gcnew System::EventHandler(this, &Calcul::button10_Click);
			// 
			// button11
			// 
			this->button11->Location = System::Drawing::Point(112, 143);
			this->button11->Name = L"button11";
			this->button11->Size = System::Drawing::Size(75, 39);
			this->button11->TabIndex = 11;
			this->button11->Text = L"5";
			this->button11->UseVisualStyleBackColor = true;
			this->button11->Click += gcnew System::EventHandler(this, &Calcul::button11_Click);
			// 
			// button12
			// 
			this->button12->Location = System::Drawing::Point(193, 143);
			this->button12->Name = L"button12";
			this->button12->Size = System::Drawing::Size(75, 39);
			this->button12->TabIndex = 12;
			this->button12->Tag = L"";
			this->button12->Text = L"6";
			this->button12->UseVisualStyleBackColor = true;
			this->button12->Click += gcnew System::EventHandler(this, &Calcul::button12_Click);
			// 
			// button13
			// 
			this->button13->Location = System::Drawing::Point(29, 188);
			this->button13->Name = L"button13";
			this->button13->Size = System::Drawing::Size(75, 39);
			this->button13->TabIndex = 13;
			this->button13->Text = L"7";
			this->button13->UseVisualStyleBackColor = true;
			this->button13->Click += gcnew System::EventHandler(this, &Calcul::button13_Click);
			// 
			// button14
			// 
			this->button14->Location = System::Drawing::Point(112, 188);
			this->button14->Name = L"button14";
			this->button14->Size = System::Drawing::Size(75, 39);
			this->button14->TabIndex = 14;
			this->button14->Text = L"8";
			this->button14->UseVisualStyleBackColor = true;
			this->button14->Click += gcnew System::EventHandler(this, &Calcul::button14_Click);
			// 
			// button15
			// 
			this->button15->Location = System::Drawing::Point(193, 188);
			this->button15->Name = L"button15";
			this->button15->Size = System::Drawing::Size(75, 39);
			this->button15->TabIndex = 15;
			this->button15->Text = L"9";
			this->button15->UseVisualStyleBackColor = true;
			this->button15->Click += gcnew System::EventHandler(this, &Calcul::button15_Click);
			// 
			// button16
			// 
			this->button16->Location = System::Drawing::Point(112, 231);
			this->button16->Name = L"button16";
			this->button16->Size = System::Drawing::Size(75, 41);
			this->button16->TabIndex = 16;
			this->button16->Text = L"0";
			this->button16->UseVisualStyleBackColor = true;
			this->button16->Click += gcnew System::EventHandler(this, &Calcul::button16_Click);
			// 
			// button17
			// 
			this->button17->Location = System::Drawing::Point(274, 51);
			this->button17->Name = L"button17";
			this->button17->Size = System::Drawing::Size(75, 40);
			this->button17->TabIndex = 17;
			this->button17->Text = L"+";
			this->button17->UseVisualStyleBackColor = true;
			this->button17->Click += gcnew System::EventHandler(this, &Calcul::button17_Click);
			// 
			// button18
			// 
			this->button18->Location = System::Drawing::Point(274, 98);
			this->button18->Name = L"button18";
			this->button18->Size = System::Drawing::Size(75, 174);
			this->button18->TabIndex = 18;
			this->button18->Text = L"=";
			this->button18->UseVisualStyleBackColor = true;
			this->button18->Click += gcnew System::EventHandler(this, &Calcul::button18_Click);
			// 
			// Calcul
			// 
			this->AutoScaleDimensions = System::Drawing::SizeF(6, 13);
			this->AutoScaleMode = System::Windows::Forms::AutoScaleMode::Font;
			this->ClientSize = System::Drawing::Size(361, 304);
			this->Controls->Add(this->button18);
			this->Controls->Add(this->button17);
			this->Controls->Add(this->button16);
			this->Controls->Add(this->button15);
			this->Controls->Add(this->button14);
			this->Controls->Add(this->button13);
			this->Controls->Add(this->button12);
			this->Controls->Add(this->button11);
			this->Controls->Add(this->button10);
			this->Controls->Add(this->button9);
			this->Controls->Add(this->button8);
			this->Controls->Add(this->button7);
			this->Controls->Add(this->button6);
			this->Controls->Add(this->button5);
			this->Controls->Add(this->button4);
			this->Controls->Add(this->button3);
			this->Controls->Add(this->button2);
			this->Controls->Add(this->textBox1);
			this->Name = L"Calcul";
			this->Text = L"Calcul";
			this->ResumeLayout(false);
			this->PerformLayout();

		}
		int firstnum;
		int secondnum;
		char operation;
		int result;
		


#pragma endregion
	private: System::Void button7_Click(System::Object^  sender, System::EventArgs^  e) {

		if (textBox1->Text == "0")
		{
			textBox1->Text = "1";
			
		}
		else
		{
			textBox1->Text = System::Convert::ToInt32(textBox1->Text) + "1";
			
		}
	}
private: System::Void button17_Click(System::Object^  sender, System::EventArgs^  e) {

	firstnum = System::Convert::ToInt32(textBox1->Text);
	textBox1->Text = "0";
	operation = '+';
}
private: System::Void button6_Click(System::Object^  sender, System::EventArgs^  e) {
	firstnum = System::Convert::ToInt32(textBox1->Text);
	textBox1->Text = "0";
	operation = '-';
	 
}
private: System::Void button5_Click(System::Object^  sender, System::EventArgs^  e) {
	firstnum = System::Convert::ToInt32(textBox1->Text);
	textBox1->Text = "0";
	operation = '*';
}
private: System::Void button4_Click(System::Object^  sender, System::EventArgs^  e) {
	firstnum = System::Convert::ToInt32(textBox1->Text);
	textBox1->Text="0";
	operation = '/';
	
}
private: System::Void button3_Click(System::Object^  sender, System::EventArgs^  e) {
	firstnum = System::Convert::ToInt32(textBox1->Text);
	SQRT(firstnum);
	textBox1->Text = System::Convert::ToString(c);
	
}

private: System::Void button8_Click(System::Object^  sender, System::EventArgs^  e) {
	if (textBox1->Text == "0")
	{
		textBox1->Text = "2";
		
	}
	else
	{
		textBox1->Text = System::Convert::ToInt32(textBox1->Text) + "2";
	}
}
private: System::Void textBox1_TextChanged(System::Object^  sender, System::EventArgs^  e) {
	//x = System::Convert::ToInt32(textBox1->Text);
}
private: System::Void button18_Click(System::Object^  sender, System::EventArgs^  e) {
	secondnum= System::Convert::ToInt32(textBox1->Text);
	switch (operation)
	{
	case '+':
		result=Sumb(firstnum, secondnum);
		textBox1->Text = System::Convert::ToString(c);
	
	break;
	case '-':
Minus(firstnum, secondnum);
textBox1->Text = System::Convert::ToString(c);
		
		if (result)
		{
			Minus(firstnum, secondnum);
			textBox1->Text = System::Convert::ToString(c);
		}
				
		
		break;
	case '*':
		Multiplication(firstnum, secondnum);
		textBox1->Text = System::Convert::ToString(c);
		break;
	case '/':
		Division(firstnum, secondnum);
		textBox1->Text = System::Convert::ToString(c);
		break;
	case 'SQRT':
		
		break;
	 
	}
}
private: System::Void button9_Click(System::Object^  sender, System::EventArgs^  e) {
	if (textBox1->Text == "0")
	{
		textBox1->Text = "3";
	}
	else
	{
		textBox1->Text = System::Convert::ToInt32(textBox1->Text) + "3";
	}
}
private: System::Void button10_Click(System::Object^  sender, System::EventArgs^  e) {
	
	if (textBox1->Text == "0")
	{
		textBox1->Text = "4";
	}
	else
	{
		textBox1->Text = System::Convert::ToInt32(textBox1->Text) + "4";
	}
}
private: System::Void button11_Click(System::Object^  sender, System::EventArgs^  e) {
	
	if (textBox1->Text == "0")
	{
		textBox1->Text = "5";
	}
	else
	{
		textBox1->Text = System::Convert::ToInt32(textBox1->Text) + "5";
	}
}
private: System::Void button12_Click(System::Object^  sender, System::EventArgs^  e) {
	if (textBox1->Text =="0" )
	{
		textBox1->Text = "6";
	}
	else
	{
		textBox1->Text = System::Convert::ToInt32(textBox1->Text)+"6";
	}
	
}
private: System::Void button13_Click(System::Object^  sender, System::EventArgs^  e) {
	
	if (textBox1->Text == "0")
	{
		textBox1->Text = "7";
	}
	else
	{
		textBox1->Text = System::Convert::ToInt32(textBox1->Text) + "7";
	}
}
private: System::Void button14_Click(System::Object^  sender, System::EventArgs^  e) {

	if (textBox1->Text == "0")
	{
		textBox1->Text = "8";
	}
	else
	{
		textBox1->Text = System::Convert::ToInt32(textBox1->Text) + "8";
	}
}
private: System::Void button15_Click(System::Object^  sender, System::EventArgs^  e) {
	
	if (textBox1->Text == "0")
	{
		textBox1->Text = "9";
	 
	}
	else
	{
		textBox1->Text = System::Convert::ToInt32(textBox1->Text) + "9";
	 
	};
}
private: System::Void button16_Click(System::Object^  sender, System::EventArgs^  e) {

	textBox1->Text = " ";
	textBox1->Text = "0";
	
}

private: System::Void button2_Click(System::Object^  sender, System::EventArgs^  e) {
	textBox1->Text = "0";
	firstnum = 0;
	secondnum = 0;
}
private: System::Void button19_Click(System::Object^  sender, System::EventArgs^  e) {
}
};
}

(calcul.cpp)
#include "Calcul.h"
#include<iostream>
#include <math.h>
 



using namespace System;
using namespace System::Windows::Forms;

 

 
bool value = true;
 
int Sumb(int x, int y)
{
	c = x+y;
 
	return  c;
}

int Minus(int x, int y)
{

	c= x-y;
	return  c;
}
int Division(int x, int y)
{
	c  = x/y;
	 return  c;
}
int Multiplication(int x, int y)
{
	c =x*y;
	return  c;
}
int SQRT(int x)
{
	c=sqrt(x);
	return c;
}
int Pop(int x)
{
	int c = 0;
	std::string str;
	str = std::to_string(x);
	str.pop_back();
	c = atoi(str.c_str());
	return  c;
}


[STAThreadAttribute]
int main(array < String^>^ args) {
	 
	Application::EnableVisualStyles();
	Application::SetCompatibleTextRenderingDefault(false);
	Calcul::Calcul form;
	Application::Run(%form);
 
	


	return 0;
}
