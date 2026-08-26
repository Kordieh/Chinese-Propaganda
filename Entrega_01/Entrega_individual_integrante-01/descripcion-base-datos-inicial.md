# Descripción base de datos

De momento, la única base de datos que ya tengo disponible es la que corresponde al interés de búsqueda en Google de conceptos como "Año nuevo chino", a modo de contextualización para medir el interés de algunos países (en específico Chile en este caso) sobre eventos culturales de China. En ese sentido;

- **Autor y publicación de los datos**: El propietario de los datos es Alphabet (Google). Recopilados el 26 de agosto de 2026, con datos desde 2004 hasta este año. Obtenida mediante [Google Trends](https://trends.google.es/trends/explore?date=today%205-y&q=%2Fm%2F012m47&hl=es).
- **Contenido**: Datos sobre el aumento o disminución de términos de búsqueda concretos, entre 2004 y 2026, relacionados con China en Chile.
- **Pertinencia**: Esta base de datos es relevante dado que permite medir, con datos, si realmente ha existido o no un aumento en el interés hacia China (aunque no representa la única forma y no es posible afirmar de manera contundente usando únicamente Google, pero es posible establecer una tendencia lo que sí es algo humanamente alcanzable).
- **Metodología**: Los datos fueron obtenidos mediante herramientas internas de Google. Esa información no es pública.

Otra base de datos relevante serían las empresas de las cuales es dueña Tencent, junto con el porcentaje de propiedad y el país de cuál son originarias. En este caso sería necesaria la creación de la base de datos mediante web scraping y elaboración manual, dado que las disponibles actualmente no se encuentran 100% completas —o están directamente tras muros de pago—. En ese sentido:

- **Autor y publicación de los datos**: El autor en este caso sería yo, dado que tendría que armarla mediante búsqueda de datos y noticias de compras relacionadas, desde 2026 hasta 2024 (por tirar una fecha, para no abrumarme con una búsqueda de datos demasiado extensa en esta materia en específico).
- **Contenido**: Nombre de la empresa adquirida, fecha de adquisición, país de origen de la empresa adquirida, porcentaje de adquisición, monto pagado.
- **Pertinencia**: Esta base de datos es relevante dado que permite observar el tamaño de la mayor empresa de videojuegos de China (Tencent), la cual es bastante polémica dentro de la industria por su agresiva política de adquisiciones de empresas extranjeras.
- **Metodología**: Los datos serán obtenidos mediante web scraping y elaboración manual, apoyándome de sitios como el [China Global Investment Tracker](https://www.aei.org/china-global-investment-tracker/) (que permite ver las adquisiciones e inversiones de empresas chinas cuyo monto supere los 100 millones de dólares), [InvestGame](https://investgame.net/news/pdf/2026-03-19-tencent_q4_2025_wp/) que permite ver los reportes financieros de las empresas de videojuegos junto a sus inversiones y portales de noticias especializados en la materia como lo son [Eurogamer](https://www.eurogamer.es/tencent-se-convierte-en-la-accionista-mayoritaria-de-kuro-games-el-estudio-de-wuthering-waves).

Ejemplo de cómo se vería la tabla:

| Empresa adquirida  | Porcentaje adquirido | Año de adquisición | País de origen | Monto pagado (si está disponible) |
| ------------- |:-------------:|:-------------:|:-------------:|:-------------:|
| Empresa 1 | Porcentaje 1 | Año 1 | País 1 | Monto 1 |
| Empresa 2 | Porcentaje 2 | Año 2 | País 2 | Monto 2 |
| Empresa 3 | Porcentaje 3 | Año 3 | País 3 | Monto 3 |