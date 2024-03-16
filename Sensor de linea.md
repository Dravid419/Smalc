int sensorLinea = 7;
bool sensorDeLineaEstado = false;

void setup() {
pinMode(7,INPUT);
Serial.begin(9600);
}

void loop() {
Serial.println(getSensorDeLinea());
}

bool getSensorDeLinea(){
  return digitalRead(sensorLinea); //Pero pq usamos funciones?
}
