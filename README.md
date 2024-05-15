# Automatización de Pruebas para Urban Routes

Este repositorio contiene un conjunto de pruebas automatizadas para la aplicación web Urban Routes, utilizando Selenium WebDriver en Python.

## Descripción

El código proporcionado define una serie de pruebas para validar la funcionalidad de la aplicación Urban Routes. Esto incluye pruebas para la navegación de páginas, interacción con elementos de la interfaz de usuario, y la verificación de flujos de trabajo críticos como la selección de rutas, ingreso de números de teléfono, y métodos de pago.

## Requisitos

- Python 3.6 o superior
- Selenium WebDriver
- Google Chrome o cualquier navegador compatible con WebDriver

## Configuración

Antes de ejecutar las pruebas, asegúrese de tener instalado Selenium WebDriver y el controlador correspondiente para su navegador.

## Estructura del Código

El código se divide en varias partes:

## Archivo Main:
- `TestUrbanRoutes`: Clase principal que contiene todos los métodos de prueba.
- `setup_class`: Método para configurar las opciones del navegador y el WebDriver antes de ejecutar las pruebas.
- Métodos de prueba: Cada método `test_*` representa una prueba independiente para un aspecto específico de la aplicación.

## Archivo Helpers:
- retrieve_phone_code:
Este método recupera un código de confirmación de teléfono de los registros de rendimiento del navegador y lo devuelve como una cadena de texto. Utilice este método después de haber solicitado el código en la aplicación.
- wait_visibility_of_element: Espera hasta que el elemento especificado sea visible en la página antes de continuar con la siguiente acción.
- wait_to_be_clickable_of_element: Espera hasta que el elemento especificado sea clickeable antes de continuar con la siguiente acción.

## Archivo UrbanRotesPage:

-set_from_to: Establece las direcciones de origen y destino.
-get_from_to: Obtiene los valores actuales de las direcciones de origen y destino.
-click_botton_confort: Realiza clics en los botones para pedir un taxi y seleccionar opciones de confort.
-click_find_taxi: Realiza un clic en el botón para solicitar un taxi.
-check_botton_find_taxi: Verifica si el botón para buscar un taxi está visible.
-check_taxi_driver_selected: Verifica si se ha seleccionado un conductor.
-check_order_header_title: Verifica si el título del encabezado del pedido está visible.
-set_steps_number_and_code_phone: Ingresa un número de teléfono y espera un código SMS.
-set_steps_payment_method: Ingresa detalles de la tarjeta de crédito y confirma el método de pago.
-set_message_for_driver: Envía un mensaje al conductor.
-click_blanket_selector: Activa el selector de manta y pañuelos.
-get_blanket_value: Obtiene el valor del selector de manta y pañuelos.
 
