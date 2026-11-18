# Tasks API · Starter para CI/CD

La aplicación ya está desarrollada. **Tu trabajo es construir los workflows en `.github/workflows/`** siguiendo la guía de retos.

## Preparación inicial (profesor, antes de publicar plantilla)

1. Con Node 22: `npm install` (genera `package-lock.json`) y `npm run format`.
2. `npm run lint && npm run format:check && npm run test:unit`.
3. Con Docker: `npm run test:integration` y `docker compose up -d --build`.
4. Publicar este repositorio como **template**, después de comprobar que todo pasa.

## Uso por el alumno

- `npm ci` · `npm run test:unit` · `npm start`
- `curl http://localhost:3000/health`
- `curl http://localhost:3000/version`
- `docker compose up -d --build` (si hay Docker)

`DATABASE_URL` activa PostgreSQL. Sin ella, los datos se mantienen en memoria y se pierden al reiniciar.
No subas `.env` ni tokens. El repositorio no contiene workflows resueltos.

⚠ El paquete entregado no incluye `package-lock.json` porque este entorno de creación no pudo instalar dependencias desde npm. El **profesor debe generarlo y verificar los scripts antes de entregar**. No ejecutar `npm ci` hasta crear y commitear el lock.
