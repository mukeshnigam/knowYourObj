# knowYourObj
const descripter = Object.getOwnPropertyDescriptor(Math,"PI")
console.log(descripter);
console.log(Math.PI);
Math.PI = 9.18
console.log(Math.PI);

const tea = {
    name: 'black tea',
    price: 50,
    isAvilable: true,

ordertea: function(){
    console.log("tea is not presnt");
    }

}
console.log(Object.getOwnPropertyDescriptor(tea,"name"));

//********to define object********

// Object.defineProperty(tea, "name"{
//     writable:false,
//     enumerable: false,
//     configurable: false,
// })

for (let [key,value] of Object.entries(tea)) {
    if (typeof value !== 'function') {
    console.log(`${key},${value}`);
    }
}
