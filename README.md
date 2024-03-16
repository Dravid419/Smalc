int sensorLinea = 7;
bool sensorDeLineaEstado = false;

void setup() {
pinMode(7,INPUT);
Serial.begin(9600);
}

void loop() {
  // put your main code here, to run repeatedly:
Serial.println(getSensorDeLinea());
}

//Crear una funcion para llamar a la lectura del sensor y que me devuelva su valor en donde le indique
bool getSensorDeLinea(){
  return digitalRead(sensorLinea); //Pero pq usamos funciones?
}
