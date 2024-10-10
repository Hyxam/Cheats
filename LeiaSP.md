# LeiaSP


```javascript
javascript:(function(){var event=new KeyboardEvent('keydown',{key:'ArrowRight',code:'ArrowRight',keyCode:39,which:39,bubbles:true});var count=0;var maxTimes=300;var intervalId;function startInterval(){intervalId=setInterval(function(){document.dispatchEvent(event);count++;if(count>=maxTimes){clearInterval(intervalId);alert("Terminou de passar as p%C3%A1ginas!");}},200);}startInterval();var observer=new MutationObserver(function(mutations){for(var mutation of mutations){if(document.readyState==='complete'){clearInterval(intervalId);count=0;console.log("P%C3%A1gina atualizada, reiniciando contagem.");startInterval();break;}}});observer.observe(document.body,{childList:true,subtree:true});})();
```
