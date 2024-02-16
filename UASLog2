#include <iostream>
#include <string>
using namespace std;

string sensorKata(string kalimat, string kata_yang_disensor, char karakter_untuk_sensor) {
    string hasil = "";
    size_t pos = 0;
    while ((pos = kalimat.find(kata_yang_disensor, pos)) != string::npos) {
        kalimat.replace(pos, kata_yang_disensor.length(), kata_yang_disensor.length(), karakter_untuk_sensor);
        pos += kata_yang_disensor.length();
    }
    return kalimat;
}

int main() {
    string kalimat = "Kelakuan anak itu sangat bodoh sekali";
    string kata_yang_disensor = "bodoh";
    char karakter_untuk_sensor = '$';

    string hasil_sensor = sensorKata(kalimat, kata_yang_disensor, karakter_untuk_sensor);

    cout << "Output: " << hasil_sensor << endl;

    return 0;
}
