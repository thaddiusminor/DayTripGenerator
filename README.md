# DayTripGenerator 
"use strict"

function trip(sel){
let Destination = ["london","New York","Ghana","Zambia","Paris" ]  
let random = Math.random() * Destination.length; 
random = Math.floor(random);
console.log(Destination[random]) 
let userInput = prompt( "Are you happy with this Location") 

if(userInput === "no") {
    console.log(Destination[random])
    trip();   
}   

if(userInput === "yes") { 
    console.log("Ok, let's select your food option")  
    food() 
}

}
trip() 

function food() {
    let Resturant = ["Cheesecake Factory","Longhorn Steakhouse", "Dave & Busters","Ruth Chris ", " Burger King"]
    let random = Math.random() * Resturant.length; 
    random = Math.floor(random);
    console.log(Resturant[random]) 
    let userInput = prompt( "Are you happy with this Resuturant") 
    
    if(userInput === "no") {
        console.log(Resturant[random])
        food();   
    }   
    {
    if(userInput === "yes") 
        console.log("Ok, let's select your entertainment")  
        Activity()
    }
    

function Activity(){
    let toDo = ["hiking","Beach Visit","Sky Diving","Car Racing","Go Carting" ] 
    
   
    
    let random = Math.random() * toDo.length; 
    random = Math.floor(random);
    console.log(toDo[random]) 
    let userInput = prompt( "Are you happy with this form of entertainment") 
    
    if(userInput === "no") {
        console.log(toDo[random])
        Activity();   
    }   
    if(userInput === "yes") { 
        console.log("All set")  
     } 
} 
   console.log("Your Trip is now Complete") 
}
