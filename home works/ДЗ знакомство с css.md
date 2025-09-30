>[!main]
>[[знакомство с css]]
>[[проводник]]

---

## Задачи

1. Создайте новый HTML-файл и подключите к нему CSS двумя способами:
   - через внешний файл `styles/index.css`
   - через встроенный тег `<style>` внутри `<head>`

2. В теге `<style>` задайте фоновый цвет страницы `body` с помощью `background-color: #333;`

3. Создайте 4 блока `<div>` с уникальными `id`: `first`, `second`, `third`, `fourth`.  
   - каждому блоку задайте свой цвет фона и текста через `id`-селекторы  
   - используйте как имена цветов (`red`, `green`, `blue`, `yellow`), так и HEX-записи  

4. Создайте 4 встроенных элемента `<span>` с уникальными `id`: `fifth`, `sixth`, `seventh`, `eighth`.  
   - задайте им разные цвета через HEX-записи (например: `#800080`, `#ffa500`, `#ffc0cb`, `#00ffff`)  

5. Создайте 4 класса: `.green`, `.red`, `.blue`, `.yellow`.  
   - в каждом классе определите `background-color` и `color`  
   - примените эти классы к паре элементов: `<div>` и `<span>`

---

## Чек-лист для самопроверки

- [ ] Подключён CSS-файл через `<link>`  
- [ ] Подключены стили через `<style>`  
- [ ] Фон всей страницы (`body`) тёмно-серый (`#333`)  
- [ ] Созданы 4 блока `<div>` с уникальными `id`  
- [ ] Созданы 4 встроенных элемента `<span>` с уникальными `id`  
- [ ] Для `id` используются как названия цветов, так и HEX-запись  
- [ ] Созданы 4 класса `.green`, `.red`, `.blue`, `.yellow`  
- [ ] Классы применены и к `<div>`, и к `<span>`  
- [ ] Проверена работа стилей для `color` и `background-color`  

---

## решение

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>знакомство с css</title>
    <link rel="stylesheet" href="styles/index.css">
    <style>
        body {
            background-color: #333;
        }

        #first {
            background-color: red;
            color: white;
        }

        #second {
            background-color: green;
            color: white;
        }

        #third {
            background-color: blue;
            color: white;
        }

        #fourth {
            background-color: yellow;
            color: black;
        }

        #fifth {
            background-color: #800080;
            color: white;
        }

        #sixth {
            background-color: #ffa500;
            color: white;
        }

        #seventh {
            background-color: #ffc0cb;
            color: black;
        }

        #eighth {
            background-color: #00ffff;
            color: black;
        }

        .green {
            background-color: green;
            color: white;
        }

        .red {
            background-color: red;
            color: white;
        }

        .blue {
            background-color: blue;
            color: white;
        }

        .yellow {
            background-color: yellow;
            color: black;
        }
    </style>
</head>

<body>
    <div id="first">1</div>
    <div id="second">2</div>
    <div id="third">3</div>
    <div id="fourth">4</div>

    <p></p>
    <span id="fifth">5</span>
    <span id="sixth">6</span>
    <br>
    <span id="seventh">7</span>
    <span id="eighth">8</span>

    <p></p>
    <div class="green">green</div>
    <span class="green">green</span>
    <p></p>
    <div class="red">red</div>
    <span class="red">red</span>
    <p></p>
    <div class="blue">blue</div>
    <span class="blue">blue</span>
    <p></p>
    <div class="yellow">yellow</div>
    <span class="yellow">yellow</span>
</body>

</html>
