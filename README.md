<html lang="en">
  <head>
    <title>Nooks Work</title>
   </head
   <body>

<html><head><link rel="stylesheet" href="../style.css">

</head><body><h2 style="color:black">Retro Bowl</h2>
<br>
<button>Play now!</button>
<script>
    var urlObj = new window.URL(window.location.href);
    var url = "https://nookman9.github.io/retro";

    if (url) {
        var win;

        document.querySelector('button').onclick = function() {
            if (win) {
                win.focus();
            } 
            else {
                win = window.open();
                win.document.body.style.margin = '0';
                win.document.body.style.height = '100vh';
                var iframe = win.document.createElement('iframe');
                iframe.style.border = 'none';
                iframe.style.width = '100%';
                iframe.style.height = '100%';
                iframe.style.margin = '0';
                iframe.src = url;
                win.document.body.appendChild(iframe);
            }
            document.querySelector('button').style.background='#ff5148';
            document.querySelector('button').innerHTML="Page Opened!";
        };
    }
</script>
<style>
* {
    color: white; 
    font-family: arial;
    text-align: center;
}
button {
    width: 220px; 
    height: 40px;
    border-radius: 12px;
    background-color: #fc0000;
    font-family: Arial, Helvetica, sans-serif;
    border: none;
    transition: background-color 500ms;
}
button:hover {
    background-color: #fc0000;
}
</style>
</body></html>
