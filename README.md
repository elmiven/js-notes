html preview:  
https://htmlpreview.github.io/?https://github.com/elmiven/js-notes/blob/main/index.html  

[https://raw.githack.com/elmiven/js-notes/main/index.html](https://rawcdn.githack.com/elmiven/js-notes/63036a337177ea3e8c8f7142ca021073b49c27d0/index.html)



### Using Objects for Lookups  
Objects can be thought of as a key/value storage, like a dictionary. If you have tabular data, you can use an object to lookup values rather than a switch statement or an if/else chain. This is most useful when you know that your input data is limited to a certain range.  

```js
const article = {
  "title": "How to create objects in JavaScript",
  "link": "https://www.site.com",
  "author": "Kaashan Hussain",
  "language": "JavaScript",
  "tags": "TECHNOLOGY",
  "createdAt": "NOVEMBER 28, 2018"
};

const articleAuthor = article["author"];
const articleLink = article["link"];

const value = "title";
const valueLookup = article[value];

```



### Record Collection 
You are given an object literal representing a part of your musical album collection. Each album has a unique id number as its key and several other properties. Not all albums have complete information.
          
You start with an updateRecords function that takes an object literal, records, containing the musical album collection, an id, a prop (like artist or tracks), and a value. Complete the function using the rules below to modify the object passed to the function.
          
Your function must always return the entire record collection object.  
If prop isn't tracks and value isn't an empty string, update or set that album's prop to value.  
If prop is tracks but the album doesn't have a tracks property, create an empty array and add value to it.  
If prop is tracks and value isn't an empty string, add value to the end of the album's existing tracks array.  
If value is an empty string, delete the given prop property from the album.
          
Note: A copy of the recordCollection object is used for the tests.
  
```js
    const recordCollection = {
      2548: {
        albumTitle: 'Slippery When Wet',
        artist: 'Bon Jovi',
        tracks: ['Let It Rock', 'You Give Love a Bad Name']
      },
      2468: {
        albumTitle: '1999',
        artist: 'Prince',
        tracks: ['1999', 'Little Red Corvette']
      },
      1245: {
        artist: 'Robert Palmer',
        tracks: []
      },
      5439: {
        albumTitle: 'ABBA Gold'
      }
    };
    
    // Only change code below this line
    function updateRecords(records, id, prop, value) {
      return records;
    }
    
    updateRecords(recordCollection, 5439, 'artist', 'ABBA');
```



### Recursion


