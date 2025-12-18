<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Volante Multiservicios Ayquipa</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700;900&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Open Sans', sans-serif;
            background-color: #f3f4f6;
        }
        h1, h2, h3, .price-tag {
            font-family: 'Montserrat', sans-serif;
        }
        .pattern-bg {
            background-image: radial-gradient(#e5e7eb 1px, transparent 1px);
            background-size: 20px 20px;
        }
        .clip-path-header {
            clip-path: polygon(0 0, 100% 0, 100% 85%, 50% 100%, 0 85%);
        }
        @media print {
            body {
                background-color: white;
                -webkit-print-color-adjust: exact;
                print-color-adjust: exact;
            }
            .no-print {
                display: none;
            }
            .page-container {
                box-shadow: none;
                margin: 0;
                width: 100%;
                max-width: 100%;
            }
        }
    </style>
</head>
<body class="min-h-screen flex flex-col items-center justify-center p-4 pattern-bg">

    <!-- Botón de Imprimir (Visible solo en pantalla) -->
    <div class="no-print mb-6 fixed top-4 right-4 z-50">
        <button onclick="window.print()" class="bg-blue-600 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded-full shadow-lg transition duration-300 flex items-center gap-2">
            <i class="fas fa-print"></i> Imprimir / Guardar PDF
        </button>
    </div>

    <!-- Contenedor del Volante (Tamaño A5 aproximado para visualización, ajustable) -->
    <div class="page-container bg-white w-full max-w-lg shadow-2xl overflow-hidden relative" style="min-height: 800px;">
        
        <!-- Encabezado -->
        <header class="bg-red-700 text-white pt-8 pb-12 px-6 text-center clip-path-header relative">
            <div class="absolute top-0 left-0 w-full h-full opacity-10 bg-[url('https://www.transparenttextures.com/patterns/food.png')]"></div>
            <p class="text-yellow-400 font-bold tracking-widest text-sm uppercase mb-2">¡Todo lo que necesitas en un solo lugar!</p>
            <h1 class="text-4xl md:text-5xl font-black uppercase leading-tight drop-shadow-md">
                Multiservicios<br>
                <span class="text-yellow-400">Ayquipa</span>
            </h1>
            <div class="mt-4 inline-block bg-white text-red-700 px-6 py-1 rounded-full font-bold text-sm shadow-md">
                VENTA POR MAYOR Y MENOR
            </div>
        </header>

        <!-- Sección Principal de Ofertas -->
        <main class="px-6 py-4">
            
            <div class="text-center mb-6">
                <h2 class="text-2xl font-bold text-gray-800 uppercase border-b-4 border-yellow-400 inline-block px-4 pb-1">
                    Super Ofertas
                </h2>
            </div>

            <!-- Grid de Productos Destacados -->
            <div class="grid grid-cols-2 gap-4 mb-6">
                <!-- Producto 1 -->
                <div class="border-2 border-red-100 rounded-lg p-3 text-center relative overflow-hidden group hover:border-red-500 transition">
                    <div class="absolute top-0 right-0 bg-yellow-400 text-red-800 text-xs font-bold px-2 py-1 rounded-bl-lg">OFERTA</div>
                    <i class="fas fa-wine-bottle text-4xl text-red-600 mb-2 mt-2"></i>
                    <h3 class="font-bold text-gray-700 text-sm">Aceite Vegetal</h3>
                    <p class="text-xs text-gray-500 mb-1">Botella 1 Litro</p>
                    <div class="text-2xl font-black text-red-700 price-tag">S/ 8.50</div>
                </div>

                <!-- Producto 2 -->
                <div class="border-2 border-red-100 rounded-lg p-3 text-center relative overflow-hidden group hover:border-red-500 transition">
                    <div class="absolute top-0 right-0 bg-yellow-400 text-red-800 text-xs font-bold px-2 py-1 rounded-bl-lg">OFERTA</div>
                    <i class="fas fa-shopping-bag text-4xl text-blue-600 mb-2 mt-2"></i>
                    <h3 class="font-bold text-gray-700 text-sm">Arroz Superior</h3>
                    <p class="text-xs text-gray-500 mb-1">Por Kilo</p>
                    <div class="text-2xl font-black text-red-700 price-tag">S/ 3.80</div>
                </div>

                 <!-- Producto 3 -->
                 <div class="border-2 border-red-100 rounded-lg p-3 text-center relative overflow-hidden group hover:border-red-500 transition">
                    <div class="absolute top-0 right-0 bg-yellow-400 text-red-800 text-xs font-bold px-2 py-1 rounded-bl-lg">PACK</div>
                    <i class="fas fa-mug-hot text-4xl text-amber-700 mb-2 mt-2"></i>
                    <h3 class="font-bold text-gray-700 text-sm">Leche Evaporada</h3>
                    <p class="text-xs text-gray-500 mb-1">Pack x 6 Unid.</p>
                    <div class="text-2xl font-black text-red-700 price-tag">S/ 21.00</div>
                </div>

                 <!-- Producto 4 -->
                 <div class="border-2 border-red-100 rounded-lg p-3 text-center relative overflow-hidden group hover:border-red-500 transition">
                    <i class="fas fa-soap text-4xl text-teal-500 mb-2 mt-2"></i>
                    <h3 class="font-bold text-gray-700 text-sm">Detergente</h3>
                    <p class="text-xs text-gray-500 mb-1">Bolsa 2kg</p>
                    <div class="text-2xl font-black text-red-700 price-tag">S/ 14.50</div>
                </div>
            </div>

            <!-- Lista de Categorías -->
            <div class="bg-gray-100 rounded-xl p-5 mb-6 border-l-4 border-red-600">
                <h3 class="font-bold text-gray-800 text-lg mb-3 flex items-center">
                    <i class="fas fa-list-ul mr-2 text-red-600"></i> Tenemos todo para tu hogar:
                </h3>
                <ul class="grid grid-cols-2 gap-2 text-sm text-gray-700">
                    <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Abarrotes en General</li>
                    <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Bebidas y Gaseosas</li>
                    <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Útiles de Aseo</li>
                    <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Lácteos y Embutidos</li>
                    <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Snacks y Golosinas</li>
                    <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Comida para Mascotas</li>
                </ul>
            </div>

             <!-- Sección de Agente/Servicios -->
             <div class="flex justify-between items-center bg-blue-50 p-4 rounded-lg border border-blue-200 mb-6">
                 <div>
                     <h3 class="font-bold text-blue-900">¿Necesitas Efectivo?</h3>
                     <p class="text-xs text-blue-700">Contamos con Agente BCP y Yape</p>
                 </div>
                 <div class="flex gap-2">
                     <div class="bg-orange-500 text-white w-10 h-10 rounded-full flex items-center justify-center font-bold text-xs shadow-sm">BCP</div>
                     <div class="bg-purple-600 text-white w-10 h-10 rounded-full flex items-center justify-center font-bold text-xs shadow-sm">Yape</div>
                 </div>
             </div>

        </main>

        <!-- Pie de Página -->
        <footer class="bg-gray-900 text-white p-6 text-center">
            <h3 class="text-yellow-400 font-bold text-xl mb-4">¡TE ESPERAMOS!</h3>
            
            <div class="flex flex-col gap-3 text-sm">
                <div class="flex items-center justify-center gap-3">
                    <i class="fas fa-map-marker-alt text-red-500 text-xl"></i>
                    <span class="text-gray-300">[Dirección de tu Tienda Aquí], Arequipa</span>
                </div>
                
                <div class="flex items-center justify-center gap-3">
                    <i class="fab fa-whatsapp text-green-500 text-xl"></i>
                    <span class="text-gray-300">Pedidos: 987 654 321</span>
                </div>

                <div class="flex items-center justify-center gap-3">
                    <i class="far fa-clock text-blue-400 text-xl"></i>
                    <span class="text-gray-300">Lun - Sab: 7:00 AM - 9:00 PM</span>
                </div>
            </div>
            
            <div class="mt-6 pt-4 border-t border-gray-700 text-xs text-gray-500">
                Atención rápida y los mejores precios del barrio.
            </div>
        </footer>

    </div>

</body>
</html>
