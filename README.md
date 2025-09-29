# 📱 AplicaciónBicis

## 🎯 Objetivo
Aplicación Android que permite consultar información sobre **estaciones de bicicletas públicas en Valencia**.  

La app permite:  
- Ver la **dirección** de cada estación.  
- Consultar el **número de bicicletas disponibles**.  
- Consultar el **número de anclajes libres**.  
- Localizar la estación en un **mapa interactivo**.  

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

## 📂 Estructura principal del proyecto
- **MainActivity.kt** → Punto de entrada, gestiona la navegación entre pantallas.  
- **StationsViewModel.kt** → Carga y gestiona los datos de las estaciones desde un CSV.  
- **Station.kt** → Data class que representa una estación (dirección, bicis, anclajes, lat, lon).  
- **Pantallas:**  
  - **ListScreen** → Lista de estaciones.  
  - **DetailScreen** → Muestra un mapa con la estación seleccionada.  
- **assets/aplicacionbicis.csv** → Archivo con los datos de las estaciones.  

---

## 📊 Funcionamiento
1. **Carga de datos**  
   - Se lee el archivo `aplicacionbicis.csv` desde la carpeta `assets/`.  
   - Se procesan las filas para obtener dirección, bicis, anclajes y coordenadas.  

2. **Pantalla principal (Lista)**  
   - Muestra todas las estaciones con su dirección y número de bicis/anclajes.  
   - **Filtros con Switches:**  
     - Bicis disponibles (activado por defecto)  
     - Espacios disponibles (activado por defecto)  
   - Al pulsar una estación → Navega a la pantalla de detalle.  

3. **Pantalla de detalle (Mapa)**  
   - Muestra la estación seleccionada en Google Maps con su ubicación.  
   - Información básica de la estación.  

---

## 📌 Puntos clave de la app
- Interfaz moderna con Jetpack Compose.  
- Navegación fluida entre lista y mapa.  
- Uso de coroutines para carga asíncrona de datos.  
- Uso de Google Maps API para mostrar la localización real.  
- **Filtros dinámicos** mediante switches para ver solo estaciones con bicis o espacios disponibles.  

---

## 🚲 Conclusión
La app **AplicaciónBicis** es un prototipo funcional que:  
- Integra múltiples librerías modernas de Android.  
- Muestra cómo trabajar con datos externos (CSV).  
- Presenta una UI interactiva y práctica para el usuario.  
- Permite filtrar estaciones según disponibilidad de bicicletas o espacios, mejorando la experiencia de uso.  

---

## 📂 Repositorio
Puedes encontrar la aplicación en GitHub:  
[https://github.com/RobertMoraMoreno/AplicacionBicisDisponibles](https://github.com/RobertMoraMoreno/AplicacionBicisDisponibles)  

---

## 👨‍🎓 Autor
**Roberto Mora Moreno**  
**Curso:** 2º DAM
