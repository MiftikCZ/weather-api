# Miftik's Weather API
> api na počasí pro client-side weby bez nutnosti ověření s API-KEY hodnotou za pomocí DuckDuckGO Weather
#### *tahle api je zatím pouze pro Karlovy Vary*

### main.js
```js
async function getWeather() {
    return await (await fetch("https://Weather-Api-NO-KEY.miftikcz.repl.co")).text();
}

console.log(getWeather());
// 8°

console.log(getWeather() + "C");
// 8°C


console.log("Dnes je " + getWeather() + "C");
// Dnes je 8°C
```
