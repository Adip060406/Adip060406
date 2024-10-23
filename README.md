#include <iostream>
using namespace std;

int main() {
    // Deklarasi variabel
    double totalPembelian, potongan = 0.0, totalBayar;

    // Meminta input total pembelian dari pengguna
    cout << "Masukkan total pembelian (Rp): ";
    cin >> totalPembelian;

    // Menentukan besarnya potongan berdasarkan total pembelian
    if (totalPembelian >= 50000) {
        potongan = 0.2 * totalPembelian;
    }

    // Menghitung total yang harus dibayar setelah potongan
    totalBayar = totalPembelian - potongan;

    // Menampilkan hasil
    cout << "Total pembelian: Rp" << totalPembelian << endl;
    cout << "Potongan: Rp" << potongan << endl;
    cout << "Total yang harus dibayar: Rp" << totalBayar << endl;

    return 0;
}
