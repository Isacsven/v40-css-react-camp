## Hur kopplas CSS in i React?

CSS filen måste kopplas till `App.jsx`, annars laddas aldrig reglerna, vilket man gör genom att importera modulen med `import "./App.css"`. `className` är klassnamnen på elementen, vilket används i CSS för att skapa reglerna och stila elementen.

## Hur ser användaren vilka todos som är klara?

Användaren ser vilka todos som är klara genom `.completed` klassen, vilket lägger till en genomstrykning.
Den här klassen styrs genom `todo.done` state, i ett ternary villkor på varje `li` element. Om ett todo element är klar, läggs både `.todo` och `.completed` klassen till. Det är alltså inte state själv, utan en etikett som läggs till beroende på vad `todo.done` är.

## Tre steg när stil inte tar

Spara filen -> kolla att `App.jsx` importerar CSS -> kolla att JSX taggarna har `className` egenskaper för klassnamnen i CSS filen -> använd konsolen i Dev Tools för att inspektera elementen och se klasserna.