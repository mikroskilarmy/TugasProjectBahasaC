# TugasProjectBahasaC

TUGAS I MODIFIKASI SOAL MODUL : 

#include<stdio.h>

int main(){
    int angka1, angka2;

    printf("Demo Struktur Kondisi\n");
    printf("=====================\n");
    printf("Masukkan bilangan asli 1: ");
    scanf("%d", &angka1);
    if (!(angka1 > 0 && angka1 <= 9)) {
    printf("Harap Masukkan Bilangan asli"); return 0;
    }

    printf("Masukkan bilangan asli 2: ");
    scanf("%d", &angka2);
    if (!(angka2 > 0 && angka2 < 10)) {
        printf("Harap Masukkan Bilangan asli");
        return 0;
    }

    int pilihan;
    printf("\n\n Jenis operator\n");
    printf("--------------------\n");
    printf(" 1. Contoh Operator Aritmatika\n");
    printf(" 2. Contoh Operator Relasional\n");
    printf(" 3. Contoh Operator Logical \n");
    printf(" Pilihan [1-3]: ");
    scanf("%d", &pilihan);
    if (pilihan == 1)
    {
        printf("\n Contoh Operator Aritmatika\n");
        printf(" Penjumlahan \t: %d + %d = %d \n", angka1,angka2, angka1 + angka2);
        printf(" Perkalian \t: %d * %d = %d \n",angka1,angka2,angka1 * angka2);
    }
    else if (pilihan == 2)
    {
        printf("\n Contoh Operator Relasional\n");
        printf(" Persamaan \t: %d == %d = ",angka1, angka2);
        if (angka1 == angka2)
            printf("TRUE");
        else
            printf("FALSE");

        printf("\n Pertidaksamaan\t: %d != %d = ",angka1,angka2);
        if (angka1 != angka2)
            printf("TRUE");
        else
            printf("FALSE");
    }
    else if (pilihan == 3)
    {
        printf("\n\n Contoh Operator Logical\n");
        printf(" Logika AND \t: %d && %d = %d\n",angka1,angka2, angka1 && angka2);
        printf(" Logika OR \t: %d || %d = %d\n",angka1,angka2,angka1 || angka2);
    }
    else
        printf("\n Harap Masukkan Bilangan Asli ");



    getch();
    return 0;
}



TUGAS II BUAT SOAL SENDIRI :


#include<stdlib.h>
#include<stdio.h>

int main()
{
    int menu,nasi=3000,ayam_bakar=7000,tahu=1000,tempe=1000,lalap=2000,air_mineral=3000,sayur_asem=2000,gepuk=5000,air_hangat=1000,jumlah_pesanan,total,pajak,total_akhir;

    printf("================Selamat Datang Di Mikro Resto=======================\n\n");
    printf("PAKET MAKANAN\n");
    printf("===============\n");
    printf("Paket 1\n");
    printf("Paket 2\n");
    printf("Paket 3\n");
    printf("Silakan pilih paket menu yang ada :");
    scanf("%d", &menu);
    printf("Banyaknya pesanan :");
    scanf("%d", &jumlah_pesanan);
    printf("\n");

    switch (menu){
        case 1:
        printf("Paket 1\n");
        printf("Nasi :%d",nasi);
        printf("\nAyam Bakar : %d",ayam_bakar);
        printf("\nTahu :%d",tahu);
        printf("\nTempe :%d",tempe);
        printf("\nLalapan :%d",lalap);
        printf("\nAir Mineral: %d",air_mineral);
        printf("\nJumlah pesanan :%d paket",jumlah_pesanan);
        total= (nasi+ayam_bakar+tahu+tempe+lalap+air_mineral)*jumlah_pesanan;
        pajak=(total)*10/100;
        total_akhir=total+pajak;
        printf("\n");
        printf("\nTotal,paket1 * %d:%d",jumlah_pesanan,total);
        printf("\nPajak 10 persen : %d",pajak);
        printf("\nJadi,total yang harus anda bayar:%d",total_akhir);
        printf("\n");
        break;
        case 2 :
            printf("Paket 2\n");
            printf("Nasi :%d",nasi);
            printf("\nAyam Bakar :%d",ayam_bakar);
            printf("\nSayur Asem :%d",sayur_asem);
            printf("\nTahu :%d",tahu);
            printf("\nTempe:%d",tempe);
            printf("\nLalapan:%d",lalap);
            printf("\nAir Mineral:%d",air_mineral);
            printf("\nJumlah pesanan : %d paket",jumlah_pesanan);
            total=(nasi+ayam_bakar+sayur_asem+tahu+tempe+lalap+air_mineral)*jumlah_pesanan;
            pajak=(total)*10/100;
            total_akhir=total+pajak;
            printf("\n");
            printf("\nTotal, paket 2 * %d: %d",jumlah_pesanan,total);
            printf("\nPajak 10 persen : %d",pajak);
            printf("\nJadi,total yang harus anda bayar :%d",total_akhir);
            printf("\n");
            break;
        case 3:
            printf("Paket 1\n");
            printf("Nasi : %d",nasi);
            printf("\nGepuk : %d",gepuk);
            printf("\nTahu : %d",tahu);
            printf("\nTempe",tempe);
            printf("\nLalapan : %d",lalap);
            printf("\nAir Hangat : %d",air_hangat);
            printf("\nJumlah pesanan :%d paket",jumlah_pesanan);
            total=(nasi+gepuk+tahu+tempe+lalap+air_hangat)*jumlah_pesanan;
            pajak=(total)*10/100;
            total_akhir=total+pajak;
            printf("\n");
            printf("\nTotal, paket 2 * %d :%d",jumlah_pesanan,total);
            printf("\nPajak 10 : %d",pajak);
            printf("\Jadi,total yang harus anda bayar:%d",total_akhir);
            printf("\n");
            break;

            printf("Maaf, Paket yang anda pilih tidak ada didalam menu!!Silahkan Coba lagi :)\n");

        system("pause");
        return 0;
}

}


