- 👋 Hi, I’m @antonio180591
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
antonio180591/antonio180591 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

<?php
// Incluye la biblioteca QR Code
include 'phpqrcode/qrlib.php';

// URL que quieres que el código QR represente
$url = 'https://www.ejemplo.com/documento.pdf';

// Nombre del archivo QR (puedes personalizarlo como desees)
$archivo_qr = 'qr_code.png';

// Tamaño y nivel de corrección del código QR (opcional)
$tamaño = 10; // Tamaño de cada píxel del QR
$nivelCorreccion = 'L'; // Nivel de corrección: L, M, Q, H (L = bajo, H = alto)

// Genera el código QR
QRcode::png($url, $archivo_qr, $nivelCorreccion, $tamaño);

// Muestra el código QR generado
echo '<img src="'.$archivo_qr.'" />';
?>

