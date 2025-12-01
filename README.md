# tars brand-assets

Repositorio listo para organizar y distribuir todos los activos visuales de la marca. Incluye estructura escalable, documentación clara y ejemplos de uso.

---

## Estructura del proyecto

```
brand-assets/
  README.md
  LICENSE
  logos/
    light/
      tars-logo-light.svg
    dark/
      tars-logo-dark.svg
  examples/
    react-example.jsx
```

---

## README.md

```md
# Brand Assets

Este repositorio centraliza los logos y activos visuales de la marca. Diseñado para servirlos públicamente mediante GitHub Raw o CDNs.

## Estructura

- `logos/light/` → Logos para fondos oscuros.
- `logos/dark/` → Logos para fondos claros.
- `examples/` → Ejemplos de uso en distintos entornos.

## Uso directo con GitHub Raw

### Logo Light
```

[https://raw.githubusercontent.com/](https://raw.githubusercontent.com/)<USER>/brand-assets/main/logos/light/tars-logo-light.svg

```

### Logo Dark
```

[https://raw.githubusercontent.com/](https://raw.githubusercontent.com/)<USER>/brand-assets/main/logos/dark/tars-logo-dark.svg

````

## Ejemplo en React

```jsx
<img
  alt="Tars Logo"
  width={200}
  src="https://raw.githubusercontent.com/<USER>/brand-assets/main/logos/light/tars-logo-light.svg"
/>
````

## Cache Busting

Agregar un query param para forzar nueva versión:

```
...?v=2
```

## Licencia

Ver archivo LICENSE.

````

---

## LICENSE (MIT)
```txt
MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
````

---

## examples/react-example.jsx

```jsx
export default function LogoExample() {
  return (
    <div style={{ padding: 20 }}>
      <h1>Ejemplo de uso del logo</h1>
      <img
        alt="Tars Logo"
        width={200}
        src="https://raw.githubusercontent.com/<USER>/brand-assets/main/logos/light/tars-logo-light.svg"
      />
    </div>
  );
}
```

---

### Instrucciones para crear el repo

```sh
git init
git add .
git commit -m "Initial brand assets repo"
git branch -M main
git remote add origin git@github.com:<USER>/brand-assets.git
git push -u origin main
```
