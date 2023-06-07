# Карточка и неоновая кнопка на языке HTML и CSS
## Пример работы
![ezgif-2-d863acda40](https://github.com/Sazukiro/Card-and-Neon-Button/assets/133951840/704f40cb-925d-43c9-ace6-c8ca19918d6b)
## Описание кода
Сам код написан на двух языках программирования: HTML, CSS.
Основным ядром, если так можно выразиться, данного кода можно назвать файл HTML "Card and Neon Button.html".

В нём находятся:
- **Ссылки на CSS файлы карточки("kartochka.css") и неоновой конпки("neon.css")**
- **Обращение к CSS файлам через классы**
- **Основной текст написанный на передней и задней стороне карточки и неоновой кнопки**

За визуальную же часть отображения данных объектов отвечает язык CSS.
В обоих css файлах основой является вкладка `body`, в которой указан цвет фона, указание того, что шрифт без засечек, а также свойство `flex-wrap:wrap`, которое позволяет выстроить объекты в несколько строк если они не умещаются.

### **Для переворота карточки я использовал такие свойства как:**

`position: relative` и `position: absolute` для того, чтобы одна сторона кароточки перекрывалась другой и текст на задней стороне был отзеркален, чтобы при повороте текст на задней строне был читаем. Также для самого поворота использовал свойство `transform:rotateY(180deg)`, которое позволяет перевернуть карточку на 180 градусов по оси Y. 
Для того, чтобы поворот осуществлялся при наведении я использовал псевдокласс `hover`. А с помощью свойства `perspective` мы задаём глубину нашей карточке, чтобы поворот выглядел объёмно.


### **Для неоновой кнопкия использовал такие свойства как:**

Создание в HTML файле отдельных классов для каждого движущегося элемента по краям текста:

```html
  <a href="#" class="button">
        <span class="button__line button__line--top"> </span>
        <span class="button__line button__line--right"></span>
        <span class="button__line button__line--bottom"></span>
        <span class="button__line button__line--left"></span>
```
Использование в блоке `.button` свойство `overflow: hidden` для того чтобы все объекты уходящие за пределы кнопки исчезали:
```css
 .button {
...
...
    overflow: hidden;
}
```
Использование псевдо класса `hover` для анимации каждого элемента при наведении мыши, а также для загарания кнопки, в котором также используется `box-shadow`, которая формирует свечение от краёв кнопки. Пример блока одного из элементов, а также блока для кнопки:
```css
 .button:hover .button__line--top{ 
    left:100%; 
    transition:1s ; -webkit-transition:1s ; -moz-transition:1s ; -ms-transition:1s ; -o-transition:1s ;
    transition-delay: 0.25s;
}

.button:hover { 
   background-color: aqua;
   color:#333;
    box-shadow: 0 0 10px aqua,0 0 40px aqua, 0 0 80px aqua ;
    transition-delay: 1s;
}
```
# ССылка на код: 
**https://github.com/Sazukiro/Card-and-Neon-Button/tree/main/Card%20and%20Neon%20Button**
# Ссылка на теоретический материал:
[![CSS фичи #17 анимированная неоновая кнопка | CSS3 Button Style Neon Style](https://i.ytimg.com/vi/__rxApMI_Us/maxresdefault.jpg)](https://www.youtube.com/watch?v=__rxApMI_Us)

