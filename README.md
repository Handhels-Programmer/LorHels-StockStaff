# LorHels-StockStaff



### 🛡️ 1. Seguridad y Control de Accesos
* **Autenticación Segura:** Inicio de sesión respaldado por Firebase Auth.
* **Roles de Usuario:** Sistema de permisos inteligente (Administrador, Supervisor, Usuario). Dependiendo del rol, la aplicación oculta o muestra botones, formularios y módulos enteros para proteger la información sensible.

### 📊 2. Dashboard Interactivo
* **KPIs en Tiempo Real:** Tarjetas visuales que muestran el total de equipos y cuántos están Asignados, Disponibles o En Reparación.
* **Panel de Alertas:** Notificaciones automáticas que te avisan si hay equipos en el taller o si hay equipos disponibles acumulando polvo en el inventario.
* **Distribución Inteligente:** Barras de progreso que calculan y muestran cómo están distribuidos los equipos entre los diferentes departamentos de la empresa.

### 💻 3. Gestión Integral de Equipos
* **Registro Detallado:** Captura de datos clave (Código interno, Tipo, Marca, Modelo, S/N, IMEI, MAC, Ubicación y Estado).
* **Importación Masiva (Excel):** Capacidad de leer archivos `.xlsx` usando *SheetJS* para registrar decenas o cientos de equipos en Firebase con un solo clic, tolerando errores de formato en las columnas.
* **CRUD Completo:** Puedes crear, editar, reasignar y eliminar equipos fácilmente desde una tabla responsiva.

### 👥 4. Personal y Estructura Organizacional (Departamentos)
* **Directorio de Empleados:** Registro del personal con sus datos de contacto y cargo.
* **Gestión de Departamentos:** Creación de áreas (IT, RRHH, Ventas) asignando un Supervisor responsable.
* **Perfiles Inteligentes:** Al hacer clic en un empleado, se abre un panel que busca y muestra en tiempo real todos los equipos que esa persona tiene asignados actualmente.

### 🛠️ 5. Módulo de Taller y Mantenimiento
* **Bandeja de Reparaciones:** Una vista exclusiva para los equipos que están dañados.
* **Diagnóstico Visual (Cloudinary):** Los técnicos pueden abrir un modal, escribir el diagnóstico del problema y subir una fotografía de evidencia que se guarda en la nube sin saturar tu base de datos principal.
* **Acciones Rápidas:** Botones para marcar un equipo como "Reparado" (regresándolo al inventario) o darle de "Baja" si el daño es irreparable.

### 📈 6. Reportes y Exportación Avanzada
* **Generador Multik-filtro:** Permite cruzar datos (Ej: Buscar todas las "Laptops" que estén "Asignadas" al departamento de "Ventas").
* **Exportación Profesional:** Convierte los resultados de la búsqueda en un archivo Excel nativo (`.xlsx`) con columnas perfectamente organizadas.
* **Impresión Oficial:** Al imprimir el reporte, el sistema inyecta mágicamente un encabezado oculto con el logotipo de la app, la fecha exacta y los filtros utilizados, dándole un acabado muy formal.

### 📱 7. Sistema QR y Cédula Digital (Vista Pública)
* **Generación de Etiquetas:** Creación e impresión individual de códigos QR para pegar en los equipos físicos.
* **Escáner Inteligente:** Si alguien escanea el QR con su celular, la app detecta la URL secreta, salta la pantalla de inicio de sesión y muestra una "Cédula Digital" del equipo.
* **Perfil Público Dinámico:** Esta vista muestra a quién pertenece el equipo, sus números de serie y, si está dañado, muestra automáticamente las notas de reparación y la foto del técnico. Además, oculta los campos vacíos (como el IMEI en un monitor) para mantenerse limpia.

### 🕒 8. Trazabilidad e Historial (Línea de Tiempo)
* **Auditoría Automática:** Cada vez que un equipo se crea, se edita, se asigna o pasa por el taller, el sistema guarda un registro silencioso.
* **Línea de Tiempo Visual:** Un modal que te permite ver la historia completa de vida del equipo, detallando qué sucedió, cuándo ocurrió y qué usuario del sistema realizó el cambio.

---
