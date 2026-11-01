# 10 prompts esenciales de vibe coding

Uno por mensaje. Reemplaza lo que está entre `[corchetes]`.

**1. Plan antes de código**
```
Esta es mi idea: [describe tu app en 3-5 frases: qué hace, para quién, qué es lo más
importante]. Antes de escribir código, propón: la tecnología más simple para lograrlo,
las 3 funcionalidades de la primera versión, qué dejaría fuera por ahora y una lista
de 5 a 8 tareas en orden. Espera mi aprobación.
```

**2. Una tarea a la vez**
```
Ejecuta solo la tarea [número] del plan. Cuando termines, dime qué cambiaste y cómo
lo pruebo yo paso a paso. No avances a la siguiente tarea.
```

**3. Explícame el proyecto**
```
Explícame en 10 viñetas cómo está organizado este proyecto y qué hace cada parte
importante. Sin jerga. No cambies nada.
```

**4. Guardar un punto seguro**
```
Si no existe, inicializa Git con un .gitignore que incluya .env y .env.local. Luego haz
commit de todo con un mensaje que describa lo que funciona ahora.
```

**5. Formulario bien hecho**
```
Crea el formulario [nombre] con los campos [lista]. Etiquetas visibles, validación en el
navegador y en el servidor, errores en español junto a cada campo, botón deshabilitado
mientras envía, mensaje de éxito y que se vea bien en celular.
```

**6. Mejorar el diseño sin romper nada**
```
Mejora el diseño de [página] para que se vea moderno y profesional. Cambia solo estilos;
no toques la lógica, los datos ni los textos.
```

**7. Diagnóstico antes de arreglar**
```
Tengo este error: [pega el error completo]. Pasa cuando [qué hago]. Antes de cambiar
código, explícame en simple qué significa y las 3 causas más probables. Después propón
el arreglo mínimo, indicando qué archivo y qué líneas vas a cambiar.
```

**8. Cortar el loop**
```
Llevamos varios intentos sin resolver [problema]. Detente. Resume qué intentamos y por
qué no funcionó, y propón un enfoque distinto y más simple. Espera mi ok.
```

**9. Revisar claves expuestas**
```
Busca en todo el proyecto claves, tokens o contraseñas escritas en el código, variables
secretas con prefijo NEXT_PUBLIC_ o VITE_ y archivos .env que no estén en .gitignore.
Dame la lista con archivo y línea, sin cambiar nada todavía.
```

**10. Cerrar la sesión**
```
Terminamos por hoy. Crea o actualiza PROXIMA-SESION.md con: qué funciona, qué quedó a
medias, problemas abiertos y la siguiente tarea. Luego haz commit con un mensaje claro.
```

---
¿Quieres los 50 prompts, guía de pagos por país (Stripe, PayPal, Mercado Pago y más), publicación con dominio propio y plantillas por rubro? 👉 **https://marena74.gumroad.com/l/yjwiym**
