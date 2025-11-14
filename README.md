# 🧮 Calculadora Multifuncional


## 📌 Descripción del Proyecto
Esta calculadora multifuncional en Python integra operaciones matemáticas básicas, cálculos geométricos, estadística descriptiva y generación de la sucesión real de Fibonacci. El proyecto demuestra buenas prácticas de programación, manejo robusto de errores y documentación profesional, cumpliendo con los requisitos de transferibilidad de código en entornos colaborativos.

## ⚙️ Cómo Funciona
### Arquitectura y Lógica
El sistema está organizado en módulos independientes:
1. **`validar_numero()`**: Maneja todas las entradas de usuario con validación contextual (números positivos, no división por cero, etc.).
2. **Operaciones básicas**: Implementa aritmética con manejo de excepciones para divisiones por cero.
3. **Áreas geométricas**: 
   - Círculo: Calcula área, diámetro y radio intercambiablemente
   - Cuadrado/Triángulo/Trapecio: Fórmulas estándar con validación de dimensiones positivas
4. **Estadística básica**: 
   - Media: Promedio aritmético
   - Mediana: Valor central en lista ordenada
   - Moda: Valor más frecuente (soluciona empates seleccionando el menor valor)
5. **Sucesión de Fibonacci**:
   - Valida que el número inicial pertenezca a la sucesión real usando propiedades matemáticas
   - Genera términos auténticos sin inventar valores


## 🎯 Propósito de Cada Módulo
| Módulo | Propósito | Características Clave |
|--------|-----------|----------------------|
| `validar_numero()` | Centralizar validación de entradas | Manejo de tipos, positividad, y casos especiales |
| Operaciones básicas | Cálculos aritméticos esenciales | Prevención de divisiones por cero |
| Áreas geométricas | Cálculos para figuras 2D | Flexibilidad en parámetros (radio/diámetro para círculos) |
| Estadística básica | Análisis de datos | Manejo de múltiples modas con selección determinista |
| Sucesión Fibonacci | Generación de secuencia matemática | Validación rigurosa usando propiedades numéricas |

## ⚠️ Dificultades y Soluciones
1. **Validación de números de Fibonacci**  
   **Dificultad**: Generar solo números auténticos sin inventar valores.  
   **Solución**: Implementamos la propiedad matemática que verifica si `5n²±4` es un cuadrado perfecto, garantizando autenticidad.

2. **Manejo de múltiples modas en estadística**  
   **Dificultad**: La moda puede no ser única en conjuntos de datos reales.  
   **Solución**: Seleccionamos el menor valor entre los números con máxima frecuencia, proporcionando un resultado determinista.

3. **Flexibilidad en cálculos circulares**  
   **Dificultad**: Permitir cálculo desde radio o diámetro manteniendo precisión.  
   **Solución**: Sistema de menú contextual que adapta las fórmulas según el dato proporcionado.

4. **Prevención de fallos en entradas**  
   **Dificultad**: Usuarios pueden ingresar valores no numéricos o negativos en contextos inadecuados.  
   **Solución**: Validación centralizada con retroalimentación inmediata y bucles de reintento.


   git clone https://github.com/tu-usuario/calculadora-multifuncional.git
   cd calculadora-multifuncional
