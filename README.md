# javanomeemail
javascript
<html>
<head>
<script type="text/javascript">
function verifica() {
  if (document.forms[0].email.value.length == 0) {
    alert('Por favor, informe o seu EMAIL.');
	document.frmEnvia.email.focus();
    return false;
  }
  return true;
}
 
function checarEmail(){
if( document.forms[0].email.value=="" 
   || document.forms[0].email.value.indexOf('@')==-1 
     || document.forms[0].email.value.indexOf('.')==-1 )
	{
	   alert( "Por favor, informe um E-MAIL válido!" );
	   return false;
	}
}
</script>
</head>
<body>
<form method="post" action="" onSubmit="return ( verifica() )" name="frmEnvia">
   <label for="nome">Nome: </label>
   <input name="nome" type="text" class="input" id="nome" onblur="checarNome();" />
   <label for="email">E-mail: </label>
   <input name="email" type="text" class="input" id="email" onblur="checarEmail();" />
   <input name="submit" type="submit" value=" VALIDAR"/>
</form>
</body>

</html>
