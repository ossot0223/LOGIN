<!DOCTYPE html>
<html lang="es">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Mi primer Login</title>
	<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
</head>
<body class="align-content-center text-center" style="height: 100vh;">
	<main class="form-signin" style="width: 100%;max-width: 330px;margin: auto; padding: 15px;">
		<form>
			<h1 class="h3 mb-3 fw-normal">Ingrese a su cuenta</h1>
	
			<div class="form-floating mb-3">
				<input type="text" class="form-control" id="usuario" placeholder="name@example.com">
				<label for="email">usuario</label>
			</div>
			<div class="form-floating mb-3">
				<input type="password" class="form-control" id="password" placeholder="Password">
				<label for="password">contraseña</label>
			</div>
	
			<div class="checkbox mb-3">
				<label>
					<input type="checkbox" value="remember-me"> Recuerdame
				</label>
			</div>
			<button class="w-100 btn btn-lg btn-primary"  type="button" onclick="validarUsuario()" >Ingresar</button>
			<p class="mt-5 mb-3 text-muted">© 2024-2029</p>
		</form>
	</main>
	
	<script>
		
		function validarUsuario(){
			
			let usuario = document.getElementById('usuario').value;
			let pass = document.getElementById("password").value;
			
			if (usuario == "david" && pass == 1234) {
				window.location.href = 'catalogo.html'
			}
		}
		
	</script>
</body>
</html>
