# jQuery_Tutorial
Special Thanks To MR. Shubham Sir and  MR. Gaurav Sir ❤❤




//SELECTOR
<!DOCTYPE html>
<html>
<head>
<script src="jquery-3.2.1.min.js"></script>
<script>
$(document).ready(function(){
  $("#hide").click(function(){
    $("p").hide();
  });
  $("#show").click(function(){
    $("p").show();
  });
  $(".C1").click(function(){
    $("p").hide();
  };

});
</script>
</head>

    <body>
        <div>Click on this to see a dialogue box.</div>
        <p></p>
        <ol>
            <li id="sh">shuhbham</li>
            <li id="gt">gaurav</li>
            <li id="pp">pratik patel</li>
            <li  id="aa">aaryan</li>
            <li  id="om">Omkar</li>
            <li  id="pr">Prathamesh</li>
        </ol>
        <table>
        <tr>
            <th>sr no</th>
            <th>Name</th>
            <th>Roll No</th>
        </tr>
        <tr>
            <td>01</td>
            <td>Gaurav</td>
            <td>A052</td>
        </tr>
        <tr>
            <td>02</td>
            <td>Shubham</td>
            <td>A036</td>
        </tr><tr>
          <td>03</td>
          <td>Omkar</td>
          <td>A009</td>
        </tr>
        </table>
        <p>This paragraph is the first child of its parent (body).</p>
        <p>This paragraph is not the first child of its parent (body).</p>
        
        <div>
          <p>This paragraph is the 1first child of its parent (div).</p>
          <p>This paragraph is not the first child of its parent (div).</p>
        </div>
        
        <div>
            <p>This paragraph is the 2first child of its parent (div).</p>
            <p>This paragraph is not the first child of its parent (div).</p>
          </div>
        
          <div>
            <p>This paragraph is the 3first child of its parent (div).</p>
            <p>This paragraph is not the first child of its parent (div).</p>
        
          </div>
        
          
        <p class="C1">If you click on the "next" button, i will disappear.</p>
        
        <button id="next">next</button>
        <button id="back">back</button>
        
        
        </body>
        </html>










//HIDE() AND SHOW()

<!doctype html>
<html>
<head>
<title>The jQuery Example</title>
<script src="jquery-3.2.1.min.js"></script>
<script>
   $(document).ready(function() {
      $("li:first,li:last,p:first-of-type").click(function() {alert("Hello, world!");});
      $("p").click(function(){
  $(this).hide();
  });
      $(".C1").click(function(){
        $(".C1").hide();
      });
      $("#next").click(function(){
        $("p").hide();
      });
      $("#back").click(function(){
        $("p").show();
      });

  $("tr").dblclick(function(){
  $(this).hide();
});
$("#sh").mouseenter(function(){
  alert("You entered Shubham!");
});
$("#gt").mouseleave(function(){
  alert("Bye! You now leave Gaurav!");
})
$("#pp").mousedown(function(){
  alert("Mouse down over Patel!");
});
$("#aa").mousedown(function(){
  alert("Mouse down over Aryan!");
});
$("#tr").hover(function(){
  alert("You entered Omkar!");
},
function(){
  alert("Bye! You now leave Omkar!");
});
$("#pr").focus(function(){
  $(this).css("background-color", "#cccccc");
});



   });
</script>
</head>
<body>
<div>Click on this to see a dialogue box.</div>
<p></p>
<ol>
    <li id="sh">shuhbham</li>
    <li id="gt">gaurav</li>
    <li id="pp">pratik patel</li>
    <li  id="aa">aaryan</li>
    <li  id="om">Omkar</li>
    <li  id="pr">Prathamesh</li>
</ol>
<table>
<tr>
    <th>sr no</th>
    <th>Name</th>
    <th>Roll No</th>
</tr>
<tr>
    <td>01</td>
    <td>Gaurav</td>
    <td>A052</td>
</tr>
<tr>
    <td>02</td>
    <td>Shubham</td>
    <td>A036</td>
</tr><tr>
  <td>03</td>
  <td>Omkar</td>
  <td>A009</td>
</tr>
</table>
<p>This paragraph is the first child of its parent (body).</p>
<p>This paragraph is not the first child of its parent (body).</p>

<div>
  <p>This paragraph is the 1first child of its parent (div).</p>
  <p>This paragraph is not the first child of its parent (div).</p>
</div>

<div>
    <p>This paragraph is the 2first child of its parent (div).</p>
    <p>This paragraph is not the first child of its parent (div).</p>
  </div>

  <div>
    <p>This paragraph is the 3first child of its parent (div).</p>
    <p>This paragraph is not the first child of its parent (div).</p>

  </div>

  
<p class="C1">If you click on the "next" button, i will disappear.</p>

<button id="next">next</button>
<button id="back">back</button>


</body>
</html>




//SLIDE TOGGLE
<!DOCTYPE html>
<html>
<head>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.4/jquery.min.js"></script>
<script> 
$(document).ready(function(){
  $("#flip").click(function(){
    $("#panel").slideToggle("slow");
  });
});
</script>
<style> 
#panel, #flip {
  padding: 5px;
  text-align: center;
  background-color:orange;
  border: solid 1px white;
}

