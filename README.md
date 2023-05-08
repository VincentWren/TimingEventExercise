# TimingEventExercise

setTimeout(() => {
    const first = document.createElement(`p`);
    first.innerText = `Hi`;
  }, 1000);

setTimeout(() => {
    const one = document.createElement(`p`);
    one.innerText = `timeout-nesting`;
    const two = document.querySelector(`#timeout-nesting`);
    two.insertAdjacentElement(`afterbegin`, two);
  
  }, 1000);
}, 3000);

let number = 1;
setInterval(() => {
  console.log(number);
  number++;
}, 1000)

let num = 10;
const countdown = setInterval(() => {
  if (num > 0) {
    console.log(num);
  } else {
    console.log(num);
    clearInterval(countdown);
  }
  num--;
});

// ;-;
