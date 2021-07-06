# events

 //1. js로 Html element 가져옴 (title)
 
 
const title = document.querySelector("div.hello:first-child h1");



//3.event가 발생하면 어떤 function을 실행시켜 줌 

//handleTitleClick : function이다


function handleTitleClick() {

    title.style.color = "blue";
}

function handleMouseEnter() {

    title.innerText = "Mouse is here!";
    
}

function handleMouseLeave() {

    title.innerText = "Mouse is gone!";
    
}

//2.가져온 element 에 event listener 추가해줌 

//마우스를 title에 올리면 function 실행


title.addEventListener("click", handleTitleClick); 

title.addEventListener("mouseenter", handleMouseEnter); 

title.addEventListener("mouseleave", handleMouseLeave);
