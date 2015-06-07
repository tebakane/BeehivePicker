# BeehivePicker  
BeehivePicker is color picker like beehive(hexagon color picker).  
BeehivePickerは六角形(蜂の巣型)のカラーピッカーです。  

# How To Use
Beehive.Picker(element{, id})  
element: Document|Node  
id: when you use multiple BeehivePicker, you have to set unique key for BeehivePicker.   
    You don't have to use this id when you use just one BeehivePicker.    

Beehive.Picker(element{, id})  
element: Document|Node  
id: 複数のBeehivePickerを配置する場合は一意のキーをセット。ひとつの場合は不要  

# sample code  

    var div = document.getElementById('main');
    Beehive.Picker(div);
    div.addEventListener('click', function(e){
      var style = window.getComputedStyle(e.target, null);
      console.log(style.backgroundColor);
    });



