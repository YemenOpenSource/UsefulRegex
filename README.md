[![Stand With Palestine](https://raw.githubusercontent.com/TheBSD/StandWithPalestine/main/banner-no-action.svg)](https://TheBSD.github.io/StandWithPalestine/)

# UsefulRegex
A collection of usefull regex please add any thing seems to be usful.


Multiline Comments


`/\*[^*]*\*+(?:[^/*][^*]*\*+)*/`


Explanation here.

https://stackoverflow.com/a/36328890/14569050


_____

`^//.*`

on line comment


_________
`^[ \n]{2,}`

2 or more empty lines



# Most used for CSS files



Lines that does not end with ; or { or ,


`^.*:.*(?<!;|\{|,)$`

Lines that does not end with ; or { or ,

useful to add ; to CSS properties witch does not have



----------------------------
`(rgb)(\(.*\, .*\, .*\, .*\))`

Selects rgba colors witch written as rgb



-------------------------------
`rgb\((.* )(.* )(.* )\/ (.*)\%\)`

Chrome color Standards to old css one to avoid css syntax errors or linters errors
replace with
rgba\($1, $2, $3, \.$4\)


---------------------------------------------------------------
Check yemeni phone numbers
---------------------------------------------------------------

### for both cell phones/mobiles phones and land lines
`/^(((\+|00)9677|0?7)[01378]\d{7}|((\+|00)967|0)[1-7]\d{6})$/`

### for only cell phones/mobiles phones
`^(((\+|00)9677|0?7)[01378]\d{7})$`

### for only land lines
`^(((\+|00)967|0)[1-7]\d{6})$`

Check yemeni phone numbers As you go (if you type true it's true if you miss with something it's false)

https://gist.github.com/Waseem-Almoliky/8aab02bdb8155a06cf5c2ef60fcdebea



---------------------------------------------------------------

# Others


Variablefy


`[^\w\/]+`


php:


`~[^\w\/]+~`


php usage example:

`strtolower(preg_replace('~[^\w\/]+~', '_', $field['title']))`



---------------------------------------------------------------



`/^(\d+(\.\d*)?)|(\.\d+)$/`

numbers (floats included)




---------------------------------------------------------------



`__\(('.+?(?='\))')\)|__\((".+?(?="\))")\)`

Laravel translation function pick text




---------------------------------------------------------------


`([ء-يًٌ]+\s*)+`



regex  
مفيد في  البحث عن أي كلمة عربية




---------------------------------------------------------------


`عبد (الله|الرحمن|الرحيم|الملك|القدوس|السلام|المؤمن|المهيمن|العزيز|الجبار|المتكبر|الخالق|البارىء|المصور|الغفار|القهار|الوهاب|الرزاق|الفتاح|العليم|القابض|الباسط|الخافض|الرافع|المعز|المذل|السميع|البصير|الحكم|العدل|اللطيف|الخبير|الحليم|العظيم|الغفور|الشكور|العلي|الكبير|الحفيظ|المقيت|الحسيب|الجليل|الكريم|الرقيب|المجيب|الواسع|الحكيم|الودود|المجيد|الباعث|الشهيد|الحق|الوكيل|القوي|المتين|الولي|الحميد|المحصي|المبدىء|المعيد|المحيي|المميت|الحي|القيوم|الواجد|الماجد|الواحد|الصمد|القادر|المقتدر|المقدم|المؤخر|الأول|الآخر|الظاهر|الباطن|الوالي|المتعال|البر|التواب|المنتقم|العفو|الرءوف|مالك الملك|ذوالجلال والإكرام|المقسط|الجامع|الغني|المغني|المانع|الضار|النافع|النور|الهادي|البديع|الباقي|الوارث|الرشيد|الصبور)`                             

اسماء الله الحسنى مع مسافة بعد عبد


