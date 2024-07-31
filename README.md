<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Generador de código QR</title>
</head>
<body>
    <h1>Generador de código QR</h1>
    <div id="qr_code"></div>

    <!-- Script PHP para generar y mostrar el código QR -->
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
</body>
</html>

