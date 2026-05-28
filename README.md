<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Travesía Alimenticia - Viaja por el sabor</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        principal: '#165DFF',
                        secundario: '#FF7D00',
                        claro: '#F8FAFF',
                        oscuro: '#0F172A'
                    },
                    fontFamily: {
                        sans: ['Segoe UI', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style type="text/tailwindcss">
        @layer utilities {
            .contenedor {
                max-width: 1200px;
                margin: 0 auto;
            }
            .tarjeta {
                border-radius: 16px;
                box-shadow: 0 4px 20px rgba(0,0,0,0.08);
                overflow: hidden;
            }
        }
    </style>
</head>
<body class="bg-claro font-sans">

    <!-- 👉 ENCABEZADO -->
    <header class="bg-principal text-white py-8 shadow-lg">
        <div class="contenedor px-4">
            <div class="text-center">
                <h1 class="text-4xl md:text-5xl font-bold mb-3">
                    <i class="fa fa-plane mr-3 text-secundario"></i>
                    TRAVESÍA ALIMENTICIA
                </h1>
                <p class="text-lg opacity-90 max-w-2xl mx-auto">
                    Un recorrido por el mundo a través de sus sabores, tradiciones y culturas
                </p>
            </div>
        </div>
    </header>

    <!-- 👉 SECCIÓN DE INTRODUCCIÓN -->
    <section class="py-12 bg-white">
        <div class="contenedor px-4">
            <div class="text-center mb-10">
                <h2 class="text-3xl font-bold text-principal mb-4">¿De qué se trata este viaje?</h2>
                <p class="text-gray-700 text-lg max-w-3xl mx-auto leading-relaxed">
                    La comida es mucho más que alimento: es historia, identidad y forma de ver la vida. 
                    En esta página podrás conocer platillos de diferentes países, su origen, sus ingredientes 
                    y por qué son tan especiales para cada pueblo. ¡Prepárate para viajar con el paladar!
                </p>
            </div>

            <!-- CATEGORÍAS POR REGIONES -->
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 gap-6 text-center">
                <div class="tarjeta bg-claro p-6 hover:bg-principal hover:text-white transition-all duration-300 cursor-pointer">
                    <i class="fa fa-map-marker text-4xl mb-3"></i>
                    <h3 class="font-bold text-xl">América</h3>
                </div>
                <div class="tarjeta bg-claro p-6 hover:bg-principal hover:text-white transition-all duration-300 cursor-pointer">
                    <i class="fa fa-building text-4xl mb-3"></i>
                    <h3 class="font-bold text-xl">Europa</h3>
                </div>
                <div class="tarjeta bg-claro p-6 hover:bg-principal hover:text-white transition-all duration-300 cursor-pointer">
                    <i class="fa fa-moon-o text-4xl mb-3"></i>
                    <h3 class="font-bold text-xl">Asia</h3>
                </div>
                <div class="tarjeta bg-claro p-6 hover:bg-principal hover:text-white transition-all duration-300 cursor-pointer">
                    <i class="fa fa-sun-o text-4xl mb-3"></i>
                    <h3 class="font-bold text-xl">África</h3>
                </div>
            </div>
        </div>
    </section>

    <!-- 👉 SECCIÓN DE PLATILLOS -->
    <section class="py-16 contenedor px-4">
        <h2 class="text-3xl font-bold text-center text-principal mb-12">Platillos de nuestra travesía</h2>

        <div class="space-y-12">

            <!-- 🥘 PLATILLO 1 -->
            <div class="tarjeta bg-white">
                <div class="md:flex">
                    <div class="md:w-1/2">
                        <img src="https://images.unsplash.com/photo-1551183053-bf91a1d81141?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" 
                             alt="Pupusas" class="w-full h-full object-cover">
                    </div>
                    <div class="md:w-1/2 p-8">
                        <span class="inline-block bg-secundario/10 text-secundario px-4 py-1 rounded-full text-sm font-semibold mb-3">
                            🇸🇻 El Salvador - América
                        </span>
                        <h3 class="text-3xl font-bold text-principal mb-3">Pupusas</h3>
                        <p class="text-gray-700 mb-4 leading-relaxed">
                            Son el platillo más representativo de El Salvador. Son tortillas de maíz rellenas de queso, 
                            frijoles o chicharrón. Se acompañan de salsa de tomate y curtido de verduras. 
                            Tienen más de 2000 años de historia y son consideradas patrimonio cultural.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm">Maíz</span>
                            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm">Queso</span>
                            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm">Verduras</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- 🍕 PLATILLO 2 -->
            <div class="tarjeta bg-white">
                <div class="md:flex flex-row-reverse">
                    <div class="md:w-1/2">
                        <img src="https://images.unsplash.com/photo-1621996346565-e3dbc646d9a9?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" 
                             alt="Pizza Napolitana" class="w-full h-full object-cover">
                    </div>
                    <div class="md:w-1/2 p-8">
                        <span class="inline-block bg-secundario/10 text-secundario px-4 py-1 rounded-full text-sm font-semibold mb-3">
                            🇮🇹 Italia - Europa
                        </span>
                        <h3 class="text-3xl font-bold text-principal mb-3">Pizza Napolitana</h3>
                        <p class="text-gray-700 mb-4 leading-relaxed">
                            Originaria de Nápoles, es uno de los platillos más famosos del mundo. Su receta original lleva 
                            masa de harina, salsa de tomate, queso mozzarella, albahaca fresca y aceite de oliva. 
                            Se cocina en hornos de leña y tiene reconocimiento como Patrimonio Inmaterial de la Humanidad.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm">Harina</span>
                            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm">Tomate</span>
                            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm">Queso</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- 🍣 PLATILLO 3 -->
            <div class="tarjeta bg-white">
                <div class="md:flex">
                    <div class="md:w-1/2">
                        <img src="https://images.unsplash.com/photo-1563245372-f21724e3856d?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" 
                             alt="Sushi" class="w-full h-full object-cover">
                    </div>
                    <div class="md:w-1/2 p-8">
                        <span class="inline-block bg-secundario/10 text-secundario px-4 py-1 rounded-full text-sm font-semibold mb-3">
                            🇯🇵 Japón - Asia
                        </span>
                        <h3 class="text-3xl font-bold text-principal mb-3">Sushi</h3>
                        <p class="text-gray-700 mb-4 leading-relaxed">
                            Es un conjunto de platillos basados en arroz aderezado con vinagre, acompañado de pescado crudo, 
                            mariscos, vegetales o huevo. Es parte fundamental de la cultura japonesa, donde se valora mucho 
                            la frescura de los ingredientes y la presentación.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm">Arroz</span>
                            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm">Pescado</span>
                            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm">Algas</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- 🍲 PLATILLO 4 -->
            <div class="tarjeta bg-white">
                <div class="md:flex flex-row-reverse">
                    <div class="md:w-1/2">
                        <img src="https://images.unsplash.com/photo-1585937421612-70a008356fbe?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" 
                             alt="Couscous" class="w-full h-full object-cover">
                    </div>
                    <div class="md:w-1/2 p-8">
                        <span class="inline-block bg-secundario/10 text-secundario px-4 py-1 rounded-full text-sm font-semibold mb-3">
                            🇲🇦 Marruecos - África
                        </span>
                        <h3 class="text-3xl font-bold text-principal mb-3">Couscous</h3>
                        <p class="text-gray-700 mb-4 leading-relaxed">
                            Es un platillo tradicional del norte de África, hecho de semillas de sémola de trigo cocidas al vapor. 
                            Se sirve acompañado de verduras, carne o pollo, y es muy usado en celebraciones y reuniones familiares. 
                            Es símbolo de hospitalidad y amistad.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm">Sémola</span>
                            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm">Verduras</span>
                            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm">Carne</span>
                        </div>
                    </div>
                </div>
            </div>

        </div>
    </section>

    <!-- 👉 SECCIÓN DE DATOS CURIOSOS -->
    <section class="py-16 bg-principal text-white">
        <div class="contenedor px-4">
            <h2 class="text-3xl font-bold text-center mb-12">Datos curiosos de la comida</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="bg-white/10 p-8 tarjeta text-center">
                    <i class="fa fa-history text-5xl text-secundario mb-4"></i>
                    <h3 class="text-xl font-bold mb-3">Historia antigua</h3>
                    <p class="opacity-90 leading-relaxed">
                        Muchos platillos que comemos hoy tienen más de mil años de historia y han viajado 
                        de generación en generación, cambiando poco a poco según el lugar.
                    </p>
                </div>
                <div class="bg-white/10 p-8 tarjeta text-center">
                    <i class="fa fa-heart text-5xl text-secundario mb-4"></i>
                    <h3 class="text-xl font-bold mb-3">Unión de pueblos</h3>
                    <p class="opacity-90 leading-relaxed">
                        La comida une a las personas sin importar de dónde sean. Compartir un platillo es una 
                        forma hermosa de mostrar respeto, cariño y amistad.
                    </p>
                </div>
                <div class="bg-white/10 p-8 tarjeta text-center">
                    <i class="fa fa-leaf text-5xl text-secundario mb-4"></i>
                    <h3 class="text-xl font-bold mb-3">Ingredientes locales</h3>
                    <p class="opacity-90 leading-relaxed">
                        Cada región usa lo que la naturaleza le ofrece, por eso cada lugar tiene sabores únicos 
                        y especiales que no se encuentran en ningún otro sitio del mundo.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- 👉 PIE DE PÁGINA -->
    <footer class="bg-oscuro text-white py-8">
        <div class="contenedor px-4 text-center">
            <h3 class="text-2xl font-bold mb-3">Travesía Alimenticia</h3>
            <p class="opacity-75 mb-4">Conoce el mundo a través de su sabor y tradiciones</p>
            <p class="text-sm opacity-50">&copy; 2024 - Todos los derechos reservados</p>
        </div>
    </footer>

</body>
</html>
