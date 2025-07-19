# Banca_Indicadores_diarios
Para tomar decisiones ágiles, la gerencia necesita monitorear indicadores operativos y comerciales diarios. Actualmente, la información se gestiona en archivos dispersos (Excel, reportes manuales), lo que dificulta la centralización, análisis y visualización de datos clave.
🏦 Caso propuesto: Gestión diaria de indicadores en Banco Nova
Contexto:

Banco Nova es una entidad financiera con varias sucursales a nivel nacional. Para tomar decisiones ágiles, la gerencia necesita monitorear indicadores operativos y comerciales diarios. Actualmente, la información se gestiona en archivos dispersos (Excel, reportes manuales), lo que dificulta la centralización, análisis y visualización de datos clave como:

Número de transacciones por día y por canal (ventanilla, cajero, app, web)

Monto total de depósitos y retiros por día

Número de clientes nuevos diarios

Solicitudes de crédito recibidas/aprobadas por día

Productividad por sucursal y por analista

Para solucionar esto, se propone diseñar una base de datos centralizada que almacene todos los datos diarios y permita generar reportes automatizados para la alta dirección.

🎯 Objetivo del sistema:
Crear una base de datos que permita registrar y consultar indicadores diarios de desempeño bancario, segmentados por fecha, sucursal, canal y analista, para una toma de decisiones rápida y fundamentada.

🧱 Entidades principales (a modelar):
Sucursal: ID, nombre, ubicación, gerente

Empleado/Analista: ID, nombre, cargo, sucursal_id

Cliente: ID, nombre, tipo (nuevo/antiguo), fecha_registro

Transacción: ID, tipo (depósito, retiro), canal (cajero, app, etc.), monto, fecha, sucursal_id

Crédito: ID, tipo, monto, estado (pendiente/aprobado/rechazado), fecha_solicitud, analista_id, cliente_id

Indicador Diario: ID, fecha, sucursal_id, total_transacciones, total_clientes_nuevos, total_creditos_aprobados, total_depositos, total_retiros, etc.

📊 Requerimientos funcionales:
Registrar las transacciones y operaciones diarias por sucursal y canal.

Registrar la productividad de los analistas (n° créditos procesados, aprobados).

Generar reportes diarios por sucursal y a nivel nacional.

Consultar la evolución de indicadores a lo largo del tiempo.

Alertar en caso de caída de indicadores clave (por ejemplo: menos de 50 clientes atendidos en una sucursal).

🔄 Consultas frecuentes esperadas:
¿Cuál fue el monto total de depósitos ayer?

¿Qué sucursal tuvo más transacciones en la última semana?

¿Cuántos créditos fueron aprobados por el analista X este mes?

¿Cuántos clientes nuevos se registraron hoy?

¿Cuál es el canal más usado para operaciones?

