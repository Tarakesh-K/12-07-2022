1st Question

var obj={

  "name":"johndoe",
  
  "age":"23",
  
  "year":"2018"
  
};


Getting the request,

var request = new XMLHttpRequest();

request.open("GET","https://raw.githubusercontent.com/rvsp/restcountries-json-data/master/res-countries.json");

request.send();

request.onload=function(){

    var result = JSON.parse(request.response);
    
    console.log(result);
    
    for(var i=0;i<result.length;i++){  
    
        console.log(result[i].name);
        
    }
    
}


for in loop JSON,

for(var key in obj){

  console.log(key,obj[key]);
  
}


for of loop,

for (let [key, value] of Object.entries(obj)) {

  console.log(key, value);
  
}


for each loop,

Object.entries(obj).forEach(([key, value]) => {

  console.log(`${key} ${value}`);
  
});


2nd Question

var resume = {

  "FirstName":"Tarakesh",
  
  "LastName":"K",
  
  "Role":"Developer",
  
  "Experience":"0 Years",
  
  "Languages":"English, Tamil",
  
  "Education":"B.E",
  
};


3rd Question

Window is the main JavaScript object root, aka the global object in a browser, and it can also be treated as the root of the document object model. You can access it as window.

window.screen or just screen is a small information object about physical screen dimensions like mentioning the width and height of the screen.

window.document or just document is the main object of the potentially visible (or better yet: rendered) document object model/DOM.
