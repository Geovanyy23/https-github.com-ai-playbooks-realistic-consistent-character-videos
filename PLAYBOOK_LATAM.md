# PLAYBOOK LATAM — Minidramas realistas y personajes consistentes (v1.0)

> Adaptación para VideoExpress. Idioma de los **diálogos y voces: español latino**, preferencia colombiano neutro. Los prompts visuales pueden estar en inglés para mayor precisión. **Este documento describe un flujo de trabajo; no garantiza que VideoExpress genere siempre una voz, identidad o lip sync correctos.** Prueba clips cortos antes de gastar créditos en la historia completa.

## 0. Principios y seguridad
- Usa solo imágenes de **personas adultas con consentimiento** o personajes originales ficticios. No suplantes a personas reales en situaciones engañosas, difamatorias, humillantes o de noticia falsa.
- **No publiques** por defecto: desactiva «Share this in the public gallery» cada vez que se abra un panel de generación.
- No aceptes en nombre del usuario condiciones legales, permisos sensibles, compras ni gastos. Pide intervención cuando sea necesario.
- Nunca exijas «Full access» como requisito universal: usa el modo navegador disponible y los permisos mínimos necesarios; si no es posible operar VideoExpress, entrega los prompts y una guía manual.
- No prometas generación en segundo plano ni entregas futuras sin una ejecución real.
- Este es un repositorio de instrucciones, **no software instalable**.

## 1. Entrada
Solicita solo información indispensable, aprovechando lo ya dado:
1. Personaje A: nombre y 1–2 fotos nítidas de rostro con permiso, **o** descripción de personaje ficticio.
2. Personaje B: opcional, igual.
3. Idea de historia (una frase); si falta, propone 3 ideas originales.
4. Duración: 30 segundos por defecto (alternativas 45 o 60 segundos).
5. Formato: vertical 9:16 por defecto; 16:9 si se solicita.
6. Tipo: drama familiar, comedia, suspenso ligero, sorpresa, lección de vida.
7. Voz: **español latino**; por defecto **colombiano neutro**, sin caricaturizar el acento.
No pidas datos repetidos. Si el usuario trae personajes ficticios, no exijas fotos reales: se pueden usar ilustraciones originales como referencias, si la herramienta lo permite.

## 2. Biblia de personajes (Character Lock)
Para cada personaje, redacta una ficha fija de 90–140 palabras: rango de edad adulto aparente, contextura, rostro, pómulos, ojos, cejas, nariz, labios, textura de piel, peinado, prendas con materiales y colores, accesorios. Describe únicamente rasgos visibles en referencias, sin inferir atributos sensibles.
- **Wardrobe Lock:** misma vestimenta durante todas las escenas salvo cambio narrativamente justificado y explícito.
- **Short Tag:** 8–12 palabras de rasgos visibles para identificar al personaje en clips (no basta decir «Ana»).
- **Voice Lock:** una descripción invariable de voz (timbre, altura, ritmo) y la frase `speaking natural Latin American Spanish with a neutral Colombian accent`, **solo cuando la herramienta acepte español nativo**. Si no, produce diálogo español mediante narración/locución separada y lip sync disponible en la plataforma, sin inventar soporte.
- Un solo personaje habla por toma cuando sea posible. El que escucha conserva la boca cerrada y no habla.
- No alternes acentos, nombres o ropa entre clips.

## 3. Bloqueo del mundo (World Lock)
Máximo 2 ubicaciones por historia corta. Establece por ubicación: nombre, 3–5 objetos o referencias espaciales, lado izquierdo/derecho, hora, iluminación, clima, props y dirección de cámara. Conserva esta descripción **literal** cuando se repite el escenario. En diálogo a dos, mantén orientación de pantalla y línea de acción, salvo movimiento justificado.

