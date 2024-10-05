# KhanLixo

```js
javascript:let originalParse=JSON.parse;console.log("if you look in the console you WILL see a error, they save it as a question though so I'm not worried about it right now."),JSON.parse=function(t,e){let o=originalParse(t,e);try{const t=JSON.parse(o.data.assessmentItem.item.itemData);t.question&&t.question.content&&t.question.content[1]===t.question.content[1].toUpperCase()&&(console.log(t),t.question.content="Please select a answer choice.\n [[☃ radio 1]] [[☃ explanation 1]]",t.question.widgets={"radio 1":{options:{choices:[{content:"Correct",correct:!0},{content:"Incorrect",correct:!1}]}},"explanation 1":{options:{explanation:"This hack was made by @ilyTobias on Discord & GitHub.",hidePrompt:"",showPrompt:"Credit"}}},o.data.assessmentItem.item.itemData=JSON.stringify(t))}catch(t){}return o},location.softReload=()=>{const t=document.getElementsByTagName("html")[0].outerHTML;document.open(),document.write(t),document.close()},location.softReload();
```
