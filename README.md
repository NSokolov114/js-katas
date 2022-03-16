# js-katas
Katas mostly from CodeWars  



Testing

[6 kyu] [Srot the inner ctonnet in dsnnieedcg oredr](https://www.codewars.com/kata/5898b4b71d298e51b600014b)

```JS
function sortTheInnerContent(words)
{
  const arr = [];
  
  words.split(' ').forEach(word => {
    const subWord = word.slice(1, -1).split('').sort().reverse().join('');
    const newWord = word[0] + subWord + word[word.length-1];
    
    arr.push(word.length > 3 ? newWord : word);
  });
  
  return arr.join(' ');
}
```
