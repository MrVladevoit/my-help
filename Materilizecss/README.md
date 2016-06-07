# Моя шпаргалка по работе с Materializecss.com

![alt tag](https://scotch.io/wp-content/uploads/2015/01/getting-started-materialize-css-framework.png)

Materializecss.com - это фремворк material designer на SASS.

1. Скачать
 + [Скачать и использовать](#Установка-GIT);


## Скачать и использовать Materializecss.com

Для того, чтобы начать переходим по ссылке : http://materializecss.com/getting-started.html

###CDN

Можно не скачивать файлы на локальный компьютер, достаточно подключить CDN

```html

	<!-- Compiled and minified CSS -->
	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/materialize/0.97.6/css/materialize.min.css">

	<!-- Compiled and minified JavaScript -->
	<script src="https://cdnjs.cloudflare.com/ajax/libs/materialize/0.97.6/js/materialize.min.js"></script>

```

###NPM and Bower

Установить **materialize** можно через **npm** или с помощью Bower

- `npm install materialize-css`

- `bower install materialize`

## Запуск

После загрузки распакуйте файлы в папку, где размещен сайт. Структура файлов выглядит следующим образом.

```

	 MyWebsite/
  |--css/
  |  |--materialize.css
  |
  |--fonts/
  |  |--roboto/
  |
  |--js/
  |  |--materialize.js
  |
  |--index.html

```

### Запуск HTML

```html

  <!DOCTYPE html>
  <html>
    <head>
      <!--Import Google Icon Font-->
      <link href="http://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
      <!--Import materialize.css-->
      <link type="text/css" rel="stylesheet" href="css/materialize.min.css"  media="screen,projection"/>

      <!--Let browser know website is optimized for mobile-->
      <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    </head>

    <body>
      <!--Import jQuery before materialize.js-->
      <script type="text/javascript" src="https://code.jquery.com/jquery-2.1.1.min.js"></script>
      <script type="text/javascript" src="js/materialize.min.js"></script>
    </body>
  </html>

```

###Ruby Gem, Meteor Package, Ember Package

- `gem 'materialize-sass'`

- ` meteor add materialize:materialize`

```js

# install via npm
  $ npm install ember-cli-materialize --save-dev
  # make ember-cli fetch internal dependencies
  $ ember g ember-cli-materialize

```

###Запуск, используя SASS

```
MyWebsite/
  |--css/
  |  |--materialize.css <-- compiled from scss/materialize.scss
  |
  |--fonts/
  |  |--roboto/
  |
  |--js/
  |  |--materialize.js
  |
  |--scss/
  |  |--materialize.scss
  |  |--components/
  |
  |--index.html

```

##Использование Цвета

Полное руководство и все цвета **materialize** можно посмотреть по ссылке http://materializecss.com/color.html

###Цвет фона

Для цвета фона достаточно прописать название цвета **teal** и его оттенок **lighten-2**

```html

 <div class="card-panel teal lighten-2">This is a card panel with a teal lighten-2 class</div>

```

###Цвет текста

Чтобы применить цвет текста, просто добавьте -text к классу цвета, как это:

```html

	<div class="card-panel">
		<span class="blue-text text-darken-2">This is a card panel with dark blue text</span>
	</div>

```

###Sass

Для цвета фона, вы можете применить цвет просто путем расширения классов, как на примере ниже.

```sass

	.ilike-blue-container {
		@extend .blue, .lighten-4;
	}

```
Для изменения цвета текста, вы можете применить цвет просто путем расширения классов, как на примере ниже.

```sass

	.ilike-blue-container {
		@extend .blue-text, .text-lighten-4;
	}

```

##Grid / Сетка

###Container

Container - не является обязательным элементом сетки, но он позволяет нам центрировать основной блок, контент.Чтобы добавить контейнер просто положить содержимое внутри тега **<div>** с классом контейнера. Вот пример того, как ваша страница может быть настроена.

```html

	<body>
		<div class="container">
			<!-- Page Content goes here -->
		</div>
	</body>

```

###12 колонок

Наша стандартная сетка имеет 12 колонок. Независимо от размера браузера, каждая из этих колонок всегда будет иметь одинаковую ширину.

```html

	<div class="row">
		<div class="col s1">1</div>
		<div class="col s1">2</div>
		<div class="col s1">3</div>
		<div class="col s1">4</div>
		<div class="col s1">5</div>
		<div class="col s1">6</div>
		<div class="col s1">7</div>
		<div class="col s1">8</div>
		<div class="col s1">9</div>
		<div class="col s1">10</div>
		<div class="col s1">11</div>
		<div class="col s1">12</div>
	</div>

```

###Колонки находятся внутри Строк

Помните, когда вы создаете макет, следует все столбцы добавить внутри строки, и что вы должны добавить класс Col к своему внутреннему **div**, чтобы использовать их как столбцы.

```html

	<div class="row">
		<div class="col s12">This div is 12-columns wide</div>
		<div class="col s6">This div is 6-columns wide</div>
		<div class="col s6">This div is 6-columns wide</div>
	</div>

```

###Смещения

Чтобы сместить колонку на опрелеленно расстояние, можно использовать class **.offset-s2**. Данный класс сместит нашу колонку на малых экранов на 2 колонки правее.

**Нужно запомнить, что s = small, m = medium, l = large. Это разные @media запросы, для разных экранов, разных устройств.**

```html

	<div class="row">
		<div class="col s12"><span class="flow-text">This div is 12-columns wide on all screen sizes</span></div>
		<div class="col s6 offset-s6"><span class="flow-text">6-columns (offset-by-6)</span></div>
	</div>

```

###Push and Pull
Вы можете с легкостью менять порядок колонок и толкать их или тянуть.

```html

	<div class="row">
		<div class="col s7 push-s5"><span class="flow-text">This div is 7-columns wide on pushed to the right by 5-columns.</span></div>
		<div class="col s5 pull-s7"><span class="flow-text">5-columns wide pulled to the left by 7-columns.</span></div>
	</div>

```

###Создание Макетов

**Section** - класс **секция** используется для разделения контента на секции.
**Divider** - используется для добавления разделителей.

```html

	<div class="divider"></div>
	<div class="section">
		<h5>Section 1</h5>
		<p>Stuff</p>
	</div>
	<div class="divider"></div>
	<div class="section">
		<h5>Section 2</h5>
		<p>Stuff</p>
	</div>
	<div class="divider"></div>
	<div class="section">
		<h5>Section 3</h5>
		<p>Stuff</p>
	</div>

```

##Создание адаптивной разметки

###Размеры экранов

	1.Mobile Devices <= 600px

	Class Prefix - .s

	Container Width - 85%

	2.Tablet Devices <= 992px

	Class Prefix - .m

	Container Width - 85%

	3.Desktop Devices > 992px

	Class Prefix - .l

	Container Width - 70%

###Адаптивные колонки


```html

	<div class="row">
		<div class="grid-example col s12"><span class="flow-text">I am always full-width (col s12)</span></div>
		<div class="grid-example col s12 m6"><span class="flow-text">I am full-width on mobile (col s12 m6)</span></div>
	</div>

```

```html

	<div class="row">
		<div class="col s12"><p>s12</p></div>
		<div class="col s12 m4 l2"><p>s12 m4</p></div>
		<div class="col s12 m4 l8"><p>s12 m4</p></div>
		<div class="col s12 m4 l2"><p>s12 m4</p></div>
	</div>
	<div class="row">
		<div class="col s12 m6 l3"><p>s12 m6 l3</p></div>
		<div class="col s12 m6 l3"><p>s12 m6 l3</p></div>
		<div class="col s12 m6 l3"><p>s12 m6 l3</p></div>
		<div class="col s12 m6 l3"><p>s12 m6 l3</p></div>
	</div>

```
