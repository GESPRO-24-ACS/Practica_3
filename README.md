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

**Guía de cómo se realiza toda la secuencia de acciones desde que nos posicionamos en un nuevo commit del repositorio Go Bees hasta que pasa a estar visible en nuestra rama master local**

 **1. Go Bees (GitKraken)**:
   - **Acción**: Posicionarse en el commit para subir cambios.
   - Abrimos GitKraken y nos asegúramos de estar en el repositorio correcto. NOs dirigimos al commit correspondiente donde queremos comenzar a trabajar, generalmente el commit que incluye los últimos cambios del proyecto.

 **2. P3 (GitKraken)**:
   - **Acción**: Tener la rama **master** actualizada y posicionarse en **master**.
   - Nos debemos asegurar de que la rama **master** está al día con los cambios más recientes. Seleccionamos la rama **master** en GitKraken y confirmamos que está actualizada con los últimos cambios. Si es necesario, haremos un **pull** para sincronizarla.

 **3. P3 (GitHub)**:
   - **Acción**: Crear una rama a partir de la tarea con el nombre **Go Bees**.
   - En GitHub, creamos una nueva rama a partir de **master**. Asignaremos un nombre a la nueva rama para identificar fácilmente el trabajo en esta tarea.

 **4. P3 (GitKraken)**:
   - **Acción**: Posicionarse en la rama en local.
   - Regresamos a GitKraken y cambiamos a la nueva rama que acabamos de crear. Esto nos permitirá realizar y confirmar los cambios en una rama separada, sin afectar directamente a **master**.

 **5. Añadir cambios de la carpeta Go Bees a la carpeta P3 (Excluir .git)**:
   - **Acción**: Copia los archivos modificados de la carpeta **Go Bees** a la carpeta **P3**, asegurándote de excluir la carpeta **.git** para evitar conflictos con el repositorio.
   - Agregamos los cambios que hemos realizado en la carpeta **Go Bees** a la estructura de la carpeta **P3** en el repositorio local. Excluiremos la carpeta **.git** para evitar problemas con las configuraciones de Git.

 **6. Git Stage all & Git Commit (Nombre commit)**:
   - **Acción**: Usar el comando **Git Stage all** para agregar todos los cambios al área de preparación. Luego, haz un **git commit** con un mensaje claro describiendo los cambios realizados.
   - En GitKraken, seleccionamos todos los cambios que deseamos agregar al commit y haremos clic en **Stage All**. Luego, escribimos un mensaje de commit que describa los cambios realizados.

 **7. Git Fetch All & Sincronización**:
   - **Acción**: Realiza **Git Fetch All** y, dependiendo de si es necesario, ejecuta **git pull** o **git push**.
   - 
     - Si la rama está desactualizada y hay cambios en el repositorio remoto, primero ejecutaremos **git pull** para actualizar la rama local.
     - Si no es necesario hacer un pull (es decir, si no hay cambios nuevos), simplemente realizaremos un **git push** para enviar los cambios al repositorio remoto.

 **8. Crear PR (Pull Request)**:
   - **Acción**: Crea un PR (Pull Request) de tu rama **Go Bees** hacia **master** en GitHub.
   - Una vez que hayamos subido tus cambios a GitHub, crearemos un Pull Request (PR) desde la rama correspondiente hacia la rama **master** del repositorio. Esto permite la revisión de los cambios antes de que se fusionen en **master**.

 **9. Merge PR y Actualizar master en local**:
   - **Acción**: Merge PR y actualizar **master** en local con **git pull**.
   - Una vez que el PR haya sido revisado y aprobado, haremos el merge en GitHub. Después, regresamos a GitKraken y actualizaremos la rama **master** local con **git pull** para asegurarnos de que tu rama **master** local está sincronizada con los cambios fusionados desde el PR.

---


###GITKRAKEN 
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
