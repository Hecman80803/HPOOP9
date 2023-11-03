@startuml
scale 3

abstract class MediosTransporte{
    
}

class TransporteAcuatico{
    -velocidad: int
    -capacidad: String
    +aumentoCapacidad():void
}

class Barco{
    -puertoOrigen: String
    -puertoDestino: String
    +abordarPasajeros():void
}

MediosTransporte <|-- TransporteAcuatico
TransporteAcuatico <|-- Barco : interfaz
@enduml