# Maestria - Catalog Service 📚

Microservicio encargado de la gestión de cursos, módulos, lecciones y recursos. Utiliza PostgreSQL con Prisma ORM.

## 🚀 Requisitos e Instalación

### 1. Contratos gRPC (Obligatorio)
Clona el repositorio de contratos en el **mismo directorio padre** donde está este microservicio con el nombre `grpc-contracts`:

```bash
# Desde el directorio padre común:
git clone https://github.com/Pryectomaestria1/maestria-grpc-contracts.git grpc-contracts
```

La estructura de carpetas debe quedar así:
```
directorio-padre/
├── maestria-catalog-service/  (Este repositorio)
└── grpc-contracts/
```

### 2. Base de Datos (Prisma)
Asegúrate de tener la infraestructura de Docker encendida (`docker-compose up -d` en el gateway) y aplica el esquema de la base de datos:

```bash
npm install
npx prisma db push
```

### 3. Ejecución del Servicio
Inicia el microservicio en modo desarrollo (corre en el puerto gRPC `50052`):

```bash
npm run start:dev
```
