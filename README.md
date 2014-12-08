[KoffieScript](http://koffiescript.nl)
==========
![Dutch Flag](/assets/img/flag.png)

KoffieScript lets you write JavaScript in Dutch; Finally there is a way for Dutch people to code in their native language!

See it in action [here](http://koffiescript.nl).
### Including KoffieScript files in your HTML

- Include [koffiescript.js](dist/koffiescript.js) and [koffiescript.browser.js](dist/koffiescript.browser.js).
- Make sure your html is set to allow utf-8 characters (add `<meta charset="utf-8">` in the <head>).

KoffieScript supports the `text/koffiescript` MIME type. Any script tag with that type will be compiled and run automatically:
```htmls
<script type="text/koffiescript">
  als (x < 5) {
    console.log("hallo!");
  } anders {
    console.log("dacht het niet!");
  }
</script>
```

You can also specify a `src` for your script tags:
```html
<script type="text/koffiescript" src="snaps.koffie"></script>
```

#### Optional

##### Convert from KoffieScript to JavaScript:

```javascript
KoffieScript.DutchToEnglish(code); // returns a string representing the translated code
```

##### Convert from JavaScript to KoffieScript:

```javascript
KoffieScript.EnglishToDutch(code); // returns a string representing the translated code
```

### Missing/incorrect translations?
You can see the translations over [here](https://github.com/bouk/koffiescript/blob/gh-pages/dist/koffiescript.js#L4). Feel free to submit a pull request!

###TO-DOs
- Syntax highlighting for unicode chars
- npm support for command line compiling
- Add more translations!!! (ex: Array.pop, push, etc...)
