# Examen Final - WordPress en AWS con S3 Estático

## Datos generales

- Estudiante: Coila Mamani Jhoel Midwar
- Curso: Virtualización de servicios tecnológicos
- Proyecto: Portal WordPress para Comercial Nova
- Región: us-east-1

## Descripción

Este repositorio contiene la documentación final del examen de virtualización, donde se implementó un portal WordPress en AWS integrando servicios de cómputo, red, base de datos, almacenamiento estático, monitoreo, seguridad y balanceo de carga.

## Servicios implementados

- Amazon VPC
- Amazon EC2
- Amazon RDS MySQL
- Amazon S3
- Application Load Balancer
- Target Group
- Security Groups
- Amazon CloudWatch
- Alarma de CloudWatch

## Arquitectura general

Usuario final → Application Load Balancer → EC2 WordPress → Base de datos

También se configuró Amazon S3 para almacenamiento de archivos estáticos y CloudWatch para monitoreo de métricas y alarmas.

## Evidencias principales

El informe incluye capturas de:

1. VPC y grupos de seguridad.
2. Instancia EC2 en ejecución.
3. Base de datos RDS.
4. Instalación y funcionamiento de WordPress.
5. Bucket S3 con versionado y ciclo de vida.
6. Archivos cargados en S3.
7. Dashboard de CloudWatch.
8. Alarma de CloudWatch.
9. Grupo de destino en buen estado.
10. Application Load Balancer activo.
11. WordPress funcionando desde el DNS del ALB.

## Archivos del repositorio

- `Informe_Final_WordPress_AWS_S3_Comercial_Nova.docx`: informe editable en Word.
- `Informe_Final_WordPress_AWS_S3_Comercial_Nova.pdf`: informe final en PDF.
- `fin.docx`: documento de evidencias originales.
- `/evidencias`: carpeta para capturas adicionales.

## Costos y optimización

Debido a las restricciones del entorno AWS Academy, la estimación de costos se realizó de manera referencial. Los costos principales corresponden a EC2, RDS, S3, ALB y CloudWatch.

Acciones de optimización:

1. Apagar o eliminar recursos al finalizar.
2. Usar instancias tipo micro.
3. Aplicar ciclo de vida en S3.
4. Reducir la retención de backups en entornos de laboratorio.
5. Eliminar recursos no utilizados como balanceadores, snapshots o buckets temporales.

## Conclusión

Se logró implementar un portal WordPress funcional en AWS con evidencias de red, cómputo, almacenamiento, monitoreo, balanceo de carga y optimización de costos.
