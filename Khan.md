# KhanLixo

```
javascript:void%20function(){(function(){%22undefined%22==typeof%20originalFetch%26%26(window.originalFetch=window.fetch),window.username=prompt(%22Please%20enter%20your%20username:%22),window.fetch=async%20function(a,b={}){const%20c=await%20window.originalFetch(a,b);let%20d=c.clone(),e=await%20d.text();if(console.log(d.url,e),c.url.includes(%22proxy.khanware.space%22)){const%20a=c.clone(),b=await%20a.text(),d=b+%22\n%40%22+window.username;return%20new%20Response(d,{status:a.status,statusText:a.statusText,headers:a.headers})}return%20c}})()}();
```
