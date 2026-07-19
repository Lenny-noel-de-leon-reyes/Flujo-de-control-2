# Flujo-de-control-2


#include <iostream>
#include <string>


using namespace std;

int main() {
    int n;
    string nombre;
    float n1, n2, n3, n4, promedio;

    cout << "\t Calificacion de estudiantes" << endl;
    cout << "Ingrese la cantidad de estudiantes: ";
    cin >> n;


    cout << "\n" "\tNombre" "\t N1" "\tN2" "\tN3" "\tN4"
        "\tPromedio" "\tEstado" << endl;
    cout << string(70, '-') << endl;


    for (int i = 0; i < n; i++) {
        cout << "Ingrese nombre del estudiante: ";
        cin >> nombre;
        cout << "Ingrese las 4 notas: ";
        cin >> n1 >> n2 >> n3 >> n4;

        promedio = (n1 + n2 + n3 + n4) / 4.0;

        cout << "\tnombre  n1 \tn2 \tn3 \tn4\tPromedio  \Estado " << endl;
        cout << "\t" << nombre
            << "\t" << n1 << "\t" << n2 << "\t" << n3 << "\t" << n4
            << "\t" << promedio << "\t";

        if (promedio >= 70) {
            cout << "Aprobo" << endl;
        }
        else {
            cout << "Reprobo" << endl;
        }
    }

    return 0;
}
