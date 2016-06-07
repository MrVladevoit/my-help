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