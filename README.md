# Teardown

Galería de simuladores 3D interactivos de obras reales, armados a partir de los planos.
Cada simulador muestra la obra construyéndose capa por capa.

Se publica en `teskel.online/teardown`.

## Estructura

```
index.html          galería: lee modelos.json y arma una tarjeta por modelo
modelos.json        única fuente de datos de la galería
portadas/<ID>.jpg   captura 1600×900, menos de 200 KB
<ID>/index.html     simulador autocontenido (se sube tal cual, no se edita)
```

## Agregar un modelo

1. Subir `<ID>/index.html`.
2. Subir `portadas/<ID>.jpg`.
3. Agregar la entrada en `modelos.json`.
4. Abrir `<sitio>/<ID>/` y comprobar que carga y que arranca el recorrido automático.

La galería no se toca: se arma sola a partir de `modelos.json`.
