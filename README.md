# tugas-3
//Nama : Reina Puteri Ramadhani
//NIM : 18320039

#include <iostream>

using namespace std;

int main ()
{
    cout<<"Program Menentukan Jenis File dari Hex Signature"<<endl;

    //deklarasi jenis file

    int gif[6]={47,49,46,38,37,61};
    int pdf[5]={25,50,44,46,2};
    int mp3[3]={49,44,33};
    int mp4[8]={66,74,79,70,69,73,6,6};
    int png[8]={89,50,4,4,0,0,1,0};
    int psd[4]={38,42,50,53};

    int n;
    int i;
    n = 0;

    //input jumlah nomor
    cout<<"Masukkan Banyaknya Nomor : "; cin>>n;
    int data[n];
    for (int i=0;i<n;i++){
        cout<<"Masukkan nomor ke-"<<i+1<<" : ";
        cin>>data[i];
    }
    if (data[i]==gif[6]){
        cout<<"File ini berformat gif.";
    }
    else if (data[i]==pdf[5]){
        cout<<"File ini berformat pdf.";
    }
    else if (data[i]==mp3[3]){
        cout<<"File ini berformat mp3.";
    }
    else if (data[i]==mp4[8]){
        cout<<"File ini berformat mp4.";
    }
    else if (data[i]==png[8]){
        cout<<"File ini berformat png.";
    }
    else if (data[i]==psd[4]){
        cout<<"File ini berformat psd.";
    }
    else {
        cout<<"Nomor yang dimasukkan tidak sesuai dengan format file manapun.";
    }
    return 0;
}
