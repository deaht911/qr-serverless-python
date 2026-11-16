# QR Serverless – Python + Vercel

Microservicio serverless que recibe un texto o enlace por parámetro GET y devuelve una imagen PNG con el código QR.

**Autor:** Samuel Eli Ramirez Mamani – Arquitectura de Software – Universidad Adventista de Bolivia

## Estructura

```
qr-serverless-python/
├── api/
│   └── generate.py
├── pyproject.toml
├── requirements.txt
└── README.md
```

## Uso

```
https://TU_DOMINIO.vercel.app/api/generate?text=https://es.wikipedia.org/wiki/Serverless
```

- `text` (opcional): texto o URL a codificar. Por defecto: `https://github.com`.
- Respuesta: `200 image/png` con el QR, o `500 text/plain` si hay error.

## Despliegue

1. `git init && git add . && git commit -m "Inicial"`
2. Crear repositorio en GitHub y vincular el remoto (`git remote add origin ...` y `git push -u origin main`).
3. En Vercel: **Add New… → Project**, importar el repositorio.
4. Clic en **Deploy**.
