#include <iostream>
#include <iomanip>
#include <string>
using namespace std;

// Definisikan struct Mahasiswa
struct Mahasiswa {
    string NIM;
    string NAMA;
    double NILAI_PEMROGRAMAN;
};

int main() {
    const int JUMLAH_MAHASISWA = 10;
    Mahasiswa data_mahasiswa[JUMLAH_MAHASISWA];

    // Input data mahasiswa
    for (int i = 0; i < JUMLAH_MAHASISWA; ++i) {
        cout << "Masukkan data untuk mahasiswa ke-" << i+1 << ":" << endl;
        cout << "NIM: ";
        cin >> data_mahasiswa[i].NIM;
        cout << "Nama: ";
        cin.ignore();
        getline(cin, data_mahasiswa[i].NAMA);
        cout << "Nilai Pemrograman: ";
        cin >> data_mahasiswa[i].NILAI_PEMROGRAMAN;
        cout << endl;
    }

    // Hitung nilai rata-rata
    double total_nilai = 0;
    for (int i = 0; i < JUMLAH_MAHASISWA; ++i) {
        total_nilai += data_mahasiswa[i].NILAI_PEMROGRAMAN;
    }
    double nilai_rata_rata = total_nilai / JUMLAH_MAHASISWA;

    // Output hasil
    cout << "Data Mahasiswa:" << endl;
    cout << "-------------------------------------------------------------" << endl;
    cout << setw(10) << "NIM" << setw(20) << "NAMA" << setw(20) << "NILAI_PEMROGRAMAN" << endl;
    cout << "-------------------------------------------------------------" << endl;
    for (int i = 0; i < JUMLAH_MAHASISWA; ++i) {
        cout << setw(10) << data_mahasiswa[i].NIM << setw(20) << data_mahasiswa[i].NAMA << setw(20) << fixed << setprecision(2) << data_mahasiswa[i].NILAI_PEMROGRAMAN << endl;
    }
    cout << "-------------------------------------------------------------" << endl;
    cout << "Nilai rata-rata: " << fixed << setprecision(2) << nilai_rata_rata << endl;

    return 0;
}
