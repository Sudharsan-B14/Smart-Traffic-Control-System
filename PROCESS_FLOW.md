```mermaid
graph TD;
    A(Camera Captures Video) --> B(YOLO Model for Vehicle Detection);
    B --> C(Data Sent to Cloud - Google Colab);
    C --> D{Custom Algorithm: Vehicle Count, Density, Lane Selection};
    D --> E(Lane Data Sent via MQTT);
    E --> F(ESP32 Modifies Traffic Signals);
    F --> G(ESP8266 Alerts Lane with Alarm);
    G --> H(Traffic Flow Optimized 🚦);
