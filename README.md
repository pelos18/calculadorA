#include <iostream> 
#include <math.h> 
  
using namespace std; 

int RESULTADO; 
float RESULTADO2; 
  
int Numero1; 
int Numero2; 
float Numero3; 
float Numero4; 


  
int Multiplic(int a, int b) 
{ 
    return (a) * (b); 
} 
  
int Divis(int a, int b) 
{ 
    return (a) / (b); 
} 
  
int Sum(int a, int b) 
{ 
    return (a) + (b); 
} 
  
int Rest(int a, int b) 
{ 
    return (a) - (b); 
} 
  
float RaizCu(float a) 
{ 
    return sqrt(a); 
} 
  
float Potenc(float base, float exponente) 
{ 
    return pow(base, exponente); 
} 

int main(){ 
    
    int a; 
    char b; 
    
    	system("color 1d");
	
	printf("\n\n\n                                             INSTITUTO POLITECNICO NACIONAL");
	
	printf("\n                                   ESCUELA SUPERIOR DE INGENIERIA MECANICA Y ELECTRICA");
	
	printf("\n                                               UNIDAD CULHUACAN");
	printf("\n\n\n                                              Fecha de entrega: 20/08/2019");      
	printf("\n\n\n                                              Maestro: ALBERTO BALBOA RIVADENERIO");
	printf("\n\n\n                                         Materia: Fundamentos de programacion");
	printf("\n\n\n                                                       Practica: 8");
	printf("\n                                      Convertir pulgadas a metros y dolares a pesos");
	printf("\n\n\n                                             Alumno: MANUEL ALEJANDRO OLIVARES MORALES");
	printf("\n\n\n                                                       Grupo: 2MC3");
    
    
    
    
    
    
    
    cout << " by pelos never nuke" << endl; 
    cout << "Que operacion desea realizar? (1 - Sumar, 2 - Restar, 3 - Multiplicar, 4 - Dividir, 5 - Raiz Cuadrada, 6 - Potencia, 7 - Seno, 8 - Coseno, ,10 - Tangente )" << endl; 
    cin >> a; 
    
    switch(a) 
    { 
             case 1: 
             cout << "Ingrese el primer digito:" << endl; 
             cin >> Numero1; 
              
             cout << "Ingrese el segundo digito:" << endl; 
             cin >> Numero2; 
             RESULTADO = Sum(Numero1, Numero2); 
             cout << "Resultado: " << RESULTADO << endl; 
             break; 
              
             case 2: 
             cout << "Ingrese el minuendo:" << endl; 
             cin >> Numero1; 
              
             cout << "Ingrese el sustraendo:" << endl; 
             cin >> Numero2; 
              
             RESULTADO = Rest(Numero1, Numero2); 
             cout << "Resultado: " << RESULTADO << endl; 
             break; 
              
             case 3: 
             cout << "Ingrese el primer factor:" << endl; 
             cin >> Numero1; 
              
             cout << "Ingrese el segundo factor:" << endl; 
             cin >> Numero2; 
              
             RESULTADO = Multiplic(Numero1, Numero2); 
             cout << "Resultado: " << RESULTADO << endl; 
             break; 
              
             case 4: 
             cout << "Ingrese el dividendo:" << endl; 
             cin >> Numero1; 
              
             cout << "Ingrese el divisor:" << endl; 
             cin >> Numero2; 
              
             RESULTADO = Divis(Numero1, Numero2); 
             cout << "Resultado: " << RESULTADO << endl; 
             break; 
              
             case 5: 
             cout << "Ingrese el numero para realizar la raiz:" << endl; 
             cin >> Numero3; 
              
             RESULTADO2 = RaizCu(Numero3); 
             cout << "Resultado: " << RESULTADO2 << endl; 
             break; 
              
             case 6: 
             cout << "Ingrese el numero a potenciar:" << endl; 
             cin >> Numero3; 
              
             cout << "Ingrese el exponente:" << endl; 
             cin >> Numero4; 
              
             RESULTADO2 = Potenc(Numero3, Numero4); 
             cout << "Resultado: " << RESULTADO2 << endl; 
             break; 
              
             case 7: 
             cout << "Ingrese el angulo de seno:" << endl; 
             cin >> Numero3; 
              
             RESULTADO2 = sin(Numero3); 
             cout << "Resultado: " << RESULTADO2 << endl; 
             break; 
              
             case 8: 
             cout << "Ingrese el angulo de Coseno:" << endl; 
             cin >> Numero3; 
              
             RESULTADO2 = cos(Numero3); 
             cout << "Resultado: " << RESULTADO2 << endl; 
             break; 
             
             case 10: 
             cout << "Ingrese el angulo de Tangente:" << endl; 
             cin >> Numero3; 
              
             RESULTADO2 = tan(Numero3); 
             cout << "Resultado:" << RESULTADO2 << endl; 
             break; 
  
             default: 
             cout << "Operacion incorrecta. Vuelva a intentarlo... n" << endl; 
             cout << "********************************************" << endl; 
             cout << "******************************************** n" << endl; 
             main(); 
             } 
              
             cin.get(); 
             cout << "Desea salir? (1 - Si, 2 - No)" << endl; 
             cin >> b; 
              
             switch(b){ 
                       case '1': 
                            return 0; 
                            break; 
                       case '2': 
                            cout << "-------------------------------" << endl; 
                            cout << "------------------------------- n" << endl; 
                            main(); 
                            break; 
                            } 
             } 
