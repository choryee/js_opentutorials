# js_opentutorials
https://opentutorials.org/course/3085
https://web-n.github.io/web2_javascript/

생활코딩 Javascript 38강. 1회독 230122

28강부터 다시 복습.
ex02.html  - 중요 정리됨.

------
<body>
   <script> 
        var names=["john", "lee", "kim"];
</script>
   
<ul> 
<script> 
    var i=0;
    while(i<names.length){
        document.write('<li>'+names[i]+'</li>')
       //  alert('>>>>>', names[i]) 
        i++;
        }
    
</script>
</ul>

<script>
    function add(a,b){
        return a+b;
    }
    document.write(add(3,4)+'<br>');
    document.write('<div style="color:red; font-size:3rem; background-color:green;">'+add(7,8)+'</div><br>')

    var sum=(a,b)=>{a*b};
    document.write('>>>>'+sum(4,5)+'<br>')

    //30강.
    var workers={
        "programer":"egoing",
        "chef":"back",
        "pilot":"John"
    }

    function obj(){
        var i=0;
        while(i<workers.length){
            alert('haha')
            document.write('<div style="color:blue;">'+workers.programer+'</div><br>')
        }
    }
    obj();

  
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
----------------
