# Ujian Akhir Semester
<br> Mata Kuliah	: Dasar Pemrograman
<br> Nama		: Nazwa Hemalia Putri
<br> Jurusan		: [Teknik Informatika]
(http://if.uinsgd.ac./) [UIN Sunan Gunung Djati Bandung] (https://uinsgd.ac.id/)

## Deskripsi Umum
Program ini dibuat untuk memenuhi Ujian AKhir Semester Mata Kuliah Dasar Pemrograman. Dalam Program ini digunakan fungsi array dan pengulangan for.
program pertama menginputkan nilai baris dan kolom lalu hasil nilai baris dan kolom dibalik dari kolom menjadi baris. kemudian program yang kedua untuk
mencari bilangan yang habis dibagi 3, 5 dan 7 dari hasil inputan program pertama.

## Source Code
```
#include<iostream>
using namespace std;

int main (){
	
	cout << " ==============================================\n";
	cout << " || Nama\t: Nazwa Hemalia Putri        ||\n";
	cout << " || NIM\t\t: 1227050103                 ||\n";
	cout << " || Kelas\t: IF-1C                      ||\n";
	cout << " ==============================================\n";
	
	int kolom, baris, x[50][50], matriks;
		cout << " \n INPUTKAN BARIS\t\t : ";
		cin >> baris;
		cout << " INPUTKAN KOLOM\t\t : ";
		cin >> kolom;
		
		//Soal no 1
		//untuk menginput nilai baris dan kolom
		cout << " \n 1. Input Nilai baris dan kolom lalu dibalik " << endl;
		cout << endl;
		for ( int i=1; i<=baris; i++){
			for ( int j=1; j<=kolom; j++){	
			cout << " Baris ke  " << i <<" Kolom ke  "<<j<< "  : ";
			cin >> x[i][j];
			}
		cout<<endl;
		}
			
		//Output Hasil Matriksnya
		cout << " HASIL MATRIKSNYA SEBAGAI BERIKUT : \n";
		for ( int i=1; i<=baris; i++){
			for ( int j=1; j<=kolom; j++){	
			cout << " "  << x [i][j] << " " ;
			}
		cout<<endl;
		}
		cout << endl;
		//Output Hasil matrik dibalik kolom jadi baris
		cout << " HASIL JIKA BARIS DAN KOLOM DIBALIK SEBAGAI BERIKUT :\n";
		for ( int i=1; i<=kolom; i++){
			for ( int j=1; j<=baris; j++){	
			cout << " " << x [j] [i];
			}
		cout << endl ;
		}
		
		cout << " \n=======================================================\n" << endl;
		//soal no 2	
		//untuk print yang habis dibagi 3,5 sama 7
		cout << " 2. BILANGAN YANG HABIS  DIBAGI 3, 5, 7 SEBAGAI BERIKUT :\n " << endl;
		 for (int i = 1; i <= baris; i++) {
		for (int j = 1; j <= kolom; j++) {
			if (x[i][j] % 3 == 0 && x[i][j] % 5 == 0 && x[i][j] % 7 == 0){
				cout << " Habis dibagi 3, 5, dan 7\t : " << x[i][j] << endl;
			}
			else if (x[i][j] % 5 == 0 && x[i][j] % 7 == 0){
				cout << " Habis dibagi 5, dan 7\t\t : " << x[i][j] << endl;
			}
			else if ( x[i][j] % 7 == 0) {
				cout <<  " Habis dibagi 7\t\t\t : " << x[i][j] << endl;
			} 
		}
	}
}		
```
## Output

<br>==============================================
 <br>|| Nama        : Nazwa Hemalia Putri        ||
 <br>|| NIM         : 1227050103                 ||
 <br>|| Kelas       : IF-1C                      ||
 <br>==============================================

 <br>INPUTKAN BARIS          : 2
 <br>INPUTKAN KOLOM          : 2

 <br>1. Input Nilai baris dan kolom lalu dibalik

<br>Baris ke  1 Kolom ke  1  : 105
 <br>Baris ke  1 Kolom ke  2  : 7

 <br>Baris ke  2 Kolom ke  1  : 105
 <br>Baris ke  2 Kolom ke  2  : 100

 <br>HASIL MATRIKSNYA SEBAGAI BERIKUT :
 <br>105  7
 <br>105  100

 <br>HASIL JIKA BARIS DAN KOLOM DIBALIK SEBAGAI BERIKUT :
 <br>105 105
 <br>7 100

<br>=======================================================

 <br>2. BILANGAN YANG HABIS  DIBAGI 3, 5, 7 SEBAGAI BERIKUT :

 <br>Habis dibagi 3, 5, dan 7        : 105
 <br>Habis dibagi 7                  : 7
 <br>Habis dibagi 3, 5, dan 7        : 105

<br>--------------------------------
