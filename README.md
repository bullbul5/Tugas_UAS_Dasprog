# Tugas_UAS_Dasprog
# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Nabila Lailatanzila
<br>NIM		:	1227050100
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
<br>Array 2 dimensi adalah sebuatan array yang memiliki lebih dari satu bentuk index array. Jika pada array 1 dimensi hanya terdiri dari 1 baris ataupun kolom, di array 2 dimensi mempunyai lebih dari satu bentuk baris maupun kolom. Pada artikel kali ini, saya akan menampilkan suatu code program mengenai array 2 dimensi dimana program tersebut menampilkan hasil transpose dari suatu matriks.
Berikut adalan code programnya:
<br>Contoh Array 2 dimensi
## Source Code
 <br> #include <iostream>
 <br> using namespace std;

 <br> int main(){
   <br> int i, j, m, n, matriks[10][10], transpose[10][10];

    cout << "Masukkan jumlah baris matriks: ";
    cin >> m;
    cout << "Masukkan jumlah kolom matriks: ";
    cin >> n;

    cout << "Masukkan elemen matriks\n";
    for (i = 0; i < m; i++){
      for (j = 0; j < n; j++){
        cin  >> matriks[i][j];
      }
    }  

    for (i = 0; i < m; i++){
      for (j = 0; j < n; j++){
        transpose[j][i] = matriks[i][j];
      }
    }

    cout << "Hasil Transpose Matriks: \n";
    for (i = 0; i < n; i++){
      for (j = 0; j < m; j++){
        cout << transpose[i][j] << "\t";
      }
      cout << endl;
    }
    return 0;
  }
<br>#Program 2
  <br>#include <iostream>
  <br>using namespace std;

  <br>int main(){
    cout<<"NABILA LAILATANZILA"<<endl;
    cout<<"1227050100"<<endl;

    int i, j, baris, kolom, matriks[10][10], transpose[10][10];

    cout<<endl;
    cout << "Masukkan jumlah baris matriks: ";
    cin >> baris;
    cout << "Masukkan jumlah kolom matriks: ";
    cin >> kolom;

    cout <<endl<< "Masukkan elemen matriks\n";
    for (i = 0; i < baris; i++){
      for (j = 0; j < kolom; j++){
      cout<<"Baris ke - "<<j+1<<" Kolom ke - "<<i+1<<endl;
        cin  >> matriks[i][j];
      }
    }  
  cout<<endl<<"Nilai Matriks yaitu: "<<endl;
    for (i = 0; i < baris; i++){
      for (j = 0; j < kolom; j++){

        cout<<matriks[i][j]<<"\t";
      }
      cout<<endl;
    }

    for (i = 0; i < baris; i++) {
      for (j = 0; j < kolom; j++) {
        if (matriks[i][j] % 3 == 0 && matriks[i][j] % 5 == 0 && matriks[i][j] % 7 == 0) {
          cout <<endl<< "Bilangan yang habis dibagi 3, 5, 7 adalah : " << matriks[i][j] << endl;
        } 
      }
    }
  return 0;
  }


## Output
<br>#program 1
<br>Masukkan jumlah baris matriks: 2
<br>Masukkan jumlah kolom matriks: 2
<br>Masukkan elemen matriks
<br>2
<br>3
<br>4
<br>5
<br>Hasil Transpose Matriks:
<br>2       4
<br>3       5

<br>#program 2
<br>NABILA LAILATANZILA
<br>1227050100

<br>Masukkan jumlah baris matriks: 2
<br>Masukkan jumlah kolom matriks: 2

<br>Masukkan elemen matriks
<br>Baris ke - 1 Kolom ke - 1
<br>1
<br>Baris ke - 2 Kolom ke - 1
<br>2
<br>Baris ke - 1 Kolom ke - 2
<br>105
<br>Baris ke - 2 Kolom ke - 2
<br>1

<br>Nilai Matriks yaitu:
<br>1       2
<br>105     1

<br>Bilangan yang habis dibagi 3, 5, 7 adalah : 105
