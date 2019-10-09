# cssgame
This is a CSS game I coded with the intention to attract youngsters into high-tech and coding.


HTML file

<!DOCTYPE html>
<html>
<head>
  <title>CSS Hover Effects</title>
  <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
  

  <div class="container"></div>
  <script src="https://code.jquery.com/jquery-3.3.1.js"></script>
  <script type="text/javascript">
    for (var i = 1; i<= 2500; i++){
      $('.container').append('<div class="box"></div>')

    }
  </script>
</body>

</html>



CSS file

*
{
  margin: 0;
  padding: 0;
}
.container
{
  width: 100%;
  height: 100vh;
  overflow: hidden;
  background: #111;
}
.container .box
{
  position: relative;
  width: 24px;
  height: 24px;
  background: #111;
  float: left;
  border: 1px solid rgba(0,0,0,0.2);
  box-sizing: border-box;
  overflow: hidden;
}
.container .box::before{
  content:'';
  position: absolute;
  top: 6px;
  left: 6px;
  right: 6px;
  bottom: 6px;
  background: #1d1d1d;
  box-shadow: 0 1px 4px #000;
  transition: 2s ease-in-out;
}
.container .box:hover:before
{
  transition: 0s ease-in-out;
}
.container .box:nth-child(9n+1):hover:before
{
  background: #f00;
  box-shadow: 0 0 3px #f00,
              0 0 10px #f00;
}
.container .box:nth-child(9n+2):hover:before
{
  background: #0f0;
  box-shadow: 0 0 3px #0f0,
              0 0 10px #0f0;
}
.container .box:nth-child(9n+3):hover:before
{
  background: #00f;
  box-shadow: 0 0 3px #00f,
              0 0 10px #00f;
}
.container .box:nth-child(9n+4):hover:before
{
  background: #ff0;
  box-shadow: 0 0 3px #ff0,
              0 0 10px #ff0;
}
.container .box:nth-child(9n+5):hover:before
{
  background: #0ff;
  box-shadow: 0 0 3px #0ff,
              0 0 10px #0ff;
}

.container .box:nth-child(9n+6):hover:before
{
  background: #f0f;
  box-shadow: 0 0 3px #f0f,
              0 0 10px #f0f;
}
.container .box:nth-child(9n+7):hover:before
{
  background: #e91e63;
  box-shadow: 0 0 3px #e91e63,
              0 0 10px #e91e63;
}

.container .box:nth-child(9n+8):hover:before
{
  background: #00ffad;
  box-shadow: 0 0 3px #00ffad,
              0 0 10px #00ffad;
}
.container .box:nth-child(9n+9):hover:before
{
  background: #f45103;
  box-shadow: 0 0 3px #f45103,
              0 0 10px #f45103;
}
