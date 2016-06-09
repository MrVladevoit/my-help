# Моя шпаргалка по работе с Materializecss.com

![alt tag](https://scotch.io/wp-content/uploads/2015/01/getting-started-materialize-css-framework.png)

Materializecss.com - это фремворк material designer на SASS.

1. Скачать
 + [Скачать и использовать](#Скачать-и-использовать-materializecsscom);
 + [CDN](#cdn);
 + [Установить с NPM и Bower](#npm-and-bower);

2.Запуск и использование **Materialize**
 + [Запуск](#Запуск-html);
 + [Ruby Gem, Meteor Package, Ember Package](#ruby-gem-meteor-package-ember-package);
 + [Запуск используя sass](#Запуск-используя-sass);

3.Использование Цвета
 + [Цвет фона](#Цвет-фона);
 + [SASS](#sass);

4.Grid / Сетка
 + [Container](#container);
 + [12 колонок](#12-колонок);
 + [Колонки находятся внутри строки](#Колонки-находятся-внутри-строки);
 + [Смещения](#Смещения);
 + [Push and Pull](#push-and-pull);
 + [Создание Макетов](#Создание-Макетов);

5.Создание адаптивной разметки
 + [Размеры экранов](#Размеры-экранов);
 + [Адаптивные колонки](#Адаптивные-колонки);

6.Helpers
 + [Выравнивание по вертикали](#Выравнивание-по-вертикали);
 + [Text Align / Выравнивание текста](#text-align--Выравнивание-текста);
 + [Quick Floats / быстрые обтекания](#quick-floats--быстрые-обтекания);
 + [Hiding Content / прячем контент](#hiding-content--прячем-контент);
 + [Форматирование](#Форматирование);
 + [Анимация тени](#Анимация-тени);

7.Media CSS
 + [Изображения](#Изображения);
 + [Видео](#Видео);

8.SASS
 + [SASS](#sass-1);
 + [Media Queries](#media-queries);
 + [Prefixer](#prefixer);

9.Тени
 + [Использование теней](#Тени);

10.Таблицы
 + [Безграниыные таблицы](#Таблицы);
 + [Таблицы с границей](#Таблицы-с-границей);
 + [Фон строк](#Фон-строк);
 + [Центрированная таблица](#Центрированная-таблица);
 + [Адаптивные таблицы](#Адаптивные-таблицы);

11.Типографика
 + [Roboto](#roboto);
 + [Blockquotes](#blockquotes);

12.Baget / значки уведомлений
 + [Использование badget](#baget--значки-уведомлений);

13.Buttons / Кнопки
 + [Использование button](#buttons--Кнопки);
 + [Округлые кнопки](#Округлые-кнопки);
 + [Fixed Action Button](#fixed-action-button);
 + [Horizontal FAB](#horizontal-fab);
 + [Click-only FAB](#click-only-fab);
 + [Flat](#Flat);
 + [Submit Button](#submit-button);
 + [Большие](#Большие);
 + [Disabled](#Disabled);

14.Breadcrumbs / Хлебные крошки
 + [Использование Breadcrumbs](#breadcrumbs--Хлебные-крошки);

15.Cards / Карточки
 + [Стандартная карточка](#Стандартная-карточка);
 + [Карточка с images](#Карточка с images);
 + [Card Reveal / Анимация карточки](#card-reveal--Анимация-карточки);

16.Chips / tags
 + [Contacts](#Contacts);
 + [Tags](#Tags);

17.Collections
 + [Использование Collections](#Collections);
 + [Avatar Content](#avatar-content);

18.Footer
 + [Использование Footer](#Footer);
 + [Прилипающий футер](#Прилипающий-футер);

19.Form / Формы
 + [Inputs](#input-fields);
 + [Icon Prefixes / использование иконок](#icon-prefixes--использование-иконок);
 + [Собственные ошибки и сообщения](#Собственные-ошибки-и-сообщения);
 + [Select](#select);
 + [Radio Buttons](#radio-buttons);
 + [Чекбоксы](#Чекбоксы);
 + [Switches](#switches);
 + [File Input](#file-input);
 + [Range](#range);
 + [Date Picker](#date-picker);
 + [Счетчик символов](#Счетчик-символов);

20.Icons / Иконки
 + [Использование Icons](#icons--Иконки);

21.Navbar / меню
 + [Ссылки справа](#Ссылки-справа);
 + [Ссылки слева](#Ссылки-слева);
 + [Центрирование лого](#Центрирование-лого);
 + [Fixed](#Зафиксированная-панель-навигации);
 + [Выпадающее меню на панели навигации](#Выпадающее-меню-на-панели-навигации);
 + [Мобильное меню](#Мобильное-меню);

22.Pagination
 + [Использование Pagination](#pagination);

23.Preloader
 + [Linear - progress bar](#linear---progress-bar);
 + [Циркулярный](#Циркулярный);
 + [Circular Flashing Colors / Смешенные цвета](#circular-flashing-colors--Смешенные-цвета);

24.Collapsible
 + [Collapsible](#collapsible);

25.Dialogs
 + [Toasts](#toasts);
 + [Tooltips](#tooltips);

26.Dropdown
 + [Dropdown - выпадающее списки](#dropdown);
 + [Tooltips](#tooltips);
 + [Настройки](#Настройки);
 + [jQuery Plugin Initialization](#jquery-plugin-initialization);

27.Media : Zoom image, SLIDER, CAROUSEL
 + [Material Box](#material-box);
 + [Slider](#slider);
 + [Carousel](#carousel);

28.Modals
 + [Использование modals](#modals);
 + [Настройки](#Настройки-1);

29.Parallax
 + [Использование Parallax](#parallax);
 + [Demo](#demo);

30.ScrollFire / Transitions
 + [Использование ScrollFire](#scrollFire);
 + [Использование Transitions](#transitions);

31.Scrollspy
 + [Использование Scrollspy](#scrollspy);

32.Tabs / Табы
 + [Использование Tabs / Табы](#tabs--Табы);


33.Waves / Волна
 + [Применение волн](#Применение-волн);
 + [Нестандартные цвета](#Нестандартные-цвета);
 + [Circle](#circle);

## Скачать и использовать Materializecss.com

Для того, чтобы начать переходим по ссылке : [http://materializecss.com/getting-started.html](http://materializecss.com/getting-started.html)

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

###Колонки находятся внутри строки

Помните, когда вы создаете макет, следует все столбцы добавлять в строки.

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

*1.Mobile Devices <= 600px*

Class Prefix - .s

Container Width - 85%

*2.Tablet Devices <= 992px*

Class Prefix - .m

Container Width - 85%

*3.Desktop Devices > 992px*

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

##Helpers

###Выравнивание по вертикали

Для выравнивания по вертикали достаточно добавить класс valign-wrapper

```html

	<div class="valign-wrapper">
		<h5 class="valign">This should be vertically aligned</h5>
	</div>

```

###Text Align / Выравнивание текста

Для выравнивания текста и используем классы .left-align, .right-align and .center-align

```html

	<div>
		<h5 class="left-align">This should be left aligned</h5>
	</div>
	<div>
		<h5 class="right-align">This should be right aligned</h5>
	</div>
	<div>
		<h5 class="center-align">This should be center aligned</h5>
	</div>

```

###Quick Floats / быстрые обтекания

```html

	<div class="left">...</div>
	<div class="right">...</div>

```

###Hiding Content / прячем контент

**.hide** - скрыть на всех устройствах
**.hide-on-small-only** - скрыть только на мобильных.
**.hide-on-med-only** - скрыть на планшетах.
**.hide-on-med-and-down** - скрыть на планшетах и устройствах с экраном меньше чем у планшетов.
**.hide-on-med-and-up** - скрыть на планшетах и устройствах с экраном больше чем у планшетов.
**.hide-on-large-only** - скрыть только на Destop.

###Форматирование

Если текст не влизает в контейнер, достаточно добавить класс **truncate**, и тогда мы увидм на конце такой результат.

```html

	<h4 class="truncate">This is an extremely long title that will be truncated</h4>

```

Результат : This is an extremely long title that will be ...

###Анимация тени

```html

	<div class="card-panel hoverable"> Hoverable Card Panel</div>

```

##Media CSS

###Изображения

**Адаптивные изображения** - добавляем класс **.responsive-img** - для стилей адаптивных картинок **max-width: 100%** и **height:auto**.

**Скругленные изображения** - **class="circle"**.

###Видео

Исользуем класс **.video-container** для контейнера видео.

```html

	 <div class="video-container">
		<iframe width="853" height="480" src="//www.youtube.com/embed/Q8TXgCzxEnw?rel=0" frameborder="0" allowfullscreen></iframe>
	</div>

```
Для адаптивности видео используем **.responsive-video**.

##SASS

###Переменные

Чтобы заменить цветовую схему на стайте достатоно уже заменить значения в файле _variables.scss.

```SASS

	$primary-color: color("materialize-red", "lighten-2") !default;
	$primary-color-light: false !default;
	$primary-color-dark: false !default;
	@if not $primary-color-light {
		$primary-color-light: lighten($primary-color, 15%);
	}
	@if not $primary-color-dark {
		$primary-color-dark: darken($primary-color, 15%);
	}
	$secondary-color: color("teal", "lighten-1") !default;
	$success-color: color("green", "base") !default;
	$error-color: color("red", "base") !default;

	$link-color: color("light-blue", "darken-1") !default;

	/*** More variables not shown here.. ***/

```

###Media Queries

Маленькие экраны определены как имеющие максимальную ширину в 600px Средние экраны определяются как имеющие максимальную ширину в 992px Большой экран определены как имеющие мин ширину 993px

```SASS

 @media #{$small-and-down} {
    // styles for small screens and down
  }
  @media #{$medium-and-up} {
    // styles for medium screens and larger
  }
  @media #{$medium-and-down} {
    // styles for medium screens and down
  }
  @media #{$large-and-up} {
    // styles for large screens and up
  }

```

###Prefixer

Мы можем использовать встроенные миксины автопрефиксов

В SASS:

```SASS

	@include transition(.3s);

```

Получим в CSS:

```css

	-webkit-transition: 0.3s;
	  -moz-transition: 0.3s;
	  -o-transition: 0.3s;
	  -ms-transition: 0.3s;
	  transition: 0.3s;

```

Все миксины:

```SASS

animation($args)
  animation-delay($delay)
  animation-direction($direction)
  animation-duration($duration)
  animation-fill-mode($mode)
  animation-iteration-count($count)
  animation-name($name)
  animation-play-state($state)
  animation-timing-function($function)
  background-size($args)
  box-sizing($args)
      border-box()
      content-box()
  columns($args)
      column-count($count)
      column-gap($gap)
      column-rule($args)
      column-width($width)
  gradient($default,$start,$stop)
      linear-gradient-top($default,$color1,$stop1,$color2,$stop2,[$color3,$stop3,$color4,$stop4])
      linear-gradient-left($default,$color1,$stop1,$color2,$stop2,[$color3,$stop3,$color4,$stop4])
  transform($args)
      transform-origin($args)
      transform-style($style)
      rotate($deg)
      scale($factor)
      translate($x,$y)
      translate3d($x,$y,$z)
      translateHardware($x,$y)
  text-shadow($args)
  transition($args)
      transition-delay($delay)
      transition-duration($duration)
      transition-property($property)
      transition-timing-function($function)

```

##Тени

Для тени мы используем **class="z-depth-2"** или @extend в SASS. z-depth - обозначает глубину.

```html

	<div class="col s12 m2">
		<p class="z-depth-1">z-depth-1</p>
	</div>
	<div class="col s12 m2">
		<p class="z-depth-2">z-depth-2</p>
	</div>
	<div class="col s12 m2">
		<p class="z-depth-3">z-depth-3</p>
	</div>
	<div class="col s12 m2">
		<p class="z-depth-4">z-depth-4</p>
	</div>
	<div class="col s12 m2">
		<p class="z-depth-5">z-depth-5</p>
	</div>

```

##Таблицы

###Безграниыные таблицы

Эти таблицы используются по умолчанию.

```html

	<table>
		<thead>
			<tr>
				<th data-field="id">Name</th>
				<th data-field="name">Item Name</th>
				<th data-field="price">Item Price</th>
			</tr>
		</thead>

		<tbody>
			<tr>
				<td>Alvin</td>
				<td>Eclair</td>
				<td>$0.87</td>
			</tr>
			<tr>
				<td>Alan</td>
				<td>Jellybean</td>
				<td>$3.76</td>
			</tr>
			<tr>
				<td>Jonathan</td>
				<td>Lollipop</td>
				<td>$7.00</td>
			</tr>
		</tbody>
	</table>

```

###Таблицы с границей

Для границ нужно добавить **class="bordered"** к таблице.

###Фон строк

Нужно добавить **class="striped"** к таблице.

###Подсвечивание строк таблицы при наведении

Нужно добавить **class="highlight"** к таблице. При hover, подсвечивается строка таблицы.

###Центрированная таблица

Нужно добавить **class="centered"** к таблице.

###Адаптивные таблицы

Добавить класс = **"responsive-table"** к таблице тегов, чтобы сделать таблицу адаптивной.На мобильных устройствах появляется скролл горизонтальный.

##Типографика

###Roboto

Стандартный шрифт для Материального дизайна - Roboto. Мы включили файлы шрифта в наш фреймворк.
Удаление шрифта Roboto происходит заменной стилей тега html:

```html

	html {
		font-family: GillSans, Calibri, Trebuchet, sans-serif;
	}

```

###Blockquotes

```html

	<blockquote>
      This is an example quotation that uses the blockquote tag.
    </blockquote>

```

###Flow Text / проточный текст

```html

	<p class="flow-text">I am Flow Text</p>

```

##Baget / значки уведомлений

[Прочитать и посмотреть пример](http://materializecss.com/badges.html);


```html

	<div class="collection">
		<a href="#!" class="collection-item">Alan<span class="badge">1</span></a>
		<a href="#!" class="collection-item">Alan<span class="new badge">4</span></a>
		<a href="#!" class="collection-item">Alan</a>
		<a href="#!" class="collection-item">Alan<span class="badge">14</span></a>
	</div>

```
Badget добавляется так же и в выпадающие списки Dropdown, и в Navbar.

##Buttons / Кнопки

[Прочитать и посмотреть пример](http://materializecss.com/buttons.html);

Кнопки могут быть и с иконками material design:

```html

	<a class="waves-effect waves-light btn">button</a>
	<a class="waves-effect waves-light btn"><i class="material-icons left">cloud</i>button</a>
	<a class="waves-effect waves-light btn"><i class="material-icons right">cloud</i>button</a>

```
###Округлые кнопки

```html

	<a class="btn-floating btn-large waves-effect waves-light red"><i class="material-icons">add</i></a>

```

###Fixed Action Button

Кнопка с фиксированным положением, в которой есть еще кнопки с дополнительными действиями.

```html

	<div class="fixed-action-btn" style="bottom: 45px; right: 24px;">
	    <a class="btn-floating btn-large red">
	      <i class="large material-icons">mode_edit</i>
	    </a>
	    <ul>
	      <li><a class="btn-floating red"><i class="material-icons">insert_chart</i></a></li>
	      <li><a class="btn-floating yellow darken-1"><i class="material-icons">format_quote</i></a></li>
	      <li><a class="btn-floating green"><i class="material-icons">publish</i></a></li>
	      <li><a class="btn-floating blue"><i class="material-icons">attach_file</i></a></li>
	    </ul>
	  </div>

````

```js

	$('.fixed-action-btn').openFAB();

```
```js

	$('.fixed-action-btn').closeFAB();

```

###Horizontal FAB

```html

	<div class="fixed-action-btn horizontal" style="bottom: 45px; right: 24px;">
	    <a class="btn-floating btn-large red">
	      <i class="large material-icons">mode_edit</i>
	    </a>
	    <ul>
	      <li><a class="btn-floating red"><i class="material-icons">insert_chart</i></a></li>
	      <li><a class="btn-floating yellow darken-1"><i class="material-icons">format_quote</i></a></li>
	      <li><a class="btn-floating green"><i class="material-icons">publish</i></a></li>
	      <li><a class="btn-floating blue"><i class="material-icons">attach_file</i></a></li>
	    </ul>
	  </div>

```
###Click-only FAB

```html

	<div class="fixed-action-btn horizontal click-to-toggle" style="bottom: 45px; right: 24px;">
		<a class="btn-floating btn-large red">
		  <i class="material-icons">menu</i>
		</a>
		<ul>
		  <li><a class="btn-floating red"><i class="material-icons">insert_chart</i></a></li>
		  <li><a class="btn-floating yellow darken-1"><i class="material-icons">format_quote</i></a></li>
		  <li><a class="btn-floating green"><i class="material-icons">publish</i></a></li>
		  <li><a class="btn-floating blue"><i class="material-icons">attach_file</i></a></li>
		</ul>
	</div>

```

###Flat

Прозрачные кнопки используются для уменьшения чрезмерного наслоения. Например, эти кнопки, как правило, используются для действий внутри **card** или **modal**, так чтобы было не слишком много перекрывающихся теней.

```html

	<a class="waves-effect waves-teal btn-flat">Button</a>

```

###Submit Button

```html

	<button class="btn waves-effect waves-light" type="submit" name="action">Submit
		<i class="material-icons right">send</i>
	</button>

```

###Большие

```html

	<a class="waves-effect waves-light btn-large">Button</a>
	<a class="waves-effect waves-light btn-large"><i class="material-icons left">cloud</i>button</a>
	<a class="waves-effect waves-light btn-large"><i class="material-icons right">cloud</i>button</a>

```

###Disabled

```html

	<a class="btn-large disabled">Button</a>
	<a class="btn disabled">Button</a>
	<a class="btn-flat disabled">Button</a>
	<a class="btn-floating disabled"><i class="material-icons">add</i></a>

```

##Breadcrumbs / Хлебные крошки

```html

  <nav>
    <div class="nav-wrapper">
      <div class="col s12">
        <a href="#!" class="breadcrumb">First</a>
        <a href="#!" class="breadcrumb">Second</a>
        <a href="#!" class="breadcrumb">Third</a>
      </div>
    </div>
  </nav>


```

##Cards / Карточки

[Прочитать и посмотреть пример](http://materializecss.com/cards.html);

###Стандартная карточка

```html

      <div class="row">
        <div class="col s12 m6">
          <div class="card blue-grey darken-1">
            <div class="card-content white-text">
              <span class="card-title">Card Title</span>
              <p>I am a very simple card. I am good at containing small bits of information.
              I am convenient because I require little markup to use effectively.</p>
            </div>
            <div class="card-action">
              <a href="#">This is a link</a>
              <a href="#">This is a link</a>
            </div>
          </div>
        </div>
      </div>

```

###Карточка с images


```html

      <div class="row">
        <div class="col s12 m7">
          <div class="card">
            <div class="card-image">
              <img src="images/sample-1.jpg">
              <span class="card-title">Card Title</span>
            </div>
            <div class="card-content">
              <p>I am a very simple card. I am good at containing small bits of information.
              I am convenient because I require little markup to use effectively.</p>
            </div>
            <div class="card-action">
              <a href="#">This is a link</a>
            </div>
          </div>
        </div>
      </div>

```

###Card Reveal / Анимация карточки


```html

 <div class="card">
    <div class="card-image waves-effect waves-block waves-light">
      <img class="activator" src="images/office.jpg">
    </div>
    <div class="card-content">
      <span class="card-title activator grey-text text-darken-4">Card Title<i class="material-icons right">more_vert</i></span>
      <p><a href="#">This is a link</a></p>
    </div>
    <div class="card-reveal">
      <span class="card-title grey-text text-darken-4">Card Title<i class="material-icons right">close</i></span>
      <p>Here is some more information about this product that is only revealed once clicked on.</p>
    </div>
  </div>

```

###Размеры карточки

**Small**, **Medium**, **Large**

```html

	<div class="card small">
		<!-- Card Content -->
	</div>

```

###Card Panel

```html

   <div class="row">
      <div class="col s12 m5">
        <div class="card-panel teal">
          <span class="white-text">I am a very simple card. I am good at containing small bits of information.
          I am convenient because I require little markup to use effectively. I am similar to what is called a panel in other frameworks.
          </span>
        </div>
      </div>
    </div>

```

##Chips

Chips следует использовать для тегов и их удаления.

###Contacts


```html

  <div class="chip">
    <img src="images/yuna.jpg" alt="Contact Person">
    Jane Doe
  </div>

```

###Tags


```html

  <div class="chip">
    Tag
    <i class="material-icons">close</i>
  </div>

```

##Collections

Колекции позволяют объеденить список групп вместе.

[Прочитать и посмотреть пример](http://materializecss.com/collections.html);


```html

    <ul class="collection">
      <li class="collection-item">Alvin</li>
      <li class="collection-item">Alvin</li>
      <li class="collection-item">Alvin</li>
      <li class="collection-item">Alvin</li>
    </ul>

```

###Avatar Content

```html

  <ul class="collection">
    <li class="collection-item avatar">
      <img src="images/yuna.jpg" alt="" class="circle">
      <span class="title">Title</span>
      <p>First Line <br>
         Second Line
      </p>
      <a href="#!" class="secondary-content"><i class="material-icons">grade</i></a>
    </li>
    <li class="collection-item avatar">
      <i class="material-icons circle">folder</i>
      <span class="title">Title</span>
      <p>First Line <br>
         Second Line
      </p>
      <a href="#!" class="secondary-content"><i class="material-icons">grade</i></a>
    </li>
    <li class="collection-item avatar">
      <i class="material-icons circle green">insert_chart</i>
      <span class="title">Title</span>
      <p>First Line <br>
         Second Line
      </p>
      <a href="#!" class="secondary-content"><i class="material-icons">grade</i></a>
    </li>
    <li class="collection-item avatar">
      <i class="material-icons circle red">play_arrow</i>
      <span class="title">Title</span>
      <p>First Line <br>
         Second Line
      </p>
      <a href="#!" class="secondary-content"><i class="material-icons">grade</i></a>
    </li>
  </ul>

```
##Footer

```html

    <footer class="page-footer">
      <div class="container">
        <div class="row">
          <div class="col l6 s12">
            <h5 class="white-text">Footer Content</h5>
            <p class="grey-text text-lighten-4">You can use rows and columns here to organize your footer content.</p>
          </div>
          <div class="col l4 offset-l2 s12">
            <h5 class="white-text">Links</h5>
            <ul>
              <li><a class="grey-text text-lighten-3" href="#!">Link 1</a></li>
              <li><a class="grey-text text-lighten-3" href="#!">Link 2</a></li>
              <li><a class="grey-text text-lighten-3" href="#!">Link 3</a></li>
              <li><a class="grey-text text-lighten-3" href="#!">Link 4</a></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="footer-copyright">
        <div class="container">
        © 2014 Copyright Text
        <a class="grey-text text-lighten-4 right" href="#!">More Links</a>
        </div>
      </div>
    </footer>

```

###Прилипающий футер

Он не работает в IE, так как использует FlexBox

```css

  body {
    display: flex;
    min-height: 100vh;
    flex-direction: column;
  }

  main {
    flex: 1 0 auto;
  }

```

##Form / Формы

[Прочитать и посмотреть пример](http://materializecss.com/forms.html);

###Input fields

Для импутов используем классы .input-field.Валидания на HTML5 исопльзует такие классы и стили valid, invalid, validate.


```html

  <div class="row">
    <form class="col s12">
      <div class="row">
        <div class="input-field col s6">
          <input placeholder="Placeholder" id="first_name" type="text" class="validate">
          <label for="first_name">First Name</label>
        </div>
        <div class="input-field col s6">
          <input id="last_name" type="text" class="validate">
          <label for="last_name">Last Name</label>
        </div>
      </div>
      <div class="row">
        <div class="input-field col s12">
          <input disabled value="I am not editable" id="disabled" type="text" class="validate">
          <label for="disabled">Disabled</label>
        </div>
      </div>
      <div class="row">
        <div class="input-field col s12">
          <input id="password" type="password" class="validate">
          <label for="password">Password</label>
        </div>
      </div>
      <div class="row">
        <div class="input-field col s12">
          <input id="email" type="email" class="validate">
          <label for="email">Email</label>
        </div>
      </div>
    </form>
  </div>

```

###Icon Prefixes / использование иконок

```html

  <div class="row">
    <form class="col s12">
      <div class="row">
        <div class="input-field col s6">
          <i class="material-icons prefix">account_circle</i>
          <input id="icon_prefix" type="text" class="validate">
          <label for="icon_prefix">First Name</label>
        </div>
        <div class="input-field col s6">
          <i class="material-icons prefix">phone</i>
          <input id="icon_telephone" type="tel" class="validate">
          <label for="icon_telephone">Telephone</label>
        </div>
      </div>
    </form>
  </div>

```

###Собственные ошибки и сообщения

Мы можем добавлять пользовательское сообщение ошибки или успеха ввода данных - **data-error** или **data-success**.

```html

  <div class="row">
    <form class="col s12">
      <div class="row">
        <div class="input-field col s12">
          <input id="email" type="email" class="validate">
          <label for="email" data-error="wrong" data-success="right">Email</label>
        </div>
      </div>
    </form>
  </div>

```

###Select

```html

  <div class="input-field col s12">
    <select>
      <option value="" disabled selected>Choose your option</option>
      <option value="1">Option 1</option>
      <option value="2">Option 2</option>
      <option value="3">Option 3</option>
    </select>
    <label>Materialize Select</label>
  </div>

  <div class="input-field col s12">
    <select multiple>
      <option value="" disabled selected>Choose your option</option>
      <option value="1">Option 1</option>
      <option value="2">Option 2</option>
      <option value="3">Option 3</option>
    </select>
    <label>Materialize Multiple Select</label>
  </div>

  <div class="input-field col s12">
    <select multiple>
      <optgroup label="team 1">
        <option value="1">Option 1</option>
        <option value="2">Option 2</option>
      </optgroup>
      <optgroup label="team 2">
        <option value="3">Option 3</option>
        <option value="4">Option 4</option>
      </optgroup>
    </select>
    <label>Optgroups</label>
  </div>

  <div class="input-field col s12 m6">
    <select class="icons">
      <option value="" disabled selected>Choose your option</option>
      <option value="" data-icon="images/sample-1.jpg" class="circle">example 1</option>
      <option value="" data-icon="images/office.jpg" class="circle">example 2</option>
      <option value="" data-icon="images/yuna.jpg" class="circle">example 1</option>
    </select>
    <label>Images in select</label>
  </div>
  <div class="input-field col s12 m6">
    <select class="icons">
      <option value="" disabled selected>Choose your option</option>
      <option value="" data-icon="images/sample-1.jpg" class="left circle">example 1</option>
      <option value="" data-icon="images/office.jpg" class="left circle">example 2</option>
      <option value="" data-icon="images/yuna.jpg" class="left circle">example 3</option>
    </select>
    <label>Images in select</label>
  </div>

  <label>Browser Select</label>
  <select class="browser-default">
    <option value="" disabled selected>Choose your option</option>
    <option value="1">Option 1</option>
    <option value="2">Option 2</option>
    <option value="3">Option 3</option>
  </select>

```
```js

$(document).ready(function() {
    $('select').material_select();
  });

```

###Radio Buttons

```html

 <form action="#">
    <p>
      <input name="group1" type="radio" id="test1" />
      <label for="test1">Red</label>
    </p>
    <p>
      <input name="group1" type="radio" id="test2" />
      <label for="test2">Yellow</label>
    </p>
    <p>
      <input class="with-gap" name="group1" type="radio" id="test3"  />
      <label for="test3">Green</label>
    </p>
      <p>
        <input name="group1" type="radio" id="test4" disabled="disabled" />
        <label for="test4">Brown</label>
    </p>
  </form>

```

###Чекбоксы

```html

  <form action="#">
    <p>
      <input type="checkbox" id="test5" />
      <label for="test5">Red</label>
    </p>
    <p>
      <input type="checkbox" id="test6" checked="checked" />
      <label for="test6">Yellow</label>
    </p>
    <p>
      <input type="checkbox" class="filled-in" id="filled-in-box" checked="checked" />
      <label for="filled-in-box">Filled in</label>
    </p>
    <p>
      <input type="checkbox" id="indeterminate-checkbox" />
      <label for="indeterminate-checkbox">Indeterminate Style</label>
    </p>
    <p>
      <input type="checkbox" id="test7" checked="checked" disabled="disabled" />
      <label for="test7">Green</label>
    </p>
      <p>
        <input type="checkbox" id="test8" disabled="disabled" />
        <label for="test8">Brown</label>
    </p>
  </form>

```

###Switches

```html

  <!-- Switch -->
  <div class="switch">
    <label>
      Off
      <input type="checkbox">
      <span class="lever"></span>
      On
    </label>
  </div>

  <!-- Disabled Switch -->
  <div class="switch">
    <label>
      Off
      <input disabled type="checkbox">
      <span class="lever"></span>
      On
    </label>
  </div>

```

###File Input

```html

  <form action="#">
    <div class="file-field input-field">
      <div class="btn">
        <span>File</span>
        <input type="file">
      </div>
      <div class="file-path-wrapper">
        <input class="file-path validate" type="text">
      </div>
    </div>
  </form>

```

###Range

```js

  var slider = document.getElementById('test5');
  noUiSlider.create(slider, {
   start: [20, 80],
   connect: true,
   step: 1,
   range: {
     'min': 0,
     'max': 100
   },
   format: wNumb({
     decimals: 0
   })
  });

```

**HTML5 Range**

```html

  <form action="#">
    <p class="range-field">
      <input type="range" id="test5" min="0" max="100" />
    </p>
  </form>

```

###Date Picker

```html

	<input type="date" class="datepicker">

```

```js

  $('.datepicker').pickadate({
    selectMonths: true, // Creates a dropdown to control month
    selectYears: 15 // Creates a dropdown of 15 years to control year
  });

```

###Счетчик символов

```html

    <div class="row">
      <form class="col s12">
        <div class="row">
          <div class="input-field col s6">
            <input id="input_text" type="text" length="10">
            <label for="input_text">Input text</label>
          </div>
        </div>
        <div class="row">
          <div class="input-field col s12">
            <textarea id="textarea1" class="materialize-textarea" length="120"></textarea>
            <label for="textarea1">Textarea</label>
          </div>
        </div>
      </form>
    </div>

```

```js

  $(document).ready(function() {
    $('input#input_text, textarea#textarea1').characterCounter();
  });

```

##Icons / Иконки

Подключение :

```html

 <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">

````

Используем html:

```html

	<i class="material-icons">add</i>

```

##Navbar

[Прочитать и посмотреть пример](http://materializecss.com/navbar.html);

###Ссылки справа

```html

  <nav>
    <div class="nav-wrapper">
      <a href="#" class="brand-logo">Logo</a>
      <ul id="nav-mobile" class="right hide-on-med-and-down">
        <li><a href="sass.html">Sass</a></li>
        <li><a href="badges.html">Components</a></li>
        <li><a href="collapsible.html">JavaScript</a></li>
      </ul>
    </div>
  </nav>

```

###Ссылки слева

```html

  <nav>
    <div class="nav-wrapper">
      <a href="#" class="brand-logo right">Logo</a>
      <ul id="nav-mobile" class="left hide-on-med-and-down">
        <li><a href="sass.html">Sass</a></li>
        <li><a href="badges.html">Components</a></li>
        <li><a href="collapsible.html">JavaScript</a></li>
      </ul>
    </div>
  </nav>

```

###Центрирование лого

```html

  <nav>
    <div class="nav-wrapper">
      <a href="#" class="brand-logo center">Logo</a>
      <ul id="nav-mobile" class="left hide-on-med-and-down">
        <li><a href="sass.html">Sass</a></li>
        <li><a href="badges.html">Components</a></li>
        <li><a href="collapsible.html">JavaScript</a></li>
      </ul>
    </div>
  </nav>

```

###Активные списки меню

Для активной ссылки в меню достаточно добавить class **li.active**.

[Прочитать и посмотреть пример](http://materializecss.com/navbar.html);

###Зафиксированная панель навигации

Для фиксации меню достаточно добавить class **navbar-fixed**.




###Выпадающее меню на панели навигации

По умолчанию выпдающие меню срабатывает при **hover**, чтобы отключить нужно прописать { hover: false } в  dropdown() function.

```html

	<!-- Dropdown Structure -->
	<ul id="dropdown1" class="dropdown-content">
	  <li><a href="#!">one</a></li>
	  <li><a href="#!">two</a></li>
	  <li class="divider"></li>
	  <li><a href="#!">three</a></li>
	</ul>
	<nav>
	  <div class="nav-wrapper">
	    <a href="#!" class="brand-logo">Logo</a>
	    <ul class="right hide-on-med-and-down">
	      <li><a href="sass.html">Sass</a></li>
	      <li><a href="badges.html">Components</a></li>
	      <!-- Dropdown Trigger -->
	      <li><a class="dropdown-button" href="#!" data-activates="dropdown1">Dropdown<i class="material-icons right">arrow_drop_down</i></a></li>
	    </ul>
	  </div>
	</nav>

```

```js

	$(".dropdown-button").dropdown();

```

###Поисковая строка

Вы можете добавить поисковую форму в блок навигации.

```html

  <nav>
    <div class="nav-wrapper">
      <form>
        <div class="input-field">
          <input id="search" type="search" required>
          <label for="search"><i class="material-icons">search</i></label>
          <i class="material-icons">close</i>
        </div>
      </form>
    </div>
  </nav>

```

###Мобильное меню

[Прочитать и посмотреть пример](http://materializecss.com/navbar.html);

```html

  <nav>
    <div class="nav-wrapper">
      <a href="#!" class="brand-logo">Logo</a>
      <a href="#" data-activates="mobile-demo" class="button-collapse"><i class="material-icons">menu</i></a>
      <ul class="right hide-on-med-and-down">
        <li><a href="sass.html">Sass</a></li>
        <li><a href="badges.html">Components</a></li>
        <li><a href="collapsible.html">Javascript</a></li>
        <li><a href="mobile.html">Mobile</a></li>
      </ul>
      <ul class="side-nav" id="mobile-demo">
        <li><a href="sass.html">Sass</a></li>
        <li><a href="badges.html">Components</a></li>
        <li><a href="collapsible.html">Javascript</a></li>
        <li><a href="mobile.html">Mobile</a></li>
      </ul>
    </div>
  </nav>

```

```js

	$(".button-collapse").sideNav()

```

##Pagination

```html

  <ul class="pagination">
    <li class="disabled"><a href="#!"><i class="material-icons">chevron_left</i></a></li>
    <li class="active"><a href="#!">1</a></li>
    <li class="waves-effect"><a href="#!">2</a></li>
    <li class="waves-effect"><a href="#!">3</a></li>
    <li class="waves-effect"><a href="#!">4</a></li>
    <li class="waves-effect"><a href="#!">5</a></li>
    <li class="waves-effect"><a href="#!"><i class="material-icons">chevron_right</i></a></li>
  </ul>

```

##Preloader

[Прочитать и посмотреть пример](http://materializecss.com/preloader.html);

###Linear - progress bar

** Determinate **

```html

  <div class="progress">
      <div class="determinate" style="width: 70%"></div>
  </div>

```

** Indeterminate **

```html

  <div class="progress">
      <div class="indeterminate"></div>
  </div>

```

###Циркулярный

```html

 <div class="preloader-wrapper big active">
    <div class="spinner-layer spinner-blue-only">
      <div class="circle-clipper left">
        <div class="circle"></div>
      </div><div class="gap-patch">
        <div class="circle"></div>
      </div><div class="circle-clipper right">
        <div class="circle"></div>
      </div>
    </div>
  </div>

  <div class="preloader-wrapper active">
    <div class="spinner-layer spinner-red-only">
      <div class="circle-clipper left">
        <div class="circle"></div>
      </div><div class="gap-patch">
        <div class="circle"></div>
      </div><div class="circle-clipper right">
        <div class="circle"></div>
      </div>
    </div>
  </div>

  <div class="preloader-wrapper small active">
    <div class="spinner-layer spinner-green-only">
      <div class="circle-clipper left">
        <div class="circle"></div>
      </div><div class="gap-patch">
        <div class="circle"></div>
      </div><div class="circle-clipper right">
        <div class="circle"></div>
      </div>
    </div>
  </div>

```

###Circular Flashing Colors / Смешенные цвета

```html

 <div class="preloader-wrapper big active">
      <div class="spinner-layer spinner-blue">
        <div class="circle-clipper left">
          <div class="circle"></div>
        </div><div class="gap-patch">
          <div class="circle"></div>
        </div><div class="circle-clipper right">
          <div class="circle"></div>
        </div>
      </div>

      <div class="spinner-layer spinner-red">
        <div class="circle-clipper left">
          <div class="circle"></div>
        </div><div class="gap-patch">
          <div class="circle"></div>
        </div><div class="circle-clipper right">
          <div class="circle"></div>
        </div>
      </div>

      <div class="spinner-layer spinner-yellow">
        <div class="circle-clipper left">
          <div class="circle"></div>
        </div><div class="gap-patch">
          <div class="circle"></div>
        </div><div class="circle-clipper right">
          <div class="circle"></div>
        </div>
      </div>

      <div class="spinner-layer spinner-green">
        <div class="circle-clipper left">
          <div class="circle"></div>
        </div><div class="gap-patch">
          <div class="circle"></div>
        </div><div class="circle-clipper right">
          <div class="circle"></div>
        </div>
      </div>
    </div>

```

##Collapsible

Collapsible используется для того, чтобы скрыть/показать контент при клике

[Прочитать и посмотреть пример](http://materializecss.com/collapsible.html);

HTML - Структура:

```html

  <ul class="collapsible" data-collapsible="accordion">
    <li>
      <div class="collapsible-header"><i class="material-icons">filter_drama</i>First</div>
      <div class="collapsible-body"><p>Lorem ipsum dolor sit amet.</p></div>
    </li>
    <li>
      <div class="collapsible-header"><i class="material-icons">place</i>Second</div>
      <div class="collapsible-body"><p>Lorem ipsum dolor sit amet.</p></div>
    </li>
    <li>
      <div class="collapsible-header"><i class="material-icons">whatshot</i>Third</div>
      <div class="collapsible-body"><p>Lorem ipsum dolor sit amet.</p></div>
    </li>
  </ul>

```

```js

  $(document).ready(function(){
    $('.collapsible').collapsible({
      accordion : false // A setting that changes the collapsible behavior to expandable instead of the default accordion style
    });
  });

```

###Аккордион и Expandable

Используется 2 вида меню Collapsible:

**Аккордион**

```html

  <ul class="collapsible" data-collapsible="accordion">

```

**Expandable**

```html

  <ul class="collapsible" data-collapsible="expandable">

```

##Dialogs

[Прочитать и посмотреть пример](http://materializecss.com/dialogs.html);

###Toasts

Очень удобные тосты для отправки сообщения пользователю.

```js

 // Materialize.toast(message, displayLength, className, completeCallback);
  Materialize.toast('I am a toast!', 4000) // 4000 is the duration of the toast

```

```html

 <a class="btn" onclick="Materialize.toast('I am a toast', 4000)">Toast!</a>

```

####Custom HTML

```js

  var $toastContent = $('<span>I am toast content</span>');
  Materialize.toast($toastContent, 5000);

```

####Callback

```html

	<a class="btn" onclick="Materialize.toast('I am a toast', 4000,'',function(){alert('Your toast was dismissed')})">Toast!</a>

```

####Styling Toasts

```js

	Materialize.toast('I am a toast!', 3000, 'rounded') // 'rounded' is the class I'm applying to the toast

```

###Tooltips

```html

	<!-- data-position can be : bottom, top, left, or right -->
	<!-- data-delay controls delay before tooltip shows (in milliseconds)-->
	<a class="btn tooltipped" data-position="bottom" data-delay="50" data-tooltip="I am tooltip">Hover me!</a>

```
```js

  $(document).ready(function(){
    $('.tooltipped').tooltip({delay: 50});
  });

```

**Removal**

```js

  // This will remove the tooltip functionality for the buttons on this page
  $('.tooltipped').tooltip('remove');

```

##Dropdown

Чтобы добавить выпдающий список для кнопки, добавим **data-activates** в **ul** tag. Для разделителей **class="divider"**.

```html

  <!-- Dropdown Trigger -->
  <a class='dropdown-button btn' href='#' data-activates='dropdown1'>Drop Me!</a>

  <!-- Dropdown Structure -->
  <ul id='dropdown1' class='dropdown-content'>
    <li><a href="#!">one</a></li>
    <li><a href="#!">two</a></li>
    <li class="divider"></li>
    <li><a href="#!">three</a></li>
  </ul>

```

###Настройки

	**Появление** (induration) - указываем продолжительность для появления в миллисикундах. Default:300

	**Изчезание** (outduration) - указываем продолжительность для изчезания в миллисикундах. Default:225

	**Constrainwidth** - выпдающий список равен по ширине кнопки.Default:true

	**Hover** - выпдающий список при **hover**.Default:false

	**Gutter** - это определяет расстояние от края выровненного.Default:0

	**Beloworigin** - это определяет будет ли выпдающий список показан ниже кнопки.Default:false

	**Alignment** - выпадающее меню выровнено по умолчанию "По левому краю".Default:'left'

###jQuery Plugin Initialization

```js

  $('.dropdown-button').dropdown({
      inDuration: 300,
      outDuration: 225,
      constrain_width: false, // Does not change width of dropdown to that of the activator
      hover: true, // Activate on hover
      gutter: 0, // Spacing from edge
      belowOrigin: false, // Displays dropdown below the button
      alignment: 'left' // Displays dropdown with edge aligned to the left of button
    }
  );

```

##Media : Zoom image, SLIDER, CAROUSEL

###Material Box

[Прочитать и посмотреть пример](http://materializecss.com/media.html)

**Material Box** представляет собой реализацию материал дизайна плагина **Lightbox**. Когда пользователь нажимает на изображение, оно увеличивается. **Material Box** центрирует изображение и увеличивает его в модальном окне. Чтобы закрыть изображение, пользователь может либо нажать на изображение снова, прокрутите в сторону, или нажать клавишу **ESC**.

```html

	<img class="materialboxed" width="650" src="images/sample-1.jpg">

```
```js

  $(document).ready(function(){
    $('.materialboxed').materialbox();
  });

```

####Подписи

Подписи изображений задаются через атрибут **data-caption**.

```html

	<img class="materialboxed" data-caption="A picture of some deer and tons of trees" width="250" src="http://th01.deviantart.net/fs70/PRE/i/2013/126/1/e/nature_portrait_by_pw_fotografie-d63tx0n.jpg">

```

###Slider

[Прочитать и посмотреть пример](http://materializecss.com/media.html#slider)

Cлайдер представляет собой простой и элегантный **slider** изображений. Заголовки можно задать, как самостоятельные элементы с анимацией. Внизу добавляется пагинация слайдера.

NOTE: Слайдер использует hummer js для точ скринов

```html

  <div class="slider">
    <ul class="slides">
      <li>
        <img src="http://lorempixel.com/580/250/nature/1"> <!-- random image -->
        <div class="caption center-align">
          <h3>This is our big Tagline!</h3>
          <h5 class="light grey-text text-lighten-3">Here's our small slogan.</h5>
        </div>
      </li>
      <li>
        <img src="http://lorempixel.com/580/250/nature/2"> <!-- random image -->
        <div class="caption left-align">
          <h3>Left Aligned Caption</h3>
          <h5 class="light grey-text text-lighten-3">Here's our small slogan.</h5>
        </div>
      </li>
      <li>
        <img src="http://lorempixel.com/580/250/nature/3"> <!-- random image -->
        <div class="caption right-align">
          <h3>Right Aligned Caption</h3>
          <h5 class="light grey-text text-lighten-3">Here's our small slogan.</h5>
        </div>
      </li>
      <li>
        <img src="http://lorempixel.com/580/250/nature/4"> <!-- random image -->
        <div class="caption center-align">
          <h3>This is our big Tagline!</h3>
          <h5 class="light grey-text text-lighten-3">Here's our small slogan.</h5>
        </div>
      </li>
    </ul>
  </div>

```

###Fullscreen Slider

[Прочитать и посмотреть пример](http://materializecss.com/fullscreen-slider-demo.html)

**jQuery Initialization**

```js

    $(document).ready(function(){
      $('.slider').slider({full_width: true});
    });

```

####jQuery Plugin Options

**Indicators** - индикаторы слайдера. Default: True.

**Height** - высота слайдера. Default: 400.

**Transition** - время анимации плавного перехода слайдов. Default: 500.

**Interval** - время плавного перехода слайдов. Default: 6000.

####jQuery Plugin Methods

Есть методы, чтобы сделать паузу, запуск, переход к следующему или перемещения к предыдущему слайду.

```js

// Pause slider
$('.slider').slider('pause');
// Start slider
$('.slider').slider('start');
// Next slide
$('.slider').slider('next');
// Previous slide
$('.slider').slider('prev');

```

###Carousel

Так же имеется отдельня привлекательная карусель.

[Прочитать и посмотреть пример](http://materializecss.com/media.html#carousel)

```html

  <div class="carousel">
    <a class="carousel-item" href="#one!"><img src="http://lorempixel.com/250/250/nature/1"></a>
    <a class="carousel-item" href="#two!"><img src="http://lorempixel.com/250/250/nature/2"></a>
    <a class="carousel-item" href="#three!"><img src="http://lorempixel.com/250/250/nature/3"></a>
    <a class="carousel-item" href="#four!"><img src="http://lorempixel.com/250/250/nature/4"></a>
    <a class="carousel-item" href="#five!"><img src="http://lorempixel.com/250/250/nature/5"></a>
  </div>

  <div class="carousel carousel-slider">
    <a class="carousel-item" href="#one!"><img src="http://lorempixel.com/800/400/food/1"></a>
    <a class="carousel-item" href="#two!"><img src="http://lorempixel.com/800/400/food/2"></a>
    <a class="carousel-item" href="#three!"><img src="http://lorempixel.com/800/400/food/3"></a>
    <a class="carousel-item" href="#four!"><img src="http://lorempixel.com/800/400/food/4"></a>
  </div>

```

```js

    $(document).ready(function(){
      $('.carousel').carousel();
    });

```

####jQuery Plugin Options

**time_constant** - время перехода. Default: 200

**dist** - перспектива увеличения. Если 0, то все элементы имеют одинаковый размер. Default: -100

**shift (сдвиг)** - установите интервал центрального пункта. Default: 0

**padding** - установить padding между пунктами центра. Default: 0

**full_width** - на всю ширину.Default: false

####jQuery Plugin Methods

```js

// Next slide
$('.carousel').carousel('next');
$('.carousel').carousel('next', [3]); // Move next n times.
// Previous slide
$('.carousel').carousel('prev');
$('.carousel').carousel('prev', [4]); // Move prev n times.

````

##Modals

Используйте модальные окна для сообщения пользователям информации.Для модальной кнопки достаточно добавить id модального окна, для модального окна класс **.modal**, а для кнопки закрытия **.modal-close**

**Modals HTML Structure**

```html

  <!-- Modal Trigger -->
  <a class="waves-effect waves-light btn modal-trigger" href="#modal1">Modal</a>

  <!-- Modal Structure -->
  <div id="modal1" class="modal">
    <div class="modal-content">
      <h4>Modal Header</h4>
      <p>A bunch of text</p>
    </div>
    <div class="modal-footer">
      <a href="#!" class=" modal-action modal-close waves-effect waves-green btn-flat">Agree</a>
    </div>
  </div>


```

**Modals with Fixed Footer**

Для модального окна добавляем класс **.modal-fixed-footer**.

```html

  <!-- Modal Trigger -->
  <a class="modal-trigger waves-effect waves-light btn" href="#modal1">Modal</a>

  <!-- Modal Structure -->
  <div id="modal1" class="modal modal-fixed-footer">
    <div class="modal-content">
      <h4>Modal Header</h4>
      <p>A bunch of text</p>
    </div>
    <div class="modal-footer">
      <a href="#!" class="modal-action modal-close waves-effect waves-green btn-flat ">Agree</a>
    </div>
  </div>


```

**Bottom Sheet Modals**

Модальные окна , прилпающие к низу.

Bottom Sheet Modals

```html

  <!-- Modal Trigger -->
  <a class="waves-effect waves-light btn modal-trigger" href="#modal1">Modal</a>

  <!-- Modal Structure -->
  <div id="modal1" class="modal bottom-sheet">
    <div class="modal-content">
      <h4>Modal Header</h4>
      <p>A bunch of text</p>
    </div>
    <div class="modal-footer">
      <a href="#!" class=" modal-action modal-close waves-effect waves-green btn-flat">Agree</a>
    </div>
  </div>

```
**Modals with Button trigger**

```html

 <!-- Modal Trigger -->
  <button data-target="modal1" class="btn modal-trigger">Modal</button>

```

**jQuery Plugin Initialization**

```js

  $(document).ready(function(){
    // the "href" attribute of .modal-trigger must specify the modal ID that wants to be triggered
    $('.modal-trigger').leanModal();
  });

```

```js

 $('#modal1').openModal();

```
```js

	$('#modal1').closeModal();

```

####Настройки

```js

  $('.modal-trigger').leanModal({
      dismissible: true, // Modal can be dismissed by clicking outside of the modal
      opacity: .5, // Opacity of modal background
      in_duration: 300, // Transition in duration
      out_duration: 200, // Transition out duration
      ready: function() { alert('Ready'); }, // Callback for Modal open
      complete: function() { alert('Closed'); } // Callback for Modal close
    }
  );

```

##Parallax

[Прочитать и посмотреть пример](http://materializecss.com/parallax.html)

###Parallax HTML Structure

```html

    <div class="parallax-container">
      <div class="parallax"><img src="images/parallax1.jpg"></div>
    </div>

```
```js

    $(document).ready(function(){
      $('.parallax').parallax();
    });

```

```css

	.parallax-container {
      height: "your height here";
    }

```

###Demo

[Посмотреть demo](http://materializecss.com/parallax-demo.html)

**Parallax Demo HTML**

```html

  <div class="parallax-container">
    <div class="parallax"><img src="images/parallax1.jpg"></div>
  </div>
  <div class="section white">
    <div class="row container">
      <h2 class="header">Parallax</h2>
      <p class="grey-text text-darken-3 lighten-3">Parallax is an effect where the background content or image in this case, is moved at a different speed than the foreground content while scrolling.</p>
    </div>
  </div>
  <div class="parallax-container">
    <div class="parallax"><img src="images/parallax2.jpg"></div>
  </div>

```

##Pushpin - прикрепить блок при скролле с опделенного момента до другого позиционирования.

```js

  $(document).ready(function(){
    $('.tabs-wrapper .row').pushpin({ top: $('.tabs-wrapper').offset().top });
  });

```
###CSS Classes

```css

  // Class for when element is above threshold
  .pin-top {
    position: relative;
  }

  // Class for when element is below threshold
  .pin-bottom {
    position: relative;
  }

  // Class for when element is pinned
  .pinned {
    position: fixed !important;
  }

```

###jQuery Plugin Options

**Top** - Расстояние в пикселях от верхней границы страницы, где элемент станет фиксированным. (Default: 0)

**Bottom** - Расстояние в пикселях от верхней границы страницы, где элемент перестанет быть фиксированным. (Default: infinity)

**Offset** - Отступ от верхней границы окна, на которой будет фиксироваться элемент. (Default: 0)

##ScrollFire

Действия при прокрутке , скролла страницы. Это могу быть анимации, сообщения и тп.

##Scrollspy

Следит за контентом и отмечает активным классом пункты меню

###Table of Contents Structure

```html

  <div class="row">
    <div class="col s12 m9 l10">
      <div id="introduction" class="section scrollspy">
        <p>Content </p>
      </div>

      <div id="structure" class="section scrollspy">
        <p>Content </p>
      </div>

      <div id="initialization" class="section scrollspy">
        <p>Content </p>
      </div>
    </div>
    <div class="col hide-on-small-only m3 l2">
      <ul class="section table-of-contents">
        <li><a href="#introduction">Introduction</a></li>
        <li><a href="#structure">Structure</a></li>
        <li><a href="#initialization">Intialization</a></li>
      </ul>
    </div>
  </div>

```
```js

  $(document).ready(function(){
    $('.scrollspy').scrollSpy();
  });

```

##Tabs / Табы

###Tabs HTML Structure

```html

  <div class="row">
    <div class="col s12">
      <ul class="tabs">
        <li class="tab col s3"><a href="#test1">Test 1</a></li>
        <li class="tab col s3"><a class="active" href="#test2">Test 2</a></li>
        <li class="tab col s3 disabled"><a href="#test3">Disabled Tab</a></li>
        <li class="tab col s3"><a href="#test4">Test 4</a></li>
      </ul>
    </div>
    <div id="test1" class="col s12">Test 1</div>
    <div id="test2" class="col s12">Test 2</div>
    <div id="test3" class="col s12">Test 3</div>
    <div id="test4" class="col s12">Test 4</div>
  </div>

```
```js

  $(document).ready(function(){
    $('ul.tabs').tabs();
  });

```
```js

  $(document).ready(function(){
    $('ul.tabs').tabs('select_tab', 'tab_id');
  });

```

##Transitions

Этот плагин подобен ScrollFire. При клике на кнопку , элементы плавно появляются.

[Посмотреть demo](http://materializecss.com/transitions.html)

##Waves / Волна

###Применение волн

Добавляем класс к кнопкам **.waves-effect** для добавления волны при клике.
```html

 <a class="waves-effect waves-light btn-large" href="#">Wave</a>

```
####Нестандартные цвета

Для добавления цвета волны используем класс **waves- + цвет**

```html

 <a href="#!" class="btn waves-effect waves-teal">Send</a>

```

Если нужен свой цвет. Пишем CSS:

```css

    /*
    When creating your CSS selector,
    change "brown" to something of your choosing
    */
    .waves-effect.waves-brown .waves-ripple {
     /* The alpha value allows the text and background color
     of the button to still show through. */
      background-color: rgba(121, 85, 72, 0.65);
    }

```

###Circle

Добавить класс для круглых кнопок **waves-circle**.

+ Default

+ waves-light

```html

  <a href="#!" class="waves-effect waves-circle waves-light btn-floating secondary-content">
    <i class="material-icons">add</i>
  </a>

```