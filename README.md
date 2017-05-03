Página Web Básica con Bootstrap 3
==========

En esta clase vamos a ver como crear una página básica con Bootstrap 3 y que se pueda ver para los múltiples dispositivos como escritorio, tablets y teléfonos mobiles.


Paso 1: Plantilla básica
--------------------

Primero debemos de tener la estructura básica de la plantilla que nos ofrece Bootstrap desde su pagina oficial. Seria la siguiente y la puedes usar en cualquier editor:

```
<!DOCTYPE html>
<html lang="es">
<head>
	<meta charset="utf-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge">
	<meta name="viewport" content="width=device-width, initial-scale=1">

	<title>Página Web Básica con Bootstrap 3</title>

	<!-- Bootstrap -->
	<!-- Latest compiled and minified CSS -->
	<link rel="stylesheet" href="css/bootstrap.min.css">
	<script src="https://use.fontawesome.com/79a0b2f6a0.js"></script>
	<link href="css/custom.css" rel="stylesheet">

	<!-- HTML5 Shim and Respond.js IE8 support of HTML5 elements and media queries -->
	<!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
 <!--[if lt IE 9]>
  <script src="https://oss.maxcdn.com/html5shiv/3.7.2/html5shiv.min.js"></script>
  <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
  <![endif]-->
</head>
<body>

  <!-- Librerías y Archivos JS-->
  <!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
  <script src="js/jquery-3.2.1.min.js"></script>
  <!-- Include all compiled plugins (below), or include individual files as needed -->

  <!-- Bootstrap Latest compiled and minified JavaScript -->
  <script src="js/bootstrap.min.js"></script>
</body>
</html>

 ```

 Paso 2: Menú de navegación
 --------------------

 Ahora vamos a insertar el código para tener el menú de navegación, con un buscador, y el menú con opciones dentro:

 ```
 <div class="container">
 <div class="row">
  <!-- Sección de Header -->
  <header>
   <!-- Sección de Nav -->
   <nav class="navbar navbar-default" role="navigation">
    <div class="container-fluid">
     <!-- Brand and toggle get grouped for better mobile display -->
     <div class="navbar-header">
      <button type="button" class="navbar-toggle" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1">
       <span class="sr-only">Toggle navigation</span>
       <span class="icon-bar"></span>
       <span class="icon-bar"></span>
       <span class="icon-bar"></span>
      </button>
      <a class="navbar-brand" href="#">Proyecto Autogestión</a>
     </div>

     <!-- Collect the nav links, forms, and other content for toggling -->
     <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
      <ul class="nav navbar-nav">
       <li class="active"><a href="#">Inicio</a></li>
       <li><a href="#">Nosotros</a></li>
       <li class="dropdown">
        <a href="#" class="dropdown-toggle" data-toggle="dropdown">Servicios <span class="caret"></span></a>
        <ul class="dropdown-menu" role="menu">
         <li><a href="#">Desarrollos</a></li>
         <li><a href="#">Diseño</a></li>
         <li><a href="#">Publicidad</a></li>
         <li class="divider"></li>
         <li><a href="#">Consultoria</a></li>
         <li class="divider"></li>
         <li><a href="#">Otros</a></li>
        </ul>
       </li>
       <li><a href="#">Contacto</a></li>
      </ul>

      <form class="navbar-form navbar-left" role="search">
       <div class="form-group">
        <input type="text" class="form-control" placeholder="Buscador">
       </div>
       <button type="submit" class="btn btn-default">Buscar</button>
      </form>
      <ul class="nav navbar-nav navbar-right">
       <li><a href="#">Usuario</a></li>
       <li class="dropdown">
        <a href="#" class="dropdown-toggle" data-toggle="dropdown">Mi cuenta <span class="caret"></span></a>
        <ul class="dropdown-menu" role="menu">
         <li><a href="#">Ingresar</a></li>
         <li><a href="#">Registrarse</a></li>
         <li><a href="#">Configuración</a></li>
         <li class="divider"></li>
         <li><a href="#">Cerrar Sesión</a></li>
        </ul>
       </li>
      </ul>
     </div><!-- /.navbar-collapse -->
    </div><!-- /.container-fluid -->
   </nav><!-- Fin Sección de Nav -->
  </header><!-- Fin Sección de Header -->
 </div>
</div>
 ```

 Paso 3: Cabecera usando jumbotron
 --------------------

