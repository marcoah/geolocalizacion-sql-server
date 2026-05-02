# geolocalizacion-sql-server

Repositorio de pruebas para funciones de geolocalizacion en SQL Server 2022 en adelante

En la seccion de SQL Server hay codigo para generar una base de datos llamada geolocalizacion que contiene informacion de ventas para una distribuidora ficticia de productos farmaceuticos que vende directamente a clientes que son hospitales, clinica y farmacias en toda Argentina y con diferentes problemas en el
maestro de Clientes.

---

## 📂 Estructura del repositorio

```text
proyecto/
├── data/
│   └── datos_salud.csv
├── SQL/
│   └── [Ver instrucciones para SQL Server](docs/instrucciones_SQL.md)
└── README.md
```

- **data/**: contiene el CSV original con direcciones sin geocodificar y el archivo base para la creacion de BD en SQL Server
- **SQL/**: scripts SQL (no usados por este proceso)

---

## Pasos de Instalación de Archivos de datos

Copiar todo el contenido de la carpeta `data` a la ubicación `C:\data` en el servidor:

```bash
# Desde la línea de comandos (CMD) con permisos de administrador
xcopy /E /I /Y ".\data" "C:\data"
```

O manualmente:

1. Crear la carpeta `C:\data` si no existe
2. Copiar todos los archivos desde la carpeta `data` del proyecto a `C:\data`

---

## 📌 Funcionalidad MS SQL Server

### Instrucciones para crear BD en SQL Server

Para ver las instrucciones especificas para el entorno de SQL Server puedes ver el documento [Ver instrucciones para SQL Server](docs/instrucciones_SQL.md)

### Funciones Geo-espaciales

Para ver las funciones geoespaciales puedes ver el documento [Ver funciones](docs/geospatial_functions.md)

## ⚠️ Consideraciones importantes

- NOTAS

---

## 📄 Licencia

Uso libre. Mapas felices, desarrolladores también.

---

## Autor

Este repositorio ha sido creado por [Marco Hernandez](https://www.linkedin.com/in/marcoah17/) como parte de la charla **Cómo aprovechar las funciones geográficas de SQL Server en soluciones reales de negocio** para el **POWER PLATFORM BOOTCAMP BUENOS AIRES 2026**.
