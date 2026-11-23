# Formularios en Django

Formulario de registro de usuarios para el e-commerce, hecho con `ModelForm` y validaciones propias. Forma parte de la serie de tareas del proyecto e-commerce de la profesión Full Stack Python de EBAC. Cada repositorio guarda el proyecto como quedó al terminar ese tema; la versión final es [e-commerce-completo](https://github.com/Moremaster123/e-commerce-completo).

## Tecnologías

- Python y Django 6.1
- SQLite

## Qué hace el formulario

- Pide usuario, nombre, apellido, correo y la contraseña dos veces. Todos los campos son obligatorios.
- Revisa que el correo no esté registrado.
- Revisa que las contraseñas coincidan y que cumplan las reglas de seguridad de Django (`validate_password`).
- Si todo está bien, crea el usuario y muestra un mensaje de éxito.

El formulario está en `/accounts/register/`. También incluye el panel de ventas con gráficas del tema anterior en `/sales/`.

## Cómo ejecutarlo

```bash
python -m venv venv
venv\Scripts\activate        # en Linux o macOS: source venv/bin/activate
pip install django
python manage.py migrate
python manage.py runserver
```

Abre `http://127.0.0.1:8000/accounts/register/`.

## Autor

Juan Carlos González Herrera · [LinkedIn](https://www.linkedin.com/in/juan-carlos-desarrollador-web) · [Portafolio](https://moremaster123.github.io)
