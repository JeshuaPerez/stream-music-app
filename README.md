# MusicStream

Interfaz completa de una plataforma de streaming y venta de música: siete
pantallas que cubren el recorrido entero del usuario, desde descubrir un álbum
hasta pagarlo. Maquetadas a mano con HTML5 semántico y CSS3, sin frameworks,
sin plantillas y sin librerías.

El reto era replicar un diseño dado respetando la estructura semántica. Lo tomé
como ejercicio de disciplina: nada de `div` para todo, cada región de la página
con la etiqueta que le corresponde.

## Pantallas

| Página | Qué resuelve |
|---|---|
| `index.html` | Portada: artista destacado, novedades de la semana y los temas más vendidos |
| `album-detail.html` | Ficha del álbum con su lista de canciones |
| `player.html` | Reproductor con la pista en curso |
| `cart.html` | Carrito con el resumen del pedido |
| `checkout.html` | Método de pago y dirección de facturación |
| `profile.html` | Biblioteca del usuario y confirmación de compra |

## Cómo está construido

- **HTML5 semántico**: 6 `main`, 6 `header`, 6 `nav`, 10 `section`, 8 `article`
  y 4 `aside` repartidos entre las páginas. La estructura se entiende leyendo
  el marcado, sin necesidad de abrir los estilos.
- **CSS separado por responsabilidad**, en lugar de un archivo único:

  | Archivo | Contiene |
  |---|---|
  | `css/main.css` | Reset y bases |
  | `css/layout.css` | Estructura y disposición de cada pantalla |
  | `css/components.css` | Piezas reutilizables: tarjetas, botones, navegación |

- **Diseño adaptable** a pantallas de celular.

## Estructura

```
index.html          Portada
album-detail.html   Detalle del álbum
player.html         Reproductor
cart.html           Carrito
checkout.html       Pago
profile.html        Perfil y biblioteca
css/                main.css · layout.css · components.css
assets/             Portadas, imágenes y favicon
```

## Cómo verlo

No necesita instalación ni servidor:

```bash
git clone https://github.com/JeshuaPerez/stream-music-app.git
cd stream-music-app
```

Abre `index.html` en cualquier navegador.

## Alcance

Es un proyecto de maquetación: no lleva JavaScript, así que el carrito, el
reproductor y el pago son la interfaz, no la funcionalidad. Para ver trabajo con
lógica y datos, mira
[FoodieRank](https://github.com/JeshuaPerez/FoodieRank-backend) (API REST con
Node.js y MongoDB) o
[Gestión de inmuebles](https://github.com/JeshuaPerez/gestion-inmuebles) (CRUD
en JavaScript).

## Nota sobre el contenido

Las portadas de álbum y el nombre de la banda pertenecen a sus respectivos
dueños y se usan únicamente con fines educativos, dentro de un ejercicio
académico sin fin comercial.

---

Jeshua Pérez · [Portafolio](https://jeshuaperez.github.io/portafolio/) · [GitHub](https://github.com/JeshuaPerez)
