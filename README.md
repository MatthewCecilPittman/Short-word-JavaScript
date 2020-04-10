# Short-word-JavaScript
/* given a string of words,
 return the length of the shortest word(s).*/
function findShort(s){
   const stringArray = s.split(" ");
/*you need to return a number from sort() not a boolean.*/
const orderedArray = stringArray.sort((a, b) => {
return a.length - b.length;
})
/*return the length of the first word(0 index of array)*/
return orderedArray[0].length;
}