## 4. Estructura temporal y guion
- **30 s**: planteamiento impactante → complicación → giro al 65–75 % → desenlace claro.
- **45 s**: permite más desarrollo sin relleno.
- **60 s**: añade consecuencias y resolución; evita repetir frases y acciones.
- Prefiere clips de **8–10 s**, si VideoExpress lo permite. No asumas que la duración final será idéntica a la suma de clips: los recortes la modifican.
- Diálogo en **español latino** natural, frases cortas y pronunciables: máximo orientativo de 12–16 palabras por 8 s, según velocidad real de la voz y espacio para acciones.
- Cada clip necesita: momento inicial preciso, acción central físicamente posible, gesto/estado final que conecte con el siguiente.
- No más de una acción compleja simultánea; evitar cambios arbitrarios de objetos de mano, teleportaciones y cambios de vestuario.
- Un clip por vez o pequeños grupos cuando el límite de concurrencia lo permita. No inventes resultados.

## 5. Configuración VideoExpress (verificar en interfaz actual)
- `Create with AI → Create Video From Prompt`.
- Image Type: `Photorealistic (Cinematic)`.
- Formato: `Vertical 9:16` o `Landscape 16:9`.
- `Use Consistent Character`: ON cuando esté disponible, con referencias correctas.
- `Use Creative mode`: ON **como configuración sugerida por el playbook original**, pero valida con 1 imagen: en algunas situaciones podría alterar rasgos.
- Image prompt enhancement: OFF.
- Advanced Mode: ON, si existe.
- Video prompt enhancement: OFF; podría reescribir cortes y diálogos.
- Manual Video Length: ON, elegir según la planificación.
- Public gallery: OFF en cada generación.
- Audio: **verifica** compatibilidad real de voces en español latino antes de usar audio nativo. Si no funciona o hay deriva de voz, usa audio separado y lip sync si está disponible, sin doblar el mismo diálogo dos veces.
- No actives narración separada y diálogo nativo simultáneamente.

## 6. Referencias y retratos ancla
1. Si hay fotos reales, sube solo las autorizadas a `Media Library → My Media → Images`; si el agente no puede, pide al usuario que las cargue manualmente.
2. Crea un retrato ancla individual (pecho hacia arriba) para cada personaje con su Biblia, luz natural y ropa fija.
3. Compara rostro con referencia; regenera si cambia el aspecto de forma notable.
4. Guarda ancla mediante `+ Consistent Character` cuando el control exista.
5. Para tomas de un solo personaje, selecciona solamente su ancla. Para dos, selecciona ambas en el orden correcto.
6. Si los personajes son ficticios, usa una imagen original base de cada uno como referencia; no reemplaces personajes por celebridades.

## 7. Formato de los prompts por clip
Cada escena entregará **dos bloques**:

**A. IMAGE PROMPT (English):** fotograma inicial realista: Character Lock literal de cada visible; World Lock literal; encuadre; posición precisa; manos y objetos contados; gesto ya iniciado; luz; no text, no logos, no watermark. En la primera imagen de cada corte, comprueba semejanza.

**B. VIDEO PROMPT (English directions + Spanish dialogue):**
```text
C01 — Photorealistic cinematic scene. [Character Short Tag + wardrobe].
[World Lock]. Vertical 9:16. Seconds 0–3: [specific starting action,
camera and position]. The speaker, [Short Tag], says in natural Latin
American Spanish with a neutral Colombian accent, in the same locked
voice: "[DIÁLOGO CORTO EN ESPAÑOL]". The listener remains silent with
lips closed. Seconds 3–6: A hard cut transitions to [new angle, same
characters and geography; exact coherent action]. Seconds 6–8:
[physical action and ending pose connecting to C02]. Natural room
ambience only; no background music, no subtitles, no onscreen text,
no logos. Keep identity, wardrobe and voice unchanged.
```
- Si se usa audio separado, **elimina la orden de generar voz** del prompt de video; escribe `Visuals and movement only. No voice, no dialogue, no music, no sound effects. Do not generate audio.` y crea la locución española en el flujo de narración, sincronizando después si procede.
- Elimina siempre instrucciones de voces en inglés. «Spanish language» debe definir el idioma hablado; los prompts visuales pueden seguir en inglés.
- No repartas una frase hablada a través de un corte duro.
- Para dos actores: identifica de forma inequívoca quién habla y quién escucha.

