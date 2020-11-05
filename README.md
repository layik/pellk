# دامەزراندن و بەکارهێنان

1. دامەزراندنی مۆدیوڵەکە:

   `npm install https://github.com/layik/pellk.git --save`
   
   یان
   
   `yarn add https://github.com/layik/pellk.git `
   
2. بەکارهێنان:

   لەوشوێنەی دەتەوێت پەڵک بەکاربهێنیت:

```javascript
   import { convert } from "pellk";
```
3. تایبەتمەندییەکان
3.1 عەرەبی بۆ لاتین

```javascript
   const options = {
		chkDilan: false,
		chkAliWeb: false,
		chkOnsetI: false,
		chkCapitaliseSentence: false,
		chkConvertNumbers: true,
		chkTreatI: false,
		dchkConnectSuffixes: true,
   }
	
   const toLatin = convert("کوردستان", 1, options) // --> kurdistan
```
   3.2 لاتین بۆ عەرەبی
```javascript
   const options = {
		chkDilan: false,
		chkAliWeb: false,
		chkOnsetI: false,
		chkCapitaliseSentence: false,
		chkConvertNumbers: true,
		chkTreatI: false,
		dchkConnectSuffixes: true,
    }
	
   const toLatin = convert("kurdistan", 2, options) // --> کوردستان
```
   
   3.3 بەستاندەردکردنی نووسەی عەرەبی
```javascript
   const options = {
		chkDilan: false,
		chkAliWeb: false,
		chkOnsetI: false,
		chkCapitaliseSentence: false,
		chkConvertNumbers: true,
		chkTreatI: false,
		dchkConnectSuffixes: true,
   }
	
   const toLatin = convert("دهۆك", 2, options) // --> دهۆک
```
4. هەڵبژاردەکان
ئارگیومێنی کۆتایی نەخشەکە کۆمەڵێک بژاردە وەردەگرێت کە ئەمانەن:


| هەڵبژاردە | وەسف | جۆر | نرخی بنەڕەت |
| ------------ | ------------ | ------------ | ------------ |
| chkDilan  | چێکردن و خاوێنکردنی فۆنتەکانی دیلان   |  boolean  | false  |
| chkAliWeb  |  چێکردن و خاوێنکردنی فۆنتەکانی AliWeb  | boolean  | false  |
| chkOnsetI | زیادکردنی بزرۆکە بۆ تێکستی کورمانجی | boolean  | false  |
| chkCapitaliseSentence  | گەورەکردنی یەکەم پیت  | boolean  |  false |
| chkConvertNumbers  | گۆڕینی ژمارەکان   | boolean  | true   |
| chkTreatI  | گۆڕینی بزرۆکە بۆ "ی"   | boolean  |  false  |
| dchkConnectSuffixes  |  پێکەوە لکاندنی پاشگرەکان  | boolean   | false  |

