# Instrucciones para correr el sitio

Para correr este sitio web localmente usando `http-server`, sigue estos pasos:

1. **Instalar Node.js (recomendado: usando NVM)**: Para una mejor gestión de versiones de Node.js, te recomiendo usar NVM (Node Version Manager). Puedes instalarlo ejecutando:
   
   ```bash
   curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash
   ```
   Luego, recarga tu terminal o ejecuta `source ~/.bashrc`. Una vez instalado, instala la versión LTS de Node.js:
   ```bash
   nvm install --lts
   nvm use --lts
   ```
   Si prefieres instalar Node.js directamente, descargalo desde [nodejs.org](https://nodejs.org/).

2. **Instalar http-server**: Ejecuta el siguiente comando en tu terminal para instalar `http-server` globalmente:
   ```bash
   npm install -g http-server
   ```

3. **Correr el servidor**: 
   ```bash
   http-server ./docs
   ```
   Opcionalmente, especifica un puerto (por ejemplo, 8080):
   ```bash
   http-server ./docs -p 8080
   ```

4. **Acceder al sitio**: Abre tu navegador y ve a `http://localhost:8080` (o el puerto que hayas elegido).

**Nota**: Usando NVM, puedes gestionar fácilmente versiones de Node.js. Para instalar `http-server`, usa `npm install -g http-server` como se indica, o considera usar `npx http-server` para ejecutar sin instalación global. Si tienes problemas con permisos, NVM ayuda a evitar conflictos de versiones.