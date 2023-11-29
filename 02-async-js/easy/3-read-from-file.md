## Reading the contents of a file
const fs = require("fs");

function fn(err, data){
  if(err){
    console.log(err);
  }
  else{
    console.log(data);
  }
}

fs.readFile("data.txt", 'utf-8', fn);
var sum = 0;
for(let i = 0; i < 10000000; i++){
  sum+=i;
}
Write code to read contents of a file and print it to the console. 
You can use the fs library to as a black box, the goal is to understand async tasks. 
Try to do an expensive operation below the file read and see how it affects the output. 
Make the expensive operation more and more expensive and see how it affects the output. 

