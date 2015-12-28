# JSileBenzersizKayitListesi

Bir dizi içerisinden istenilen sayıda elemanı benzersiz şekilde alır.

Kullanımı
=================================

```
var _inputArray = ["Zeynep", "Rümeysa", "Ayşe", "Ahmet", "Cemil", "Şakir"];

function inArray(_value, _array){ return _array.indexOf(_value); }

function generateRandom(_arrayLen){
	return Math.floor(Math.random() * _arrayLen);
}

var output = [];
function getLst(_array, _val){
    var i = 0;
    do{
    	var _rndmIndex = generateRandom(_array.length);
      if (inArray(_array[_rndmIndex], output) === -1){
        output.push(_array[_rndmIndex]);
        i += 1;
      }
    }while(i !== _val);
    return output;
}

console.log(getLst(_inputArray, 5));
```

Çalışan Örnek
=================================

https://jsfiddle.net/DeliPenguen/q6q05onv/
