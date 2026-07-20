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
    for (int i = 0; i < n; i++) {
        cout << "Ingrese nombre del estudiante: ";
        cin >> nombre;
        cout << "Ingrese las 4 notas: ";
        cin >> n1 >> n2 >> n3 >> n4;

        promedio = (n1 + n2 + n3 + n4) / 4.0;

        
    cout << "\n" "\tNombre" "\t Nota1" "\tNota2" "\tNota3" "\tNota4"
        "\tPromedio" "\tEstado" << endl;
    cout << string(70, '-') << endl;
        cout << "\t" << nombre
            << "\t" << n1 << "\t" << n2 << "\t" << n3 << "\t" << n4
            << "\t" << promedio << "\t";

        if (promedio >= 70) {
            cout << "\tAprobo" << endl;
        }
        else {
            cout << "\tReprobo" << endl;
        }

    }

    return 0;
}
