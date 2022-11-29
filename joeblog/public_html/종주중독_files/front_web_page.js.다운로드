let target = document.querySelector("#dynamic");


function randomString(){
    let stringArr = ["Learn to HTML" , "Learn to Javascript"];
    let selectString = stringArr[Math.floor(Math.random()*stringArr.length)];
    let selectStringArr =selectString.split("");
    return selectStringArr;
//타이핑 리셋
function resetTyping(){
    target.textContent="";
    dynamic(randomString());
}

//한글자씩 텍스트 출력 함수 

function dynamic(randomArr){
    if(randomArr.length>0){
        target.textContent += randomArr.shift();
        setTimeout(function(){
            dynamic(randomArr);
        },80);
    }
    else{
        setTimeout(resetTyping, 3000);

    }
}
dynamic(randomString());

function blink(){
  target.classList.toggle("active");
  //p -> dynamic id 태그에 active class를 붙였다가 땠다가
}
setInterval(blink, 500); }