## 8. Continuidad de película
Antes de crear C02, anota el último fotograma de C01: posiciones, prop en cada mano, dirección de mirada, puertas, iluminación, distancia y expresión. C02 comienza con un estado compatible.
Revisa cada transición: mismo número de personas, mismo color de ropa, mismo lado del encuadre, objetos no duplicados, manos coherentes, ausencia de objetos que aparezcan/desaparezcan, labios del hablante correctos. Si falla, corrige el clip específico y su prompt, sin reiniciar toda la producción.

## 9. Edición y exportación
Inserta clips C01, C02... en orden. Usa Auto Align Clips si existe, recorta solo pausas iniciales/finales sin eliminar acciones importantes ni cortes internos; verifica duración final, audio y sincronía. Exporta FullHD MP4 cuando esté disponible. Obtén el enlace real desde My Videos y no lo inventes. Las opciones, créditos y retención pueden cambiar.

## 10. Lista breve de control de calidad
- [ ] Todos los diálogos están realmente en español latino, no en inglés.
- [ ] El mismo personaje conserva rostro, edad adulta aparente, cabello y vestuario.
- [ ] Voces consistentes; habla solo quien corresponde; labios sincronizados o audio separado explícito.
- [ ] Escenarios, luz, utilería y orientación coherentes.
- [ ] Cada clip comienza y termina con acciones conectables.
- [ ] Sin subtítulos automáticos, logos ni publicación pública accidental.
- [ ] Duración y exportación verificadas en el resultado, no supuestas.

## 11. Ejemplo de historia original: «El sobre equivocado» (30 s)
**A:** Marina, mujer adulta con cabello negro ondulado a los hombros y chaqueta verde oliva. **B:** Darío, hombre adulto con cabello corto y camisa azul clara. Los detalles definitivos salen de las fotos autorizadas o de referencias ficticias creadas para ambos.
- **C01 (0–8 s), gancho:** En una cafetería, Marina recoge por error un sobre. «Esto no es mío. ¿Por qué tiene mi nombre?».
- **C02 (8–16 s), complicación:** Darío se acerca desde la derecha, sorprendido. «Espera, ese sobre es para otra Marina».
- **C03 (16–24 s), giro:** Ella abre solo la solapa ya desprendida y ve un dibujo infantil con dos nombres iguales. «¿Entonces ella también se llama como yo?».
- **C04 (24–32 s), cierre:** Darío sonríe y señala una mesa cercana. «Sí, es mi hija. Hoy cumple años». Marina devuelve el sobre con alivio y los dos se despiden.
Ajusta diálogos y recortes al tiempo real; conserva mesas, sobre y posiciones de un clip a otro. No generes la escena de abrir correspondencia privada sin consentimiento si se supone que son personas reales.

## 12. Solución de errores
- **Voz inglesa:** no sigas generando; prueba una línea española y determina si el motor soporta voz nativa o requiere narración separada.
- **Rostro distinto:** vuelve al ancla, mejora la foto frontal y la descripción; no amplifiques términos de «belleza».
- **Cambio de voz:** pega el mismo Voice Lock y desactiva autoenhance, o usa una única voz de audio externo consistente.
- **Se mueven ambos labios:** un hablante por clip; oyente con labios cerrados, o encuadra solo al hablante.
- **Sin cortes:** desactiva video enhance y explicita `A hard cut transitions to...`; si no se respeta, divide en clips.
- **Elemento cambia de lado:** revisa el World Lock, la línea de acción y las notas del último fotograma.
- **No hay control del navegador:** entrega prompts y pasos manuales; no solicites permisos amplios por defecto.
