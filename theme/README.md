# How do I detect dark mode using JavaScript?

<https://stackoverflow.com/a/57795495/5676460>

``` javascript
const darkModeMql = window.matchMedia && window.matchMedia('(prefers-color-scheme: dark)');

if (darkModeMql && darkModeMql.matches) {
  // dark mode
} else {
  // light mode
}
```


chatgpt

``` javascript
const theme =
    window.matchMedia("(prefers-color-scheme: dark)").matches
        ? "dark"
        : "light";

document.documentElement.setAttribute(
    "data-theme",
    theme
);
```
