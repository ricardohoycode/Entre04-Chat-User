<h1>README<h1>

<ol>
    <li> Manejar usuarios
    <li> Esos usarios puedan inicar sesion 
    <li> Crear conversaciones
    <li> Leer las conversaciones de las cuales son miembros
    <li> Crear grupos de conversaciones 
    <li> Enviar mensajes 
    <li> Eliminar mensajes
</ol>
-------------------------------------------------
<ul>
    <li> Confirmacion de lectura del mensaje 
    <li> Manejar fotos de perfil 
    <li> Reenviar un mensaje 
    <li> Crear links para invitar gente a un grupo
</ul>

![Database Diagram](https://i.imgur.com/IHhtWv2.png)

<h2>Ejemplo de respuestas exitosas:<h2>

> {
>    error: false,
>    status: 201,
>    message: 'User created Succesfully',
>    data: {
>        id: 5,
>        firstName: 'Hoyos',
>        ...
>    }
>    }

>  <h2>Autenticación</h2></hr>

<ul>
    <li>Log In</li>
    <li>Sign In</li>
    <li>Recovery Password id userId used true</li>
    <li>Verify Account</li>
    <li>Cuando hacemos un login recibimos lo siguiente - Email - Password</li>
</ul>

> <h2>POST</h2></hr>

<ul>
    <li>Validar si el usuario existe - Vamos a buscar el usuario al que le pertenezca el correo electronico que recibimos.</li>
    <li>Validar si la contraseña es correcta - Validando la contraseña que recibimos con la contraseña que esta en mi base de datos.</li>
    <li>Generar una respuesta con el token.</li>
</ul>


> <h2> Autenticacion por tokens</h2></hr>

> <h3>Recibimos el token</h3>

> Ese token lo desencriptamos. Una vez el token desencriptado, tenemos que ver si pertenece a un usuario de mi app. Esto se logra haciendo una validacion buscando en mi db si existe x usuario con el id que viene en el token damos paso a la peticion si es que es un usuario real o generamos un error en caso de que no lo sea
