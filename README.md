# "Методи та технології розробки програмного забезпечення"

## Мета лабораторної роботи
Продемонструвати базові навички роботи з системою контролю версій Git

## Хід роботи 
Реалізувати програму, яка вміє на вхід приймати шлях до текстового файлу
із розміткою Markdown та генерувати з нього фрагмент HTML-розмітки.

## Використання 

Щоб запустити програму в дію, вам потрібно в терміналі ввести команду:

```
node index.js <шлях до вашого md файлу> --out <шлях до html файлу>
```

### Приклад md файлу
```
Форматування Markdown:

**Колобок**

Жили собі дід та баба, та такі убогі, що нічого в них не було. Одного разу дід і каже:

– _Бабусю! Піди у хижку та назмітай у засіці борошна, та спечи мені колобок._

\```
Баба так і зр_обила. Спекла **колобок** і залишила на вікні, щоб простиг.
А він з вікна та на призьбу, а з _призьби_ та на землю, та й покотився дорогою.
\```

Котиться, котиться, а назустріч йому зайчик-побігайчик:

– `Колобок, колобок, я тебе з’їм!`

– Не їж мене, **зайчику-побігайчику**, я тобі пісню засп*іваю.

– Я по _коробу_ метений, На яйцях спечений, Я від баби втік, я **від** діда втік, І від тебе втечу!
```

### Результат програми
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
<p>Форматування Markdown:</p>
<p><b>Колобок</b></p>
<p>Жили собі дід та баба, та такі убогі, що нічого в них не було. Одного разу дід і каже:</p>
<p>–  <em>Бабусю! Піди у хижку та назмітай у засіці борошна, та спечи мені колобок.</em> </p>
<p><pre>
Баба так і зр_обила. Спекла **колобок** і залишила на вікні, щоб простиг.
А він з вікна та на призьбу, а з _призьби_ та на землю, та й покотився дорогою.
</pre></p>
<p>Котиться, котиться, а назустріч йому зайчик-побігайчик:</p>
<p>–  <tt>Колобок, колобок, я тебе з’їм!</tt> </p>
<p>– Не їж мене, <b>зайчику-побігайчику</b>, я тобі пісню засп*іваю.</p>
<p>– Я по  <em>коробу</em>  метений, На яйцях спечений, Я від баби втік, я <b>від</b> діда втік, І від тебе втечу!</p>
</body>
</html>
```

### revert-коміт
https://github.com/ToxicAli3n/MTRPZ_Lab.1/commit/40e240587a05387d8c82d80675d34ead4f022722