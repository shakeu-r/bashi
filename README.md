<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Valentine 💖</title>

<style>
body{
  margin:0;
  height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  background:linear-gradient(135deg,#ffb6c1,#ffc0cb);
  font-family:Arial,sans-serif;
}
.card{
  background:white;
  padding:30px;
  border-radius:20px;
  text-align:center;
  width:90%;
  max-width:350px;
  box-shadow:0 10px 25px rgba(0,0,0,.2);
}
h1{
  color:#e91e63;
  margin-bottom:25px;
}
.buttons{
  display:flex;
  gap:10px;
}
button{
  flex:1;
  padding:15px;
  font-size:18px;
  border:none;
  border-radius:12px;
}
#yes{
  background:#4caf50;
  color:white;
}
#no{
  background:#f44336;
  color:white;
}
img{
  width:100%;
  border-radius:15px;
}
</style>
</head>

<body>

<div class="card">
  <h1 id="text">Will you be my Valentine? 🌹</h1>

  <div class="buttons" id="btns">
    <button id="yes">Yes 💚</button>
    <button id="no">No ❤️</button>
  </div>
</div>

<script>
const noBtn = document.getElementById("no");
const yesBtn = document.getElementById("yes");
const text = document.getElementById("text");
const card = document.querySelector(".card");

noBtn.onclick = () => {
  text.innerText = "Stop messing with me! 😾";
  card.innerHTML = `
    <h1 style="color:#e91e63">Stop messing with me! 😾</h1>
    <img src="https://media.tenor.com/0AVbKGY_MxMAAAAC/cat-angry.gif">
  `;
};

yesBtn.onclick = () => {
  text.innerText = "Yaaay 😍💖";
  document.getElementById("btns").style.display="none";
};
</script>

</body>
</html>
