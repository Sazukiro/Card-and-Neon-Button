# Карточка и неоновая кнопка на языке HTML и CSS
## Пример работы
<h3 align="center"> ![ezgif-2-d863acda40](https://github.com/Sazukiro/Card-and-Neon-Button/assets/133951840/704f40cb-925d-43c9-ace6-c8ca19918d6b)</h3>
## Описание кода
Сам код написан на двух языках программирования: HTML, CSS.
Основным ядром, если так можно выразиться, данного кода можно назвать файл HTML "Card and Neon Button.html".

В нём находятся:
- **Ссылки на CSS файлы карточки("kartochka.css") и неоновой конпки("neon.css")**
- **Обращение к CSS файлам через классы**
- **Основной текст написанный на передней и задней стороне карточки и неоновой кнопки**

За визуальную же часть отображения данных объектов отвечает язык CSS.
В обоих css файлах основой является вкладка **body**, в которой указан цвет фона, указание того, что шрифт без засечек, а также свойство **"flex-wrap:wrap"**, которое позволяет выстроить объекты в несколько строк если они не умещаются.

Для переворота карточки я использовал такие свойства как **"position: relative"** и **"position: absolute"** для того, чтобы одна сторона кароточки перекрывалась другой и текст на задней стороне был отзеркален, чтобы при повороте текст на задней строне был читаем. Также для самого поворота использовал свойство **"transform:rotateY(180deg)"**, которое позволяет перевернуть карточку на 180 градусов по оси Y. 
Для того, чтобы поворот осуществлялся при наведении я использовал псевдокласс **"hover"**. А с помощью свойства **"perspective"** мы задаём глубину нашей карточке, чтобы поворот выглядел объёмно.

