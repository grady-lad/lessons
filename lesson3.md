# Objects 

 ## Exercise 1


Implement a Music Box object that should make the following code work well:

```` javascript


(function() {
// Write your code here  

  var box = MusicBox(),
      a1 = Album("The Who", "Tommy"),
      a2 = Album("Tom Waits", "Closing Time"),
      a3 = Album("John Cale", "Paris 1919"),
      favorite;
 
  box.addAlbum(a1);
  box.addAlbum(a2);
  box.addAlbum(a3);
 
  a1.play() ; // prints "Playing The Who - Tommy"
  a2.play(); // prints "Playing Tom Waits - Closing Time"  
  a1.play(); // prints "Playing The Who - Tommy"
 
  favorite = box.favoriteAlbum(); 
 
  // prints "favorite album is The Who - Tommy"
  console.log("favorite album is " + favorite); 
 
}());


````
 ## Exercise 2

Implement a Music Box object that should make the following code work well:

```` javascript

(function () {
  // Code goes here

  var album = PhotoAlbum(),
      p1, p2, p3;
 
  p1 = Photo("Paris Trip 1");
  p1.tag("Jimmy");
  p1.tag("Jane");
  p1.tag("Jeff");
 
  album.addPicture(p1);
 
  p2 = Photo("Look the Eiffel");
  p2.tag("Jimmy");
  p2.tag("Max");
  album.addPicture(p2);
 
  p3 = Photo("OMG it's so high");
  p3.tag("Jimmy");
  p3.tag("Jane");
 
  // prints "Jimmy, Jane"
  p3.showTags();
 
  album.addPicture(p3);
 
  // prints "Paris Trip 1, Look the Eiffel, OMG it's so high"
  album.showPictures("Jimmy");
 
  // prints "Paris Trip 1, OMG it's so high"
  album.showPictures("Jane");    
}());

````


 ## Exercise 3
  
  ### arrayToObject
  
  Imagine we have an array of numbers from 0 to 9 like the array below
  
  ```` javascript
   var arr = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
  ````
  Write a function that transforms this array to a object. 
  
  The resulting object should have the word representation of the number as the key and the actual number as the value.
  
  So given an array of `[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]` the result should be:
  
  ````
  {
   zero: 0,
   one: 1,
   two,: 2,
   three: 3,
   four: 4,
   five: 5,
   six: 6,
   seven: 7,
   eight: 8,
   nine: 9
  }
  ````
  
