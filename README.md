# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)
## ImaginaryNumber module

The project includes a small utility class in `src/assets/imaginary.js` for working with complex numbers.

### What it provides

- `ImaginaryNumber([real = 0, imaginary = 0])` — construct a complex number.
- `toString()` — get a human-readable form like `3 + 2i`, `i`, `-i`, or `0`.
- `display()` — alias of `toString()`.
- `multiply(factors)` — multiply by one or more complex numbers.
- `addition(numbers)` — add one or more complex numbers.
- `subtract(numbers)` — subtract one or more complex numbers.
- `division(divisors)` — divide by one or more complex numbers (throws on division by zero).
- `sqrt()` — compute a square root of the complex number.
- `toPolar()` — convert to polar form, returning `modulus`, `rad`, and `deg`.

### Example

```js
import ImaginaryNumber from './src/assets/imaginary.js';

const z = new ImaginaryNumber([3, -1]);
console.log(z.toString()); // "3 - i"

const w = new ImaginaryNumber([1, 2]);
const product = z.multiply([w]);
console.log(product.toString()); // "5 + 5i"

const polar = z.toPolar();
console.log(`${polar.modulus.toFixed(2)} ∠ ${polar.deg.toFixed(2)}°`);
```

### Notes

- The class is intentionally lightweight and suitable for simple complex-number calculations.
- The `division()` method validates the denominator and throws an error if a divisor is zero.
- If you use this class from a React app, import it with the correct relative path from the file where you need it.
## React Compiler

The React Compiler is enabled on this template. See [this documentation](https://react.dev/learn/react-compiler) for more information.

Note: This will impact Vite dev & build performances.

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
































































# Contando Vidas Salvando Almas
official animal shelter website
I am still building this thing, if you want to see the interfaces here´s a link to the figma project:
https://www.figma.com/design/78Rt1nDJlow2VpV5ioLRnI/Sin-t%C3%ADtulo?node-id=0-1&t=o7acsWc73o1xKh4Q-1 
--------- by carlos_rtx
