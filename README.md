# events


const title = document.querySelector("div.hello:first-child h1"); //1. js로 Html element 가져옴 (title)


//3.event가 발생하면 어떤 function을 실행시켜 줌 
function handleTitleClick() {    //handleTitleClick : function이다
    title.style.color = "blue";
}
function handleMouseEnter() {
    title.innerText = "Mouse is here!";
}
function handleMouseLeave() {
    title.innerText = "Mouse is gone!";
}

//2.가져온 element 에 event listener 추가해줌 
title.addEventListener("click", handleTitleClick); 
title.addEventListener("mouseenter", handleMouseEnter); //마우스를 title에 올리면 handleMouseEnter function 실행
title.addEventListener("mouseleave", handleMouseLeave);
![image](https://user-images.githubusercontent.com/85345914/124550892-57743580-de6c-11eb-86e7-5bd71c90e7e0.png)
