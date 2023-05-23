# CodeAlpha_Online_code_Editor
an online code editor usin html,css and js
#css code
*{
    margin:0;
    padding:0;
    font-family: 'poppins',serif;
    box-sizing: border-box;
}
body{
    background: #444;
    color:aquamarine;  
}
.container{
    width: 100%;
    height:100%;
    padding:20px;
    display:flex;
}
.left,.right{
     flex-basis: 50%;
     padding: 10px;
}
textarea{
    width: 100%;
    height:28%;
    background: black;
    color:white;
    padding: 10px 20px;
    border:0;
    outline:0;
    font-size: 18px;
}
iframe{
    width: 100%;
    height: 95%;
    background:white;
    border:0;
    outline:0;
}
label{
    display: flex;
    align-items: center;
    background: #000;
    height:30px;
}