Después vamos a realizar la cabecera principal en donde puedes hacer destacar de manera elegante algun articulo, anuncio, etc. Esto lo podemos hacer bien fácil con Bootstrap usando el código siguiente:

 ```
 <!-- Sección Jumbotron -->
<div class="container">
  <div class="row">
   <div class="jumbotron">
    <h1>Web Básica con Bootstrap 3</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellendus dolorem ad officiis nihil delectus quidem animi rerum, molestias sint natus ducimus quod, unde molestiae dolores laboriosam error facilis odio doloremque.</p>
    <p><a class="btn btn-primary btn-lg" role="button">Leer mas</a></p>
  </div>
</div>
 </div><!-- Fin Sección Jumbotron -->

 ```

 Paso 4: Insertando los artículos
 --------------------

 Vamos a insertar los artículos en nuestra pagina, en este caso puedes utilizar los artículos que quieras, pero para este ejemplo solo te mostrare a continuación el código de un solo articulo, si tu quieres mas artículos solo tienes que copiar y pegar lo siguiente:

 ```
 <!-- Sección de Artículos -->
  <div class="container" style="padding: 15px 10px;">
    <div class="row">
      <div class="col-xs-12 col-sm-6 col-md-4">
        <h2>Titulo del articulo 1</h2>
        <figure></figure><!-- Especificar contenido gráfico Ej: Una Imagen -->
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Fugiat distinctio illo rerum atque ducimus, laboriosam debitis eum deserunt ab libero quis voluptas, illum, perferendis numquam aut aliquam itaque qui magnam!</p>
        <a href="#" class="btn btn-success">Leer mas</a>
      </div>

      <div class="col-xs-12 col-sm-6 col-md-4">
        <h2>Titulo del articulo 2</h2>
        <figure></figure><!-- Especificar contenido gráfico Ej: Una Imagen -->
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Fugiat distinctio illo rerum atque ducimus, laboriosam debitis eum deserunt ab libero quis voluptas, illum, perferendis numquam aut aliquam itaque qui magnam!</p>
        <a href="#" class="btn btn-success">Leer mas</a>
      </div>

      <div class="col-xs-12 col-sm-6 col-md-4">
        <h2>Titulo del articulo 3</h2>
        <figure></figure><!-- Especificar contenido gráfico Ej: Una Imagen -->
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Fugiat distinctio illo rerum atque ducimus, laboriosam debitis eum deserunt ab libero quis voluptas, illum, perferendis numquam aut aliquam itaque qui magnam!</p>
        <a href="#" class="btn btn-success">Leer mas</a>
      </div>
	
	<!-- Puedes agregar más articulos ... -->
	
    </div>
  </div><!-- Fin Sección de Artículos -->
 ```

 Paso 5: Multimedia
 --------------------

 También agregaremos imágenes y un video a nuestra web, para ello, escribiremos el siguiente código:

 ```
 <!-- Sección de Multimedia -->
<div class="container" style="padding: 15px 10px;">
  <div class="row">

    <div class="col-md-4">
      <div class="thumbnail">
        <a href="http://lorempixel.com/600/400/" target="_blank">
          <img src="http://lorempixel.com/600/400/" alt="Lights" style="width:100%">
          <div class="caption">
            <p>Lorem ipsum...</p>
          </div>
        </a>
      </div>
    </div>

    <div class="col-md-4">
      <div class="thumbnail">
        <div class="embed-responsive embed-responsive-4by3" style="padding-bottom: 66.9%;">
          <iframe class="embed-responsive-item" width="560" height="235" src="https://www.youtube.com/embed/Y1HHBXDL9bg" frameborder="0" allowfullscreen></iframe>
        </div>
        <div class="caption"> <p>Lorem ipsum...</p> </div>
      </div>
    </div>

    <div class="col-md-4">
      <div class="thumbnail">
        <a href="http://lorempixel.com/600/400/" target="_blank">
          <img src="http://lorempixel.com/600/400/" alt="Fjords" style="width:100%">
          <div class="caption">
            <p>Lorem ipsum...</p>
          </div>
        </a>
      </div>
    </div>

  </div>
  <hr>
 </div><!-- Sección de Multimedia -->
 ```

 Paso 6: Pie de Página / Footer
 --------------------

 Para terminar, vamos a insertar el pie de página o footer que consta de solo dos textos centrados en base a la pagina con el siguiente código:

 ```
 <footer class="footer-basic-centered">
  <p class="footer-company-motto">Proyecto Autogestión</p>
  <p class="footer-derechos">Todos los Derechos e Izquierdos Reservados &copy; 2017</p>
 </footer><!-- Fin Sección Pie de Página -->

 ```
