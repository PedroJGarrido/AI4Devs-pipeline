## IA usada
He utilizado Cursor con el modelo claude-3.5-sonnet

## Prompt
Como experto ingeniero DevOps., tienes que crear un archivo de configuración para GitHub Actions (.github/workflows/deploy-backend.yml) que implemente el siguiente pipeline:

### Trigger:
- El workflow debe ejecutarse automáticamente cuando se haga un **push a una rama que tenga un Pull Request abierto**.

### Pasos del pipeline:
1. **Correr los tests del backend** (puedes asumir que es un proyecto Node.js, Python o especificar el lenguaje si lo conoces).
2. **Generar el build del backend**.
3. **Desplegar el backend en una instancia EC2** de AWS. Puedes asumir que hay acceso por SSH con clave privada guardada en los secrets del repositorio (`EC2_HOST`, `EC2_USER`, `EC2_KEY`), y que el backend puede ser desplegado ejecutando un script remoto (`deploy.sh`) en la máquina EC2.

Incluye comentarios explicativos en cada paso del workflow y asegúrate de que el archivo sea funcional.