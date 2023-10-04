let CelsiusInput = document.querySelector('#Celsius > input');
let FahrenheitInput = document.querySelector('#Fahrenheit > input');
let KelvinInput = document.querySelector('#Kelvin > input');

let btn = document.querySelector('.button button');


function roundnumber(number){
    return Math.round(number*100)/100
}
/*Celsius to fahrenheit and kelvin */
CelsiusInput.addEventListener('input', function(){
    let CTemp = parseFloat(CelsiusInput.value)
    let FTemp = (CTemp*(9/5)) + 32
    let KTemp= CTemp + 273.15

    FahrenheitInput.value = roundnumber(FTemp)
    KelvinInput.value = roundnumber(KTemp)
})
/*fahrenehit to celsius and kelvin */
FahrenheitInput.addEventListener('input', function(){
    let FTemp = parseFloat(FahrenheitInput.value)
    let CTemp = (FTemp-32)*(5/9)
    let KTemp = (FTemp-32)*(5/9)+273.15

    CelsiusInput.value = roundnumber(CTemp)
    KelvinInput.value = roundnumber(KTemp)
})

/* kelvin to celsius and fahrenheit */
KelvinInput.addEventListener('input', function(){
    let KTemp = parseFloat(KelvinInput.value)
    let CTemp = KTemp - 273.15
    let FTemp = (KTemp-273.15)*(9/5)+32

    CelsiusInput.value = roundnumber(CTemp)
    FahrenheitInput.value = roundnumber(FTemp)
})

btn.addEventListener('click',()=>{
    CelsiusInput.value = ""
    FahrenheitInput.value = ""
    KelvinInput.value = ""
})