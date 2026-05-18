<!DOCTYPE html>
<html>
<head>
<title>MotionFlow AI</title>
<style>
body{
margin:0;
font-family:Arial;
background:#000;
color:white;
text-align:center;
}

.hero{
padding:100px 20px;
}

button{
padding:15px 30px;
background:#00ccff;
border:none;
border-radius:10px;
cursor:pointer;
font-size:16px;
}

input{
padding:12px;
width:300px;
margin:20px;
border-radius:8px;
border:none;
}

#preview{
margin-top:30px;
max-width:400px;
display:none;
border-radius:15px;
}
</style>
</head>
<body>

<div class="hero">
<h1>MotionFlow AI</h1>
<p>Upload fashion image and preview render</p>

<input type="file" id="upload" accept="image/*"><br>

<button onclick="previewImage()">Preview</button>

<br>
<img id="preview">

</div>

<script>
function previewImage(){
const file=document.getElementById("upload").files[0];
const preview=document.getElementById("preview");

if(file){
preview.src=URL.createObjectURL(file);
preview.style.display="block";
}
}
</script>

</body>
</html># motionflow-ai
AI fashion motion render platform
