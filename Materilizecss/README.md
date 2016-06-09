# Моя шпаргалка по работе с Materializecss.com

![alt tag](https://scotch.io/wp-content/uploads/2015/01/getting-started-materialize-css-framework.png)

Materializecss.com - это фремворк material designer на SASS.

1. Скачать
 + [Скачать и использовать](#Установка-GIT);


## Скачать и использовать Materializecss.com

Для того, чтобы начать переходим по ссылке : + [http://materializecss.com/getting-started.html](http://materializecss.com/getting-started.html)

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

**Адаптивные изображения** - добавляем класс **.responsive-img** - для стилей адаптивных картинок max-width: 100% и height:auto.

**Скругленные изображения** - class="circle"

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

Добавить класс = "responsive-table" к таблице тегов, чтобы сделать таблицу адаптивной.На мобильных устройствах появляется скролл горизонтальный.

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

 + [Прочитать и посмотреть пример](http://materializecss.com/badges.html);


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

 + [Прочитать и посмотреть пример](http://materializecss.com/buttons.html);

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

 + [Прочитать и посмотреть пример](http://materializecss.com/cards.html);

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

###Карточка с imgages


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

 + [Прочитать и посмотреть пример](http://materializecss.com/collections.html);


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

##Form

 + [Прочитать и посмотреть пример](http://materializecss.com/forms.html);

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

<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">

Используем html:

```html

	<i class="material-icons">add</i>

```

##Navbar

 + [Прочитать и посмотреть пример](http://materializecss.com/navbar.html);

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

 + [Прочитать и посмотреть пример](http://materializecss.com/navbar.html);

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

 + [Прочитать и посмотреть пример](http://materializecss.com/navbar.html);

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