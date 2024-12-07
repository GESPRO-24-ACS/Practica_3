Nombre de los compañeros

Guillermo Arce

Pablo Citores

David Santamaria


![header](https://cloud.githubusercontent.com/assets/6546265/22174630/785cdf04-dfe3-11e6-8cf4-024e8dc1c051.png)

[![ZenHub](https://raw.githubusercontent.com/ZenHubIO/support/master/zenhub-badge.png)](https://zenhub.com)
[![Build Status](https://travis-ci.org/davidmigloz/go-bees.svg?branch=master)](https://travis-ci.org/davidmigloz/go-bees)
[![codecov](https://codecov.io/gh/davidmigloz/go-bees/branch/master/graph/badge.svg)](https://codecov.io/gh/davidmigloz/go-bees)
[![Code Climate](https://codeclimate.com/github/davidmigloz/go-bees/badges/gpa.svg)](https://codeclimate.com/github/davidmigloz/go-bees)
[![SonarQube](https://sonarqube.com/api/badges/gate?key=go-bees)](https://sonarqube.com/component_measures/?id=go-bees)
[![Dependency Status](https://www.versioneye.com/user/projects/57f7b19e823b88004e06ad33/badge.svg?style=flat-square)](https://www.versioneye.com/user/projects/57f7b19e823b88004e06ad33)
[![Documentation Status](https://readthedocs.org/projects/go-bees/badge/?version=develop)](http://go-bees.readthedocs.io/es/develop/?badge=develop)

**GUIA DE COMO REALIZAR LA SECUENCIA DE ACCIONES DESDE EL COMMIT HASTA QUE ES VISIBLE EN NUESTRA RAMA MASTER LOCAL**
A continuación, te proporciono la guía siguiendo el esquema de la imagen adjunta:

---

## **Guía de Acción: Secuencia de Acciones en GitKraken**

### **1. Go Bees (GitKraken)**:
   - **Acción**: Posicionarse en el commit para subir cambios.
   - **Descripción**: Abre GitKraken y asegúrate de estar en el repositorio correcto. Dirígete al commit correspondiente donde quieres comenzar a trabajar, generalmente el commit que incluye los últimos cambios de tu proyecto.

### **2. P3 (GitKraken)**:
   - **Acción**: Tener la rama **master** actualizada y posicionarse en **master**.
   - **Descripción**: Asegúrate de que tu rama **master** está al día con los cambios más recientes. Selecciona la rama **master** en GitKraken y confirma que está actualizada con los últimos cambios. Si es necesario, haz un **pull** para sincronizarla.

### **3. P3 (GitHub)**:
   - **Acción**: Crear una rama a partir de la tarea con el nombre **Go Bees**.
   - **Descripción**: En GitHub, crea una nueva rama a partir de **master**. Asigna un nombre descriptivo a la nueva rama, como **GoBees**, para identificar fácilmente el trabajo en esta tarea.

### **4. P3 (GitKraken)**:
   - **Acción**: Posicionarse en la rama en local.
   - **Descripción**: Regresa a GitKraken y cambia a la nueva rama **Go Bees** que acabas de crear. Esto te permitirá realizar y confirmar tus cambios en una rama separada, sin afectar directamente a **master**.

### **5. Añadir cambios de la carpeta Go Bees a la carpeta P3 (Excluir .git)**:
   - **Acción**: Copia los archivos modificados de la carpeta **Go Bees** a la carpeta **P3**, asegurándote de excluir la carpeta **.git** para evitar conflictos con el repositorio.
   - **Descripción**: Agrega los cambios que has realizado en la carpeta **Go Bees** a la estructura de la carpeta **P3** en tu repositorio local. Excluye la carpeta **.git** para evitar problemas con las configuraciones de Git.

### **6. Git Stage all & Git Commit (Nombre commit)**:
   - **Acción**: Usar el comando **Git Stage all** para agregar todos los cambios al área de preparación. Luego, haz un **git commit** con un mensaje claro describiendo los cambios realizados.
   - **Descripción**: En GitKraken, selecciona todos los cambios que deseas agregar a tu commit y haz clic en **Stage All**. Luego, escribe un mensaje de commit que describa los cambios realizados (por ejemplo, "Añadidos cambios de Go Bees a la carpeta P3").

### **7. Git Fetch All & Sincronización**:
   - **Acción**: Realiza **Git Fetch All** y, dependiendo de si es necesario, ejecuta **git pull** o **git push**.
   - **Descripción**:
     - Si tu rama está desactualizada y hay cambios en el repositorio remoto, primero ejecuta **git pull** para actualizar tu rama local.
     - Si no es necesario hacer un pull (es decir, si no hay cambios nuevos), simplemente realiza un **git push** para enviar tus cambios al repositorio remoto.

### **8. Crear PR (Pull Request)**:
   - **Acción**: Crea un PR (Pull Request) de tu rama **Go Bees** hacia **master** en GitHub.
   - **Descripción**: Una vez que hayas subido tus cambios a GitHub, crea un Pull Request (PR) desde tu rama **Go Bees** hacia la rama **master** de tu repositorio. Esto permite la revisión de los cambios antes de que se fusionen en **master**.

### **9. Merge PR y Actualizar master en local**:
   - **Acción**: Merge PR y actualizar **master** en local con **git pull**.
   - **Descripción**: Una vez que tu PR haya sido revisado y aprobado, haz el merge en GitHub. Después, regresa a GitKraken y actualiza tu rama **master** local con **git pull** para asegurarte de que tu rama **master** local está sincronizada con los cambios fusionados desde el PR.

---


GITKRAKEN
**Gráfico obtenido con una captura de pantalla con la lista de commits del repositorio**

![image](https://github.com/user-attachments/assets/95d2821d-188e-4864-aadf-5d2724e4300a)



**Captura de pantalla del primer commit**
![image](https://github.com/user-attachments/assets/5aadb7ae-5594-486d-a267-0ec580f2e91c)


**Captura de pantalla del último commit**
![image](https://github.com/user-attachments/assets/84dee2df-1b68-4257-9b1d-383c2b23ab10)



**La información del proyecto de Github obtenida desde la opción de menú "Insights→Pulse"**
![image](https://github.com/user-attachments/assets/6d8adb1a-0227-47fe-9c50-f1c263a528da)

**La información del proyecto de Github obtenida desde la opción menú "Insights→ Code frequency"**
![image](https://github.com/user-attachments/assets/f701d087-961d-4cc5-85bb-cbeff9b07705)

**Captura con la relación de las PRQs realizadas cerradas**
![image](https://github.com/user-attachments/assets/6782e03f-dbde-4048-8d8f-6b0e3426c074)






## License

Copyright (c) 2016 - 2017 David Miguel Lozano

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.