#panel {
  padding: 50px;
  display: none;
}
</style>
</head>
<body>
 
<div id="flip">Click to slide the panel down or up</div>
<div id="panel">Hello world!</div>

</body>
</html>






//FADE 
<!DOCTYPE html>
<html>
<head>
<script src="jquery-3.2.1.min.js"></script>
<script>
$(document).ready(function(){
  $("#b1").click(function(){
    $("#div1").fadeIn();
    $("#div2").fadeIn("slow");
    $("#div3").fadeIn(3000);
  });
  $("#b2").click(function(){
    $("#div1").fadeOut();
    $("#div2").fadeOut("slow");
    $("#div3").fadeOut(3000);
  });
});
</script>
</head>
<body>

<p>Demonstrate fadeIn() and fadeOut() with different parameters.</p>

<button id="b1">Click to fade in boxes</button><br><br>
<button id="b2">Click to fade out boxes</button><br><br>

<div id="div1" style="width:2000px;height:200px;display:none;background-color:orange;"></div><br>
<div id="div2" style="width:2000px;height:200px;display:none;background-color:white;"></div><br>
<div id="div3" style="width:2000px;height:200px;display:none;background-color:green;"></div>

</body>
</html>



//FADE TOGGLE FUNCTION
<!DOCTYPE html>
<html>
<head>
<script src="jquery-3.2.1.min.js"></script>
<script>
$(document).ready(function(){
  $("button").click(function(){
    $("#fa1").fadeToggle();
    $("#fa2").fadeToggle("slow");
    $("#fa3").fadeToggle(3000);
  });
});
</script>
</head>
<body>

<p>Demonstrate fadeToggle() with different speed parameters.</p>

<button>Click to fade in/out boxes</button><br><br>

<div id="fa1" style="width:2000px;height:200px;background-color:orange;"></div>


<div id="fa2" style="width:2000px;height:200px;background-color:white;"></div>
<br>
<div id="fa3" style="width:2000px;height:200px;background-color:green;"></div>

</body>
</html>

//Event handling 
//Mouse Event
<!doctype html>
<html>
<head>
<title>The jQuery Example</title>
<script src="jquery-3.2.1.min.js"></script>
<script>
   $(document).ready(function() {
      $("li:first,li:last,p:first-of-type").click(function() {alert("Hello, world!");});
      $("p").click(function(){
  $(this).hide();
  });
  $("tr").dblclick(function(){
  $(this).hide();
});
$("#sh").mouseenter(function(){
  alert("You entered Shubham!");
});
$("#gt").mouseleave(function(){
  alert("Bye! You now leave Gaurav!");
})
$("#pp").mousedown(function(){
  alert("Mouse down over Patel!");
});
$("#aa").mousedown(function(){
  alert("Mouse down over Aryan!");
});

   });
</script>
</head>
<body>
<div>Click on this to see a dialogue box.</div>
<p></p>
<ol>
    <li id="sh">shuhbham</li>
    <li id="gt">gaurav</li>
    <li id="pp">pratik patel</li>
    <li  id="aa">aaryan</li>
</ol>
<table>
<tr>
    <th>sr no</th>
    <th>Name</th>
    <th>Roll No</th>
</tr>
<tr>
    <td>01</td>
    <td>Gaurav</td>
    <td>A052</td>
</tr>
<tr>
    <td>02</td>
    <td>Shubham</td>
    <td>A036</td>
</tr><tr>
  <td>03</td>
  <td>Omkar</td>
  <td>A009</td>
</tr>
</table>
<p>This paragraph is the first child of its parent (body).</p>
<p>This paragraph is not the first child of its parent (body).</p>

<div>
  <p>This paragraph is the 1first child of its parent (div).</p>
  <p>This paragraph is not the first child of its parent (div).</p>
</div>

<div>
    <p>This paragraph is the 2first child of its parent (div).</p>
    <p>This paragraph is not the first child of its parent (div).</p>
  </div>

  <div>
    <p>This paragraph is the 3first child of its parent (div).</p>
    <p>This paragraph is not the first child of its parent (div).</p>
  </div>


</body>
</html>



//DOM Manipulation

<!DOCTYPE html>
<html>
<head>
<script src="jquery-3.2.1.min.js"></script>

<script>
    $(document).ready(function() {
      $("#id1").click(function(){
         
         alert($("#id0").text());
      });
      $("#id2").click(function(){
         alert($("P").text());
      });
      $("#id3").click(function(){
         alert($("#id0").html());
      });
      $("#b1").click(function(){
         alert($("#n1").val());
      });
      $("#b2").click(function(){
         alert($("#n2").val());
      });
   });
    </script>
</head>
<body>
<P id="id0"> FFUWFHNO<br></bt>AIUEWGAIU<br>EGIAEGNIUREHNGIU<br>EGNEANGAEN</P>
<h2>Remove an HTML Element</h2>
<button id="id1">Hello <br>Shubham</button>
<button  id="id2">Hello Gaurav</button>
<button id="id3">Hello omKAR</button>

<p>
    Name:<input type="text" id="n1" value="Gaurav">
</p>
<p>
    Name:<input type="text" id="n2" value="Shubham">
</p>
<button id="b1">Get First Student Name</button>
<button id="b2">Get Second Student Name</button>


</body>
</html>



