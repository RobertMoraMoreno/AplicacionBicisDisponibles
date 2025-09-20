# 🚲 AplicaciónBicis

Aplicación Android que muestra información en tiempo real sobre las estaciones de bicicletas públicas en Valencia.  
Permite consultar la dirección, número de bicicletas disponibles, número de anclajes libres y la ubicación en el mapa.

---

## 🎯 Objetivo
El objetivo de este proyecto es desarrollar una app funcional que integre tecnologías modernas de Android y que permita:
- Visualizar estaciones de bicicletas.
- Consultar bicis y anclajes disponibles.
- Ubicar las estaciones en un mapa interactivo.

---

## 🛠️ Tecnologías utilizadas
- **Lenguaje:** Kotlin  
- **IDE:** Android Studio  
- **Arquitectura:** MVVM (Model - ViewModel - UI)  
- **UI:** Jetpack Compose + Material 3  
- **Navegación:** Navigation Compose  
- **Mapas:** Google Maps API (Play Services Maps)  
- **Asincronía:** Coroutines + Flow  

---

## 📂 Estructura del proyecto
- `MainActivity.kt` → Punto de entrada, gestiona la navegación.  
- `StationsViewModel.kt` → Carga y gestiona los datos desde CSV.  
- `Station.kt` → Data class que representa una estación (dirección, bicis, anclajes, coordenadas).  
- **Pantallas**:  
  - `ListScreen` → Lista de estaciones.  
  - `DetailScreen` → Mapa con la estación seleccionada.  
- `assets/aplicacionbicis.csv` → Datos de las estaciones.  

---

## 📊 Funcionamiento
1. **Carga de datos**: Se leen desde `aplicacionbicis.csv`.  
2. **Pantalla principal**: Lista todas las estaciones con bicis y anclajes.  
3. **Pantalla de detalle**: Muestra en Google Maps la ubicación de la estación seleccionada con su información básica.  

---

## 📌 Puntos clave
- Interfaz moderna con **Jetpack Compose**.  
- Navegación fluida entre lista y mapa.  
- Uso de **Coroutines + Flow** para carga asíncrona de datos.  
- Integración con **Google Maps API** para localización real.  

---

## 🚲 Conclusión
AplicacionBicis es un prototipo funcional que:
- Integra librerías modernas de Android.  
- Demuestra cómo trabajar con datos externos (CSV).  
- Presenta una UI práctica e interactiva para el usuario.  

---

👨‍🎓 **Autor**: Roberto Mora Moreno  
📘 **Curso**: 2º DAM
