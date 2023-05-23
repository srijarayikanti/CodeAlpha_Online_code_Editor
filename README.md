# CodeAlpha_Online_code_Editor
an online code editor usin html,css and js
#html code
<!DOCTYPE html>
<html>
    <head>
        <meta name="viewport" content="width=device-width,initial-scale=1.0">
        <title>online code editor</title>
        <link rel="stylesheet" href="code.css">
    </head>
    <body>
        <div class="container">
            <div class="left">
               <label>HTML</label>
               <textarea id="html-code" onkeyup="run()"></textarea>
               <label>CSS</label>
               <textarea id="css-code" onkeyup="run()"></textarea>
               <label>Javascript</label>
               <textarea id="js-code" onkeyup="run()"></textarea>
            </div>
            <div class="right">
                <label>output</label>
                <iframe id="output"></iframe>
            </div>
        </div>
        <script>
            function run(){
                let htmlCode=document.getElementById("html-code").value;
                let cssCode=document.getElementById("css-code").value;
                let JsCode=document.getElementById("js-code").value;
                let output=document.getElementById("output");

                output.contentDocument.body.innerHTML= htmlCode+"<style>"+cssCode+"</style>"+JsCode;
                output.contentWindow.eval(JsCode);
            }
        </script>
    </body>
</html>
