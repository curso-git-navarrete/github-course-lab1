# � Configuración de Seguridad
## Secretos del Repositorio
Este proyecto utiliza GitHub Secrets para manejar información sensible:
### Secretos configurados:
- `API_KEY_EXAMPLE` - Clave de API para servicios externos
- `DATABASE_URL_DEV` - URL de conexión a base de datos de desarrollo
### Uso en GitHub Actions:
```yaml
- name: Usar secreto
 env:
 API_KEY: ${{ secrets.API_KEY_EXAMPLE }}
 run: echo "API configurada correctamente"