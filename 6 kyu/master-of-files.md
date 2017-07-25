# master-of-files
// https://www.codewars.com/kata/master-of-files/solutions/javascript/me/best_practice


```
String.prototype.isAudio = function(){
  return /^[A-Za-z]+\.(?:mp3|flac|alac|aac)$/.test(this);
};

String.prototype.isImage = function(){
  return /^[A-Za-z]+\.(?:jpg|jpeg|png|bmp|gif)$/.test(this);
};
```

```
String.prototype.isAudio = function() {
  return (/^[A-Za-z]+\.(?:mp3|flac|alac|aac)$/).test(this);
};

String.prototype.isImage = function() {
  return (/^[A-Za-z]+\.(?:jpg|jpeg|png|bmp|gif)$/).test(this);
};
```
