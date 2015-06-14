# BeehivePicker  
BeehivePicker is color picker like beehive(hexagon color picker).  
BeehivePickerは六角形(蜂の巣型)のカラーピッカーです。  

# How To Use
Beehive.Picker(element{, id})  
Params::  
element: Document|Node  
id: when you use multiple BeehivePicker, you have to set unique key for BeehivePicker.   
    You don't have to use this id when you use just one BeehivePicker.    
    複数のBeehivePickerを配置する場合は一意のキーをセット。ひとつの場合は不要 
Return::  
  nothing

Beehive.getColorCode(element)  
Params::  
element: Document|Node  
Return::  
String: color code like #ffffff  
        when the element doesn't have beehive-picker class, this method will return null.  

# sample code  

    var div = document.getElementById('main');
    Beehive.Picker(div);
    div.addEventListener('click', function(e){
      var color = Beehive.getColorCode(e.target);
      if(!color){ console.log('it is not beehive picker color elemnt.'); }
      console.log(color);
    });

# demo

[DEMO](https://tebakane.github.io/BeehivePicker/sample.html)

# image

![sample image](https://github.com/tebakane/images_for_git/blob/master/images/beehive_picker_screen_shot.png)




