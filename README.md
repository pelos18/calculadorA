




























#include <iostream> 
#include <math.h> 
#include <windows.h>
#include <stdlib.h>

  
using namespace std; 
int RESULTADO; 
float RESULTADO2; 
float lado1,lado2,ladoa,ladob,ladoc,ladod,menord,mayorD,perimetro,apotema,area,p,diametro,radio,area2,h;
float pi= 3.14159265358979323846;
int Numero1; 
int Numero2; 
float Numero3; 
float Numero4; 
int a,b,c;
int x1,x2;
int Multiplic(int a, int b) 
{ 
    return (a) * (b); 
} 
  
int Divis(int a, int b) 
{ 
    return (a) / (b); 
} 

float RaizCu(float a) 
{ 
    return sqrt(a); 
} 
  
float Potenc(float base, float exponente) 
{ 
    return pow(base, exponente); 
} 
int i,n,s,x;
float suma (){
	 s = 0;	
	 s=s+x;
}
int m,r,o;
float resta (){
	  s = 0;	
	 s=s-x;
}
float ecu ( ){
	float sol1= 0,sol2= 0;

}
void gotoxy(int x, int y ){
	HANDLE hcon= GetStdHandle(STD_OUTPUT_HANDLE);
	COORD dwPos;
	dwPos.X=x;
	dwPos.Y=y;
	SetConsoleCursorPosition(hcon,dwPos);
}
void pintar_limites(){
	for(int i = 2;i<78;i++){
		gotoxy(i,3);printf("%c",205);
		gotoxy(i,33);printf("%c",205);	
	}
	for(int i =4 ;i<33;i++){
		gotoxy(2,i);printf("%c",186);
		gotoxy(77,i);printf("%c",186); 
	}
	gotoxy(2,3);printf("%c",201);
	gotoxy(2,33);printf("%c",200);
	gotoxy(77,3);printf("%c",187);
	gotoxy(77,33);printf("%c",188);
}
int main(){
	 int a; 
     char b;
	 system("color 0B");
     gotoxy(23,4);printf(" INSTITUTO POLITECNICO NACIONAL");
	 gotoxy(10,5);printf("ESCUELA SUPERIOR DE INGENIERIA MECANICA Y ELECTRICA");
	 gotoxy(22,6);printf(" UNIDAD CULHUACAN");
	 gotoxy(21,7);printf("Fecha de entrega:");      
 	 gotoxy(19,8);printf("Maestro: ALBERTO BALBOA RIVADENERIO");
	 gotoxy(17,9);printf("Materia: PROGRAMACION DIRIGIDA A OBJETOS ");
	 gotoxy(23,10);printf("PROYECTO ");
	 gotoxy(22,11);printf("CALCULADORA CIENTIFICA ");
	 gotoxy(12,12);printf("Alumno: MANUEL ALEJANDRO OLIVARES MORALES");
	 gotoxy(23,13);printf("Grupo: 2MC3");
	 gotoxy(13,14);cout <<"by pelos never nuke" << endl; 
     gotoxy(4,15);cout << "Que operacion desea realizar? 1-Sumar, 2-Restototar,3-Multiplicar" << endl; 
     gotoxy(7,16);cout<<"4-Dividir,5-Raiz Cuadrada,6-Potencia,7-raiz¹,"<<endl;
     gotoxy(11,17);cout <<"8 -Seno,9-Coseno,10-Tangente ,"<< endl;
     gotoxy(11,18);cout <<"11-CONVERTIDOR,12-Ecuacion segundo Grado"<<endl;
     gotoxy(11,19);cout<<"13-Perimetro y area de algunas figuras "<<endl;
     pintar_limites();
	 gotoxy(12,20);cin >> a;
	 pintar_limites();  
      switch(a) {
      	case 1:
      		system("cls");
      		gotoxy(23,4);cout<<"dame la cantidad de nuemeros  que desaes sumar "<<endl;
      		pintar_limites();
	         gotoxy(23,5);cin>>n;
	         s = 0;
	         for(i=1;i<=n;i++){
	         	system("cls");
	         	pintar_limites();
		         gotoxy(23,4);cout<<"Numero a sumar"<<endl;
		         gotoxy(23,5);cin>>x;
		         s=s+x;
	             }
	             system("cls");
	             pintar_limites();
	             gotoxy(23,4);cout<<"la suma es: "<< s <<endl;
	             pintar_limites(); 
	         return 0 ;
	         break;
	         case 2:
	         	system("cls");
	         	pintar_limites();
	         	break;
	         	case 3:
	         		system("cls");
	         		pintar_limites();
	         		gotoxy(23,4);cout << "Ingrese el primer factor:" << endl;
	         		gotoxy(23,5);cin >> Numero1;
	         		gotoxy(23,6);cout << "Ingrese el segundo factor:" << endl;
	         		gotoxy(23,7);cin >> Numero2;
	         		RESULTADO = Multiplic(Numero1, Numero2); 
	         		pintar_limites();
	         		system("cls");
	         		pintar_limites();
	         		gotoxy(23,4);cout << "Resultado: " << RESULTADO << endl;
	         		pintar_limites();
	         		break;
					 case 4:
					 system("cls");
					 pintar_limites();
					 gotoxy(23,4);cout << "Ingrese el dividendo:" << endl; 
					 gotoxy(23,5);cin >> Numero1;
					 gotoxy(23,6);cout << "Ingrese el divisor:" << endl; 
					 gotoxy(23,7);cin >> Numero2;
					 RESULTADO = Divis(Numero1, Numero2); 
					 system("cls");
					 pintar_limites();
					 gotoxy(23,5);cout << "Resultado: " << RESULTADO << endl;
					 pintar_limites();
					 break;
					 case 5:
					 system("cls");
					 pintar_limites();
					 gotoxy(23,4);cout << "Ingrese el numero para realizar la raiz:" << endl; 
					 gotoxy(23,5);cin >> Numero3;
					 RESULTADO2 = RaizCu(Numero3);
					 system("cls");
					 pintar_limites();
					 gotoxy(23,4);cout << "Resultado: " << RESULTADO2 << endl;
					 pintar_limites(); 
					 break;
					 case 6:
					 	system("cls");
					 	pintar_limites();
					 	gotoxy(23,4);cout << "Ingrese el numero a potenciar:" << endl; 
					 	gotoxy(23,5);cin >> Numero3; 
					 	gotoxy(23,6);cout << "Ingrese el exponente:" << endl; 
					 	gotoxy(23,7);cin >> Numero4; 
					 	RESULTADO2 = Potenc(Numero3, Numero4);
					 	system("cls");
					 	pintar_limites();
					 	gotoxy(23,8);cout << "Resultado: " << RESULTADO2 << endl;
					 	pintar_limites();
					 break;
					 case 7:
					 system("cls");
					 pintar_limites();
					 gotoxy(23,4);cout << "Ingrese el numero a potenciar :" << endl;
					 gotoxy(23,5);cin >> Numero3;
					 gotoxy(23,6);cout << "Ingrese el  numero subradical:" << endl;
					 gotoxy(23,7);cin >> Numero4; 
					 RESULTADO2 = Potenc(Numero3, 1/Numero4);
					 system("cls");
					 pintar_limites();
					 gotoxy(23,8);cout << "Resultado: " << RESULTADO2 << endl; 
					 system("cls");
					 pintar_limites();
					 break;
					 case 8:
					 	system("cls");
					 	pintar_limites();
					 	gotoxy(23,4);cout << "Ingrese el angulo de seno:" << endl; 
					 	gotoxy(23,5);cin >> Numero3;   
					 	RESULTADO2 = sin(Numero3); 
					 	gotoxy(23,6);cout << "Resultado: " << RESULTADO2 << endl;
					 	
					 	pintar_limites();
					 	break;
						 case 9:
						 system("cls");
						 pintar_limites();
						 gotoxy(23,4);cout << "Ingrese el angulo de Coseno:" << endl;
						 gotoxy(23,5);cin >> Numero3; 
						 RESULTADO2 = cos(Numero3);
						 system("cls");
						 pintar_limites();
						 gotoxy(23,4);cout << "Resultado: " << RESULTADO2 << endl;
						 pintar_limites();
						 break;
						 case 10:
						 	system("cls");
						 	pintar_limites();
						 	gotoxy(23,4);cout << "Ingrese el angulo de Tangente:" << endl;
						 	gotoxy(23,5);cin >> Numero3;
						 	RESULTADO2 = tan(Numero3);
						 	system("cls");
						 	pintar_limites();
						 	gotoxy(23,4);cout << "Resultado:" << RESULTADO2 << endl;
						 	pintar_limites();
						 	break;
							 case 11:
							 system("cls");
							 pintar_limites();
							 float km, hm, dam, m, dm, cm, mm;
                             float l,ml,dl,mmc,cmc,dmc,mc,inc,ftc,ydc,gal,oz;
                             system("cls");
                             pintar_limites();
                             gotoxy(30,3);cout<<"byePELOSNEVERNUKE"<<endl;
                             gotoxy(18,4);cout<<"que desea convertir: 1-distancias   2-volumen"<<endl;
                             gotoxy(33,5);cin>>a;
                             switch(a) {
                             	case 1 :
                             		pintar_limites();
                             		system("cls");
                             		pintar_limites();
                             		 gotoxy(22,4);cout<<  "Dime cuantos metros quieres convertir:" << endl;
			                         gotoxy(22,5);cin >> m;
			                         system("cls");
			                         pintar_limites();
			                         km = m*1000;
			                         gotoxy(22,4);cout<< "En"  << m <<  "metro(s) hay " << km << "” kilometros”" << endl;
			                         hm = km/10;
			                         gotoxy(22,5);cout<<"En"   << m << "metro(s) hay " << hm <<  "” hectometros”"<< endl;
			                         dam = hm/10;
			                         gotoxy(22,6);cout<< "En"  << m << "metro(s) hay " << dam << "” decametros” "<< endl;
			                         m = m;
			                         gotoxy(22,7);cout<< "En"  << m << "metro(s) hay " << m <<  "” metros”"<< endl;
			                         dm = m/10.0;
			                         gotoxy(22,8);cout<< "En" << m << "metro(s) hay " << dm <<   "” decimetros”"<< endl;
			                         cm = dm/10.0;
		 	                         gotoxy(22,9);cout<< "En"   << m << "metro(s) hay " << cm << "” centimetros”"  << endl;
			                         mm = cm/10.0;
			                         gotoxy(22,10);cout<<  "En"  << m << "metro(s) hay " << mm <<  "” milimetros”" << endl;
			                         pintar_limites();
			                         return 0;
			                         break;
			                         case 2:
									 system("cls");
									 pintar_limites();	                                                                                                                      
            	                     gotoxy(22,4);cout<<  "Dime cuantos litros  quieres convertir:" << endl;
                                     gotoxy(22,5);cin >>l;
                                     system("cls");
                                     pintar_limites();
                                     ml=l*1000;
                                     gotoxy(20,4);cout<< "En:"        <<     l         <<     "litro(s) hay " <<    ml  <<    "  MILITRO" << endl;
                                     dl=l*10;  
                                     gotoxy(20,5);cout<< "En:"        <<   l           <<    "litro(s) hay " <<    dl <<   " DECI LITRO" << endl;
                                     mmc=l*1000000;
                                     gotoxy(20,6);cout<< "En:"        <<     l        <<    "litro(s) hay " <<     mmc                         <<   " MILIMETRO CUBICO " << endl;	
                                     cmc= l /0.0010000;
                                     gotoxy(20,7);cout<< "En:"        <<     l      <<    "litro(s) hay " <<     cmc                          <<   " CENTIMETRO CUBICO " << endl;
                                     dmc=l=l;
                                     gotoxy(20,8);cout<< "En:"      <<   l      <<    "litro(s) hay " <<     dmc                         <<   " DECIMETRO CUBICO " << endl;
                                     mc=l/ 1.000;
                                     gotoxy(20,9);cout<< "En:"   <<   l      <<    "litro(s) hay " <<     mc                          <<   " METRO CUBICO " << endl;	
                                     inc=l* 61.024;	
                                     gotoxy(20,10);cout<< "En:"   <<   l      <<    "litro(s) hay " <<    inc                         <<   " PULGADAS CUBICAS IN^3" << endl;	
                                     ftc=l* 0.035315;	
                                     gotoxy(20,11);cout<< "En:"   <<   l    <<    "litro(s) hay " <<  ftc                         <<   " PIES CUBICOS  ft^3" << endl;
                                     ydc=l/0.0013080;
                                     gotoxy(20,12);cout<< "En:"   <<   l    <<    "litro(s) hay " <<  ydc                          <<   " YARDA CUBICA   yd^3" << endl;
                                     gal=l*0.26417205;
                                     gotoxy(20,13);cout<< "En:"   <<   l    <<    "litro(s) hay " <<  gal                          <<   " GALONES AMERICANOS " << endl;
                                     oz=l*33.814;
                                     gotoxy(20,14);cout<< "En:"   <<   l    <<    "litro(s) hay " << oz                          <<   " OZAS LIQUIDAS  ESTADO UNIDENCES " << endl;
									 pintar_limites();                                                                                                                                 
                                     break;
						       	    }
							 break;
							 case 12:
							 	system("cls");
							 	pintar_limites();
							     gotoxy(23,4);cout<<"ingresa los balores de A,B,C de la ecuacion "<<endl;
							     gotoxy(23,5);cout<<"ingresa los balores de A "<<endl;                                                                                               	                                 	                                                                                                                                                  
                                 gotoxy(23,6);cin>>a;
                                 system("cls");
                                 pintar_limites();
                                 gotoxy(23,4);cout<<"ingresa los balores de B "<<endl;
							     gotoxy(23,5);cin>>b;
							     system("cls");
							     pintar_limites();
							     gotoxy(23,4);cout<<"ingresa los balores de c "<<endl;
							     gotoxy(23,5);cin>>b;
							     x1=(-b+sqrt(pow(b,2)-4*a*b))/(2*a);
							     x2=(-b-sqrt(pow(b,2)-4*a*b))/(2*a);
							     system("cls");
							     pintar_limites();
							     gotoxy(23,4);cout<<"el valor de X1 ES :"<<x1<<endl;
							     gotoxy(23,5);cout<<"el valor de X2 ES :"<<x2<<endl;
							     pintar_limites();
							     break;
							         case 13:
							         	system("cls");
							         	pintar_limites();
							             gotoxy(19,4);cout<<"Que desea realizar *solo poligonos regulares*"<<endl;
							             gotoxy(23,5);cout<<"1.-PERIMETRO2"<<endl;
							             gotoxy(39,5);cout<<"2.-AREA"<<endl;
	                                     gotoxy(25,6);cin >> a;
	                                     pintar_limites();
	                                     system("cls");
	                                     switch(a) {
	                                     	case 1:
	                                     	system("cls");
	                                     	pintar_limites();
	                                     	gotoxy(14,4);cout<<"Que figura desea sacar el perimetro *poligonos regulares*"<<endl;
	                                     	gotoxy(19,5);cout<<"1.-Cuadredo"<<endl;
	                                     	gotoxy(37,5);cout<<"2.-Rectangulo"<<endl;
	                                     	gotoxy(19,6);cout<<"3.-Trianguo"<<endl;
	                                     	gotoxy(37,6);cout<<"4.-Rombo"<<endl;
	                                     	gotoxy(19,7);cout<<"5.-Paralelogramo"<<endl;
	                                     	gotoxy(37,7);cout<<"6.-Trapecio"<<endl;
	                                     	gotoxy(19,8);cout<<"7.-Poligono Regular,"<<endl;
	                                     	gotoxy(39,8);cout<<"8.-Circunferencia"<<endl;
	                                     	gotoxy(19,9);cout<<"9.-Circulo"<<endl;
	                                     	gotoxy(19,10);cin>>a;
	 		                                switch(a){                    	
	 			                            case 1:
	 			                            	system("cls");
	 			                            	pintar_limites();
	 			                            	gotoxy(23,4);cout<<"Digite el Lado del cuadrado"<<endl;
	 			                            	gotoxy(23,5);cin>>c;
	 			                                p=4*c;
	 			                                system("cls");
	 			                                pintar_limites();
								 	            gotoxy(23,4);cout<<"El perimtro es :"<<p;
								 	            pintar_limites();
	 			                                break;
	 			                                case 2:
	 			                                	system("cls");
	 			                                	pintar_limites();
	 				                                gotoxy(23,4);cout <<"Rectangulo"<<endl;
	 				                                gotoxy(23,5);cout<<"Digite el BASE(b)  ALTURA(a)"<<endl;
	 				                                gotoxy(23,6);cout<<"Digite el Numero de la Base"<<endl;
	 				                                gotoxy(23,7);cin>>b;
	 				                                system("cls");
	 				                                pintar_limites();
	 				                                gotoxy(23,4);cout<<"digte el numero de la altura"<<endl;
	 				                                gotoxy(23,5);cin>>a;
	 				                                p=2*a+2*b;
	 				                                system("cls");
	 				                                pintar_limites();
	 				                                gotoxy(23,4);cout<<"El perimtro es :"<<p<<endl;
	 				                                pintar_limites();
	 				                                break;
	 				                                case 3:
	 				                                	system("cls");
	 				                                	pintar_limites();
	 				                                	gotoxy(23,4);cout<<"Triangulo"<<endl;
	 					                                gotoxy(23,5);cout<<"Dame la Base(a)";
	 					                                gotoxy(23,6);cin>>a;
	 					                                system("cls");
	 					                                pintar_limites();
	 					                                gotoxy(23,4);cout<<"Dame el Lado 1 (b)";
	 					                                gotoxy(23,5);cin>>lado1;
	 					                                system("cls");
	 					                                pintar_limites();
	 					                                gotoxy(23,4);cout<<"Dame el Lado 2 (c)";
	 					                                gotoxy(23,5);cin>>lado2;
	 					                                p=a+lado1+lado2;
	 					                                system("cls");
	 					                                pintar_limites();
	 					                                gotoxy(23,4);cout<<"El perimtro es :"<<p<<endl;
	 					                                pintar_limites();
	 					                                break;   
	 					                                case 4:
	 					                                	system("cls");
	 					                                	pintar_limites();
	 					                                	gotoxy(23,4);cout<<"Rombo"<<endl;
	 					                                	gotoxy(23,5);cout<<"Digite el Lado del Rombo (a)"<<endl;
	 					                                	gotoxy(23,6);cin>>r;
	 					                                	p=4*r;
	 					                                	system("cls");
	 					                                	pintar_limites();
	 					                                	gotoxy(23,4);cout<<"El perimtro es :"<<p<<endl;
	 					                                	pintar_limites(); 
	 						                                break;
	 						                                case 5:
	 						                                	system("cls");
	 						                                	pintar_limites();
	 						                                	gotoxy(23,4);cout<<"Paralelogramo"<<endl;
	 						                                	gotoxy(23,5);cout<<"Digite el Lado del (a) Paralelogramo"<<endl;
	 							                                gotoxy(23,6);cin>>a;
	 							                                system("cls");
	 							                                pintar_limites();
	 							                                gotoxy(23,4);cout<<"Digite el Lado del (b) Paralelogramo"<<endl;
	 							                                gotoxy(23,5);cin>>b;
	 							                                p=2*a+2*b;
	 							                                system("cls");
	 							                                pintar_limites();
	 							                                gotoxy(23,4);cout<<"El perimtro es :"<<p<<endl;
	 							                                pintar_limites();
	 							                                break;
	 							                                case 6:
	 							                                	system("cls");
	 							                                	pintar_limites();
	 							                                	gotoxy(23,4);cout<<"Trapecio"<<endl;
	 							                                	gotoxy(23,5);cout<<"Digite el Lado del (a) Trapecio"<<endl;
	 								                                gotoxy(23,6);cin>>ladoa;
	 								                                system("cls");
	 								                                pintar_limites();
	 								                                gotoxy(23,4);cout<<"Digite el Lado del (b) Trapecio"<<endl;
	 								                                gotoxy(23,5);cin>>ladob;
	 								                                system("cls");
	 								                                pintar_limites();
	 								                                cout<<"Digite el Lado del (c) Trapecio"<<endl;
	 								                                cin>>ladoc;
	 								                                system("cls");
	 								                                pintar_limites();
	 								                                cout<<"Digite el Lado del (d) Trapecio"<<endl;
	 								                                cin>>ladod;
	 								                                system("cls");
	 								                                pintar_limites();
	 								                                p=ladoa+ladob+ladoc+ladod;
	 								                                gotoxy(23,4);cout<<"El perimtro es :"<<p<<endl;
	 								                                pintar_limites();
	 								                                break;
	 								                                case 7:
	 								                                	system("cls");
	 								                                	pintar_limites();
	 								                                	gotoxy(23,4);cout<<"Poligono Reglar"<<endl;//add
	 								                                	gotoxy(23,5);cout<<"Cuantos Lados tiene el Poligono"<<endl;
	 									                                gotoxy(23,6);cin>>a;
	 									                                system("cls");
	 									                                pintar_limites();
	 									                                gotoxy(23,4);cout<<"Ingrese el Valor del Lado del poligono"<<endl;
	 									                                gotoxy(23,5);cin>>b;
	 									                                p=a*b;
	 									                                system("cls");
	 									                                pintar_limites();
	 									                                gotoxy(23,4);cout<<"El perimtro es :"<<p<<endl;
	 									                                pintar_limites();
	 									                                break;
	 									                                case 8:
	 									                                	system("cls");
	 									                                	pintar_limites();
	 									                                	gotoxy(23,4);cout<<"Circunferencia con Radio"<<endl;
	 									                                	gotoxy(23,5);cout<<"Ingrese el Valor de Radio"<<endl;
	 									                                	gotoxy(23,6);cin>>a;
	 									                                	p=2*pi*a;
	 									                                	system("cls");
	 									                                	pintar_limites();
	 									                                	gotoxy(23,4);cout<<"El perimtro es :"<<p<<endl;
	 										                                break;
											                                    default:
																													
	 												 printf("                 .\"-,.__\n");
				                                     printf("                 `.     `.  ,\n");
				                                     printf("              .--'  .._,'\"-' `.\n");
				                                     printf("             .    .'         `'\n");
				                                     printf("             `.   /          ,'\n");
				                                     printf("               `  '--.   ,-\"'\n");
				                                     printf("                `\"`   |  \\\n");
				                                     printf("                   -. \\, |\n");
				                                     printf("                    `--Y.'      ___.\n");
				                                     printf("                         \\     L._, \\\n");
				                                     printf("               _.,        `.   <  <\\                _\n");
				                                     printf("             ,' '           `, `.   | \\            ( `\n");
				                                     printf("          ../, `.            `  |    .\\`.           \\ \\_\n");
				                                     printf("         ,' ,..  .           _.,'    ||\\l            )  '\".\n");
				                                     printf("        , ,'   \\           ,'.-.`-._,'  |           .  _._`.\n");
				                                     printf("      ,' /      \\ \\        `' ' `--/   | \\          / /   ..\\	\n");
				                                     printf("    .'  /        \\ .         |\__ - _ ,'` `        / /     `.`.\n");
				                                     printf("    |  '          ..         `-...-\"  |  `-'      / /        . `.\n");
				                                     printf("    | /           |L__           |    |          / /          `. `.\n");
				                                     printf("   , /            .   .          |    |         / /             ` `\n");
				                                     printf("  / /          ,. ,`._ `-_       |    |  _   ,-' /               ` \\	\n");
				                                     printf(" / .           \\\"`_/. `-_ \\_,.  ,'    +-' `-'  _,        ..,-.    \`.\n");
				                                     printf(".  '         .-f    ,'   `    '.       \\__.---'     _   .'   '     \\ \\	\n");
				                                     printf("' /          `.'    l     .' /          \\..      ,_|/   `.  ,'`     L`\n");
				                                     printf("|'      _.-""` `.    \\ _,'  `            \\ `.___`.'\"`-.  , |   |    | \\\n");
				                                     printf("||    ,'      `. `.   '       _,...._        `  |    `/ '  |   '     .|\n");
				                                     printf("||  ,'          `. ;.,.---' ,'       `.   `.. `-'  .-' /_ .'    ;_   ||\n");
				                                     printf("|| '              V      / /           `   | `   ,'   ,' '.    !  `. ||\n");
				                                     printf("||/            _,-------7 '              . |  `-'    l         /    `||\n");
				                                     printf(". |          ,' .-   ,' ||               | .-.        `.      .'     ||\n");
				                                     printf(" `'        ,'    `\".'    |               |    `.        '. -.'       `'\n");
				                                     printf("          /      ,'      |               |,'    \\-.._,.'/'\n");
				                                     printf("          .     /        .               .       \\    .''\n");
				                                     printf("        .`.    |         `.             /         :_,'.'\n");
				                                     printf("          \ `...\   _     ,'-.        .'         /_.-'\n");
				                                     printf("           `-.__ `,  `'   .  _.>----''.  _  __  / \n");
				                                     printf("                .'        /\"'          |  \"'   '_ \n");
				                                     printf("               /_|.-'\\ ,\".             '.'`__'-( \\ \n");
				                                     printf("                 / ,\"'\"\\,'               `/  `-.|\" mh   \n");
				                                     printf("\n");
			 	                                     printf("\n");
				                                     printf("\n");
				                                     printf("\n");
				                                     printf("\n");
				                                     printf("__________.__                    _____                .__     _________\n");
				                                     printf("\\______   \\  | _____  ___.__.   /  _  \\    _________  |__| ___\\_____   \\\n");
				                                     printf(" |     ___/  | \\__  \\<   |  |  /  /_\\  \\  / ___\\__  \\ |  |/    \\ /   __/\n");
				                                     printf(" |    |   |  |__/ __ \\\\___  | /    |    \\/ /_/  > __ \\|  |   |  \\   |\n");
			                                    	 printf(" |____|   |____(____  / ____| \\____|__  /\\___  (____  /__|___|  /___|\n");
				                                     printf("                    \\/\\/              \\//_____/     \\/        \\/<___>\\n");
													 main();		
			                                         }
			                                             cin.get();
			                                             cout << "\n Desea salir? (1 - Si, 2 - No)" << endl; 
			                                             cin >> a;  
			                                             switch(a){
			                                         	 case '1':
			                                         	 	return 0;
			                                         		break;
			                                         		case '2': 
			                                         		    cout << "-------------------------------" << endl;
			                                         		    cout << "-------------------------------" << endl;
			                                         		    main();
			                                         		    break;			                                         	
													             }
																 case 2:
																 	system("cls");
																 	pintar_limites();
																 	gotoxy(14,4);cout<<"Que figura desea sacar el Area  *poligonos regulares*"<<endl;
																 	gotoxy(19,5);;cout<<"1.-Cuadredo,"<<endl;
																 	gotoxy(37,5);cout<<"2.-Rectangulo"<<endl;
																 	gotoxy(19,6);cout<<"3.-Trianguo,"<<endl;
																 	gotoxy(37,6);cout<<"4.-Rombo"<<endl;
																 	gotoxy(19,7);cout<<"5.-Paralelogramo,"<<endl;
																 	gotoxy(37,7);cout<<"6.-Trapecio"<<endl;
																 	gotoxy(19,8);cout<<"7.-Poligono Regular,"<<endl;
																 	gotoxy(39,8);cout<<"8.-Circunferencia"<<endl;
																 	gotoxy(19,9);cout<<"9.-Circulo"<<endl;
																 	gotoxy(19,10);cin >> a;
																 	pintar_limites();
																 	switch(a){
																 		case 1:
																 			system("cls");
																 			pintar_limites();
																 			gotoxy(23,4);cout<<"Area de Un Cuadrado"<<endl;
																 			gotoxy(23,5);cout<<"Digite el Lado del cuadrado"<<endl;
																 			gotoxy(23,6);cin>>a;
																 			area=a*a;
																 			system("cls");
																 			pintar_limites();
																 			gotoxy(23,4);cout<<"El AREA es :"<<area<<endl;
																 			pintar_limites();
																 			break ;
																 			case 2:
																 				system("cls");
																 				pintar_limites();
																 				gotoxy(23,4);cout<<"Area de Un Rectangulo"<<endl;
																 				gotoxy(23,5);cout<<"Digite el BASE(b)  ALTURA(a)"<<endl;
																 				gotoxy(23,6);cout<<"Digite el Numero de la Base"<<endl;
																 				gotoxy(23,7);cin>>b;
																 				system("cls");
																 				pintar_limites();
																 				gotoxy(23,4);cout <<"digte el numero de la altura"<<endl;
																 				gotoxy(23,5);cin>>a;
																 				area=2*a+2*b;
																 				system("cls");
																 				pintar_limites();
																 				gotoxy(23,4);cout<<"El AREA es :"<<area<<endl;
																 				pintar_limites();
																 				
																 				break;
																 				case 3:																				 
																				 	cout<<"El Area De Un Triangulo"<<endl;
																				 	cout<<"Dame la Base(a)"<<endl;
																				 	cin>>a;
																				 	cout<<"Dame la altura (h)"<<endl;
																				 	cin>>h;
																				 	area=a*h/2;
																				 	cout<<"El Area es :"<<area<<endl;
																				 	break;
																				 	case 4:
																				 		cout<<"El Area De Un Rombo"<<endl;
																				 		cout<<"Dame El Lado Menor (d)"<<endl;
																				 		cin>>menord;
																				 		cout<<"Dame El Lado Mayor (D)"<<endl;
																				 		cin>>mayorD;
																				 		area=menord*mayorD/2;
																				 		cout<<"El Area es :"<<area<<endl;
																				 		break;
																				 		case 5:
																				 			cout<<"El Area De Un Paralelogramo"<<endl;
																				 			cout<<"Dame El Lado (a)"<<endl;
																				 			cin>>a;
																				 			cout<<"Dame El Lado (h)"<<endl;
																				 			cin>>h;
																				 			area=a*h;
																				 			cout<<"El Area es :"<<area<<endl;
																							 break;
																							 case 6:
																							     cout<<"El Area De Un Trapecio"<<endl;
																							     cout<<"Dame El Lado (a)"<<endl;
																							     cin>>a;
																							     cout<<"Dame El Lado (b)"<<endl;
																							     cin>>b;
																							     cout<<"Dame La Altura (h)"<<endl;
																							     cin>>h;
																							     area=(a+b/2)*h;
																							     cout<<"El Area es :"<<area<<endl;
																							     break;
																							     case 7:
																							 	cout<<"El Area De Un Poligono Reglar "<<endl;
																							 	cout<<"Tienes el Perimetro"<<endl;
																							 	cout<<"\n1.-SI\n2.-NO"<<endl;
																							 	cin>>a;
																							 	switch(a){
																							 		case 1:
																							 			cout<<"Dame el Perimetro"<<endl;
																							 			cin>>perimetro;
																							 			cout<<"Dame la Apotema"<<endl;
																							 			cin>>apotema;
																							 			area=perimetro*apotema/2;
																							 			cout<<"El Area es :"<<area<<endl;
																							 			break;
																							 			case 2:
																							 				cout <<"Ingrese la Cantidad de Lados Que Tienes  su Poligono Regular "<<endl;
																							 				cin>>a;
																							 				cout<<"Ingrese el Valor del Lado del poligono"<<endl;
																							 				cin>>b;
																							 				cout<<"Dame la Apotema"<<endl;
																							 				cin>>apotema;
																							 				area=a*b*apotema;
																							 				cout<<"El Area es :"<<area<<endl;
																							 				break;
																							 				default:
																							 					cout << "Operacion incorrecta. Vuelva a intentarlo... n" << endl; 
                                                                                                                 cout << "********************************************" << endl; 
                                                                                                                 cout << "******************************************** n" << endl; 
                                                                                                                 main();	
																							                     }
																												 case 8:
																												 cout<<"El Area De Un Circulo  "<<endl;
																												 cout<<"1.-¿Cuentas con el Dimetro? o 2.-¿Con el Radio?"<<endl;
																												 cout<<"Presiona 1 si Cuantas Con El Diametro , Presiona 2 Si Cunetas Radio"<<endl;
																												 cin>>a;
																												 switch(a){
																												 	case 1:
																												 		cout<<"El Area de un circulo Dado el Diametro"<<endl;
																												 		cout<<"Ingrese El Valor del Diamtro"<<endl;
																												 		cin>>diametro;
																												 		area=pi*diametro/4;
																												 		cout <<"El Area es:"<<area<<endl;
																												 		break;
																												 		case 2:
																												 			cout<<"Ingrese El Valor del Radio"<<endl;
																												 			cin>>radio;
																												 			area2=pi*pow(radio,2);
																												 			cout<<"El Area es:"<<area2<<endl;
																												 			break;
																												 			default:
																												 				cout<<" no usuario pendejo solo puede presionar 1 o 2 como opciones validas....n"<<endl;
																												 				cout<<"------------------------------------------------------------------"<<endl;
																												 				cout<<"T_T    T_T      T_T    T_T     T_T   T_T     T_T     T_T   T_T   T_T"<<endl;
																												 				main();
																												                         }											 																									 
																	                                                                         }		
	                                                                                                                                             return 0;														  													 
	                                                                                                                                                         }
																																					    	     break;
																																					    	         case 14:
																																					    	         	
																																					    	         	
																																				                        break; 
                                                                                                         	                                                            default: 
                                                                                                                                                                         cout << "Operacion incorrecta. Vuelva a intentarlo... n" << endl; 
                                                                                                                                                                         cout << "********************************************" << endl; 
                                                                                                                                                                         cout << "******************************************** n" << endl; 
                                                                                                                                                                         main(); 
                                                                                                         	                                                         }
                                                                                                         	                                                                 cin.get(); 
                                                                                                                                                                             cout << "\n Desea salir? (1 - Si, 2 - No)" << endl; 
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













































































