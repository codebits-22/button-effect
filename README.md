cat > README.md << 'EOF'
# Button-Effect

```basR
user@codebits:~$ ./Button-Effect --run
> Animación de botón con HTML y CSS puro
```
# Stack

## Código

**index.html**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="style.css">
    <title>Button</title>
</head>
<body>
    <button>Efecto</button>
</body>
</html>
```

**style.css**
```css
body {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 5rem;
  background: #9987;
}

button {
  width: 150px;
  height: 100px;
  cursor: pointer;
  font-size: 1.4rem;
  color: #fff;
  background: yellowgreen;
  border: none;
  border-radius: 10px;
  box-shadow: 0 10px 10px rgba(0, 0, 0, 0.4);
  transition: 0.5s ease;
}

button:hover {
  background-color: cornflowerblue;
  transform: translateY(-2px);
}

button:active {
  transform: scale(0.7);
}
```

## Cómo funciona

| estado | efecto |
|---|---|
| normal | botón verde (`yellowgreen`) con sombra |
| `:hover` | cambia a azul (`cornflowerblue`) + sube 2px |
| `:active` | se encoge al 70% al hacer clic |

El truco está en `transition: 0.5s ease` — suaviza todos los cambios automáticamente.

## Uso

```bash
git clone https://github.com/codebits-22/button-effect.git
cd button-effect
open index.html
```

## Canal

https://www.youtube.com/@codebits-22

---

> convierte lo que sabes en habilidades reales.
