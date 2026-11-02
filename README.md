# Cotizador de seguros

A small React form for a car insurance quote calculator ("cotizador de seguros"), built as a learning exercise. The UI text is in Spanish.

## Context

Built in September 2020 (two commits, 3 and 5 September) while learning React hooks and CSS-in-JS. It was bootstrapped with Create React App and never finished.

## What it does

- A header and a form with three fields: car origin (American, European, Asian), model year (2012 to 2021) and plan (basic or full).
- Form state is held in a single `useState` object; submitting with an empty field shows a "all fields are required" error.
- Styling uses `@emotion/styled` components.

What it does not do: the quote calculation is not implemented. `src/components/Formulario.js` only contains the planned rules as comments (a 3% discount per year of age, a surcharge by car origin, and a surcharge by plan). The plan radio buttons also have attribute typos (`nme` and `check` instead of `name` and `checked`), and the "Completo" radio button has `value="basico"` instead of `"completo"`, so the plan value is never set and the form cannot pass validation as committed.

## Stack

React 16 (function components, `useState`), Emotion 10, Create React App (`react-scripts` 3.4.3). No tests beyond the CRA default setup file.

## Running it

```bash
npm install
npm start   # http://localhost:3000
```

`react-scripts` 3.x uses webpack 4, which may need an older Node.js version (16 or earlier) to start.

## Status

Archived learning project, unfinished and not maintained.
