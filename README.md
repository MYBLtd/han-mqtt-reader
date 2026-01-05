# han-mqtt-reader

Doel: - Stabiele uitlezing van IDIS / DLMS HAN-poort (E.ON Zweden) 
  - ESP32 + isolated RS-485 (DFRobot DFR0845)
  - MQTT → Home Assistant (statisch, geen discovery)  Architectuur: Meter → RS-485 → ESP32 → MQTT → HA

Belangrijke keuzes: 
  - Geen voeding uit HAN - Geen MQTT discovery
  - Platte JSON payloads - Availability via LWT
