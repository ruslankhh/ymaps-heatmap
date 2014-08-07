Canvas
===

Модуль отрисовки тепловой карты на canvas'e. Позволяет получить карту в формате dataURL.

Canvas(size) 
-----------------------------
Конструктор модуля отрисовки тепловой карты.

**Parameters**

**size**: Array.&lt;Number&gt;, Размер карты: [width, height].


getBrushRadius() 
-----------------------------
Получение размера кисти, которая используется для отрисовки точек.

**Returns**: Number, margin.

generateDataURLHeatmap(points) 
-----------------------------
Получение карты в виде dataURL с нанесенными точками.

**Parameters**

**points**: Array.&lt;Object&gt;, Массив точек [[x1, y1], [x2, y2], ...].

**Returns**: String, dataURL.

destroy() 
-----------------------------
Уничтожает внутренние данные.


_setupOptionMonitor() 
-----------------------------
Устанавливает монитор на опции тепловой карты.

**Returns**: Monitor, Монитор опций.

_destroyOptionMonitor() 
-----------------------------
Уничтожает монитор опций.


_setupDrawTools() 
-----------------------------
Устанавливает внутренние опции тепловой карты.

**Returns**: Canvas, Устанавливает внутренние опции тепловой карты.

_destroyDrawTools() 
-----------------------------
Уничтожает внутренние опции тепловой карты.


_createBrush() 
-----------------------------
Создание кисти, которой будут нарисованы точки.

**Returns**: HTMLElement, brush Канвас с отрисованной тенью круга.

_createGradient() 
-----------------------------
Создание 256x1 градиента, которым будет раскрашена карта.

**Returns**: Array.&lt;Number&gt;, [r1, g1, b1, a1, r2, ...].

_drawHeatmap() 
-----------------------------
Отрисовка тепловой карты.

**Returns**: Canvas, Отрисовка тепловой карты.

_colorize(pixels, gradient) 
-----------------------------
Раскрашивание пикселей карты.

**Parameters**

**pixels**: Array.&lt;Number&gt;, Бесцветная тепловая карта [r1, g1, b1, a1, r2, ...].

**gradient**: Array.&lt;Number&gt;, Градиент [r1, g1, b1, a1, r2, ...].