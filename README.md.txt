cat > README.md <<'EOF'
# PdespliegueDJ

Proyecto Django corregido y preparado para desplegar en Render.

## Requisitos
- Python 3.11+
- Dependencias en requirements.txt

## Despliegue en Render
- Start command: `gunicorn prjrender.wsgi:application`
- Añadir SECRET_KEY en variables de entorno de Render
- Ejecutar migraciones: `python manage.py migrate`
EOF

git add README.md
git commit -m "Add README"
git push
