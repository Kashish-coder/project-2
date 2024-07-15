```
//BMI calculator
document.querySelector('form'); //form is accessed
form.addEventListener('submit', function (e) {
  e.preventDefault();
  //values are taken inside form
  const h = parseInt(document.querySelector('#height').value);
  const w = parseInt(document.querySelector('#weight').value);
  const r = document.querySelector('#resultst').value;
  if (height === '' || height < 0 || isNAN(height)) {
    //to add height
    results.innerHTML = 'Please give a valid height';
  }
 else if (weight === '' || weight < 0 || isNAN(weight)) {
    //to add height
    results.innerHTML = 'Please give a valid height';
  }
  else{
 const bmi= (weight /((height*height)/10000)).toFixed(2)  ;
 //show result
 results.innerHTML=`<span>${bmi}</span>`

  }

});
```