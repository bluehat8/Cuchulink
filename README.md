# Cuchulink
🏆 1er lugar en Hackathon ETH Salvador 2024
- Mejor Dapp sobre Ethereum 

Una Dapp innovadora que moderniza los tradicionales cuchubales, aprovechando la tecnología blockchain de Ethereum para proporcionar una plataforma segura, transparente y accesible para el ahorro y préstamos comunitarios.
Cuchulink es una aplicación descentralizada (DApp) para crear y gestionar "Cuchubales" en la testnet de Scroll Sepolia. Un "Cuchubal" es una especie de grupo de ahorro donde los participantes aportan un monto total y participan en rondas para ganar el fondo acumulado. La interfaz web interactúa con un contrato inteligente desplegado en la red de prueba para facilitar la gestión de estos grupos.

## Características

- Crear nuevos Cuchubales.
- Ver y unirse a Cuchubales existentes.
- Consultar la lista de Cuchubales creados para posteriormente unirse a ellos.
- Cuando un usuario se une a un cuchubal, tiene que aportar el monto de la ronda
- Ver la lista de participantes y el historial de rondas de un Cuchubal.
- Se muestra el ganador de las rondas en el historial (solamente cuando todos los participantes aportaron a la ronda)

## Requisitos

- Navegador web compatible con Web3 (como MetaMask).

## Configuración del Entorno

1. **Clona el repositorio:**

    ```bash
    git clone https://github.com/tu-usuario/cuchulink.git
    cd cuchulink
    ```

2. **Instala las dependencias necesarias:**

    Aunque el proyecto principal no requiere una instalación de dependencias específicas en el frontend, asegúrate de tener las siguientes configuraciones:

    - **MetaMask:** Debes tener MetaMask instalado y configurado para conectarte a la red de prueba Scroll Sepolia.
    - **Web3js:** Debes tener el script de la librería web3js en los archivos html del proyecto

3. **Obtén el ABI del contrato:**

    Asegúrate de tener el archivo `CuchulinkABI3.json` en la carpeta V3 del proyecto. Este archivo debe contener la definición del contrato inteligente en formato JSON.

4. **Configura el contrato:**

    Actualiza la dirección del contrato en el archivo HTML (`contractAddress` en el script). Esta dirección debe corresponder a la dirección del contrato inteligente desplegado en la red Scroll Sepolia.

    ```javascript
    const contractAddress = '0x51061402B9C12DBf0F8efcCB46399eB4c615a65e';
    ```

## Uso (NOTA: deben utilizarse los archivos del directorio V3 del proyecto)

1. **Crear un Cuchubal:**

    Completa el formulario en la sección "Crear Cuchubal" con el nombre, monto total, fecha de inicio, número de participantes y código del Cuchubal. Haz clic en "Crear" para desplegar un nuevo Cuchubal en la red.

2. **Ver y Unirse a Cuchubales:**

    En la sección "Mis Cuchubales," se mostrará una lista de todos los Cuchubales que has creado. Puedes unirte a otros Cuchubales y consultar detalles adicionales como participantes y historial de rondas.

3. **Consultar Participantes y Historial de Rondas:**

    Utiliza los botones correspondientes para ver la lista de participantes y el historial de rondas de un Cuchubal.

## Contrato Inteligente

El contrato inteligente está escrito en Solidity y se encuentra en el siguiente repositorio: https://app.atlaszk.com/ide?m=eNUHzb. Asegúrate de desplegar el contrato "CuchulinkV2" en la red de prueba Scroll Sepolia usando la IDE Atlas.

## Despliegue del Contrato

Para desplegar el contrato inteligente:

1. **Accede a la IDE Atlas.**
2. **Carga el smart contract CuchulinkV2.**
3. **Configura la red de despliegue como Scroll Sepolia.**
4. **Despliega el contrato.**

Asegúrate de copiar la dirección del contrato desplegado y actualizarla en el archivo HTML del frontend. Así como el ABI del propio contrato desplegado

