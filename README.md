# calculadora-
Calculadora con operaciones básicas, áreas geométricas, estadística y Fibonacci"

Desarrolle una calculadora multifuncional en Python que integra:

✅ Operaciones básicas: suma, resta, multiplicación y división con manejo robusto de errores
📐 Cálculo de áreas geométricas: círculo (con radio/diámetro), cuadrado, triángulo y trapecio
📊 Estadística básica: media, mediana y moda para series numéricas ingresadas por el usuario
🔢 Sucesión de Fibonacci: generación de términos auténticos validando que pertenezcan a la secuencia real
Este proyecto fue diseñado para demostrar código profesional, documentación clara y buenas prácticas de control de versiones, cumpliendo con los estándares exigidos para entornos colaborativos de desarrollo.

⚙️ ¿CÓMO LO HICE?
Arquitectura y Lógica
Implementamos una estructura modular con las siguientes características clave:

1. Validación Centralizada de Entradas
Cree la función validar_numero() que maneja todas las entradas del usuario con:
Conversión segura de tipos (float/int)
Validación de números positivos donde aplica (geometría)
Prevención de divisiones por cero
Mensajes de error específicos y amigables

2. Manejo Matemático Riguroso
Para Fibonacci: Implemente la propiedad matemática que verifica si un número pertenece a la secuencia real:
python

def es_numero_fibonacci(n):
    """Verifica si un número pertenece a la sucesión de Fibonacci usando propiedades matemáticas."""
    if n < 0: 
        return False
    return es_cuadrado_perfecto(5*n*n + 4) or es_cuadrado_perfecto(5*n*n - 4)
En estadística: Use collections.Counter para calcular la moda, resolviendo empates seleccionando el valor más pequeño.
3. Interfaz de Usuario Intuitiva
Menú jerárquico con separadores visuales y retroalimentación inmediata
Submenús contextuales (ej: para círculos, permite ingresar radio o diámetro)
Formato numérico consistente (4 decimales para resultados)
