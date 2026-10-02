# Categorias de Conteúdo HTML5

## Elementos de bloco

Os elementos de bloco ocupam toda a largura disponível.

**Exemplos:**
- `<div>`
- `<p>`
- `<h1>`
- `<select>`
- `<article>`

---

## Elementos de linha

Os elementos de linha ocupam apenas o espaço necessário na linha.

**Exemplos:**
- `<a>`
- `<span>`
- `<strong>`
- `<em>`
- `<img>`

---

## Regras importantes

Elementos de linha **não devem conter elementos de bloco**.

### Exemplo incorreto

```html
<span>
    <div>Texto</div>
</span>
```