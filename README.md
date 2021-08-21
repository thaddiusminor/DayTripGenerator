# DayTripGenerator 
"use strict"

function trip(){
let Destination = ["london","New York","Ghana","Zambia","Paris" ] 

let yes = true 
let no = false 

let random = Math.random() * Destination.length; 
random = Math.floor(random);
console.log(Destination[random]) 
let userInput = prompt( "Are you happy with this Location") 

while(userInput === "no") {
    console.log(Destination[random])
    trip();   
}   

if(userInput === "yes") { 
    console.log("Congrats!!")  
}

}
trip() 

function food() {
    let Resturant = ["Cheesecake Factory","Longhorn Steakhouse", "Dave & Busters","Ruth Chris ", " Burger King"]
     
    let yes = true 
     let no = false 

    let random = Math.random() * Resturant.length; 
    random = Math.floor(random);
    console.log(Resturant[random]) 
    let userInput = prompt( "Are you happy with this Resuturant") 
    
    while(userInput == "no") {
        console.log(Resturant[random])
        food();   
    }   
    
    if(userInput == "yes") { 
        console.log("Whoop Whoop!!")  
    }
    
    }
    food() 
