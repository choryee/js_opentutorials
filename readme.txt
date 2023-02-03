js_opentutorials
https://opentutorials.org/course/3085 https://web-n.github.io/web2_javascript/

집에서 VS Code로 만든것.

생활코딩 Javascript 38강. 1회독 230122

28강부터 다시 복습. ex02.html - 중요 정리됨.

----------------
    for(var key in workers){ //31강
        document.write(key+'<br>');
        document.write(workers[key]+'<br>')
        document.write(key+' : '+workers[key]+'<br>')
    }

workers.showAll=function(){ //이것은 익명함수형태이고, 그것을 왼쪽 객체workers의 변수에 넣은 꼴.
    for(var key in workers){ //32강. 현재 이 함수의 workers와 위 객체workers는 같은 것. 이때, this 사용 가능. 32강 03;31
        document.write(key+' : '+workers[key]+'<br>')
    }
}
workers.showAll();
