import React from "react";
import  ReactDOM  from "react-dom";


const date =new Date();
const currentTime=date.getHours();
console.log(currentTime);
let greeting;
const customStyle={
  color:""
}

if(currentTime<12){
  greeting="good morning"
  customStyle.color="red";
}
else if(currentTime <18)
{
greeting="good evening"
customStyle.color="green";
}
else{

  greeting="good night"
  customStyle.color="blue";
}



ReactDOM.render(


<h1 style={customStyle}>

{greeting}

</h1>
 






  ,
  document.getElementById("root")
)
