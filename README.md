<h1 align="center">Bienvenido 👋</h1>
<p>
  <a href="LICENSE" target="_blank">
    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg" />
  </a>
  <a href="https://twitter.com/rodrigotesone97" target="_blank">
    <img alt="Twitter: Rodrigo Tesone" src="https://img.shields.io/twitter/follow/rodrigotesone97.svg?style=social" />
  </a>
</p>

> El repositorio consta de un script que scrapea la pagina web de la [Municipalidad de Rosario](https://www.rosario.gob.ar/web/gobierno/personal/sueldos), descarga los pdf que contienen los sueldos dentro de ella, verifica si los pdf contienen el año y la fecha que figuren en [este](ultimos_datos.dat) archivo.</br>
> En caso de que haya nuevos archivos un bot de telegram me envia un mensaje como el siguiente notificandome:</br></br>

![Demo](Demo.jpeg)

## 📂 Clonar Repositorio

```
git clone https://github.com/rodrigotesone1997/Scrapper_Sueldos_Municipales.git
```

## 🐍 Versión de Python

```
Python 3.8.8
```

## 👨‍💻 Instalación

#### 🪟 Usuarios Windows:

Ademas de los requerimientos que estan [aquí](requirements.txt) es posible que surga el siguiente error al momento de uso:

```
TesseractNotFound Error: tesseract is not installed or it's not in your path
```

En ese caso se recomienda seguir el siguiente [video](https://www.youtube.com/watch?v=DG5D8A3zi4o&ab_channel=MotechApp).</br>
El paquete `pdf2image` necesita la descarga del ejecutable ubicado [aquí](https://github.com/oschwartz10612/poppler-windows/releases/).
Para mas información al respecto mirar https://www.geeksforgeeks.org/convert-pdf-to-image-using-python/ .

#### 🐧 Usuarios Linux:

Asi lo instale en Ubuntu 20.04 pero por lo que vi es similar en otras distros.</br>
Se necesita instalar `tesseract-ocr` con el siguiente comando:

```
apt-get install tesseract-ocr
```

Luego instalar:

```
apt-get install tesseract-ocr-EN
```

EN debe ser reemplazado por el idioma para el que quieras utilizarlo.En este caso es español:

```
apt-get install tesseract-ocr-spa
```

Aunque yo recomiendo usar `apt-get install tesseract-ocr-all` asi podes usarlo sin restricciones.</br>
Informacion sobre la instalacion [aca](https://linuxhint.com/install-tesseract-ocr-linux/) y sobre la instalacion de español [aca](https://parzibyte.me/blog/2019/05/18/instalar-tesseract-ocr-idioma-espanol-ubuntu/).

## ⚙️ Uso

1. (Opcional) Crear un entorno virtual `virtualenv` y activarlo.
2. Instalar las depedencias `pip install -r requirements.txt`
3. Reemplazar la variable `path_repositorio` con el path del repositorio clonado.
4. Revisar el código en caso de necesitar comentar algunas lineas (mas información comentada en el código)
5. Por último, ejecutar [app.py](app.py)

## 🔮 Futuro del Proyecto

Proximamente publicare un repositorio que seria la "Fase 2" del proyecto donde se crearia una carpeta donde se limpiarian los datos en pdf a archivos .xlsx.</br>
UPDATE: Estoy re-escribiendo el proyecto en un pipe-line con airflow.

## ✉️ Contacto

Cualquier sugerencia de arquitectura de código,pregunta o problema enviar mail a rodrigotesone97@outlook.com.ar

## 🤔 Autor

👤 **Rodrigo Tesone**

* Twitter: [@rodrigotesone97](https://twitter.com/rodrigotesone97)
* Github: [rodrigotesone1997](https://github.com/rodrigotesone1997)
* LinkedIn: [rodrigo-tesone](https://linkedin.com/in/rodrigo-tesone)

## 🤝 Contribuciones y Agradecimientos

Agradezco a [Bautista](https://github.com/coltking) por la motivación e ideas al proyecto , a [Alejandro](https://github.com/alexdraven) la revisión del código, a mi hermana pequeña por la selección de emojis 😉 y a la Municipalidad de Rosario por publicar tan pauperrimamente sus datos y obligarme a hacer esto.


## 📝 Licencia

Copyright © 2021 [Rodrigo](https://github.com/rodrigotesone1997).<br />
This project is [MIT](LICENSE) licensed.

***
_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_
