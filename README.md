# pocpat_automatedscript
Use this code to auto click popcat

Steps:
1. Go to your browser.
2. Right click and choose inspect element. (Or Ctrl+Shift+I)
3. Go to console.
4. Type the following code and press enter.
var event = new KeyboardEvent('keydown',{key:'t',ctrlKey:true});
setInterval(function(){
  for(i=0;i<100;i++){
    document.dispatchEvent(event);
  }
},50);
