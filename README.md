# Ex08 Event Registration Web Application
## Date:20.03.2026

## AIM:
To design, develop and deploy a web application for event registration using Figma UI tool.

## UI DESIGN TOOL:
Figma

## DESIGN STEPS:

### Step 1:
Use frames to represent screens or sections.

### Step 2:
Add column grids for consistent spacing and alignment.

### Step 3:
Insert shapes, text, buttons, and icons.

### Step 4:
Use Auto Layout for flexible, responsive design.

### Step 5:
Define color, text, and effect styles globally for consistency.

### Step 6:
Name layers logically and group related elements.

### Step 6:
Link frames to show navigation or interactions.

### Step 7:
Select the specific frame while generating code using Anima plugin.

## CODE:
```

index.html
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="android-compact">
      <div class="rectangle"></div>
      <p class="text-wrapper">SPORTS DAY EVENTS AND REGISTER</p>
      <div class="div"></div>
      <img class="text-on-a-path" src="img/image.svg" />
      <img class="img" src="img/text-on-a-path.svg" />
      <p class="p">CLICK HERE TO VIEW EVENTS</p>
      <div class="rectangle-2"></div>
      <p class="text-wrapper-2">CLICK HERE TO REGISTER FOR EVENTS</p>
      <div class="rectangle-3"></div>
      <div class="text-wrapper-3">VAHINI-25018547</div>
    </div>
  </body>
</html>

global.css
@import url("https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css");
* {
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
html,
body {
  margin: 0px;
  height: 100%;
}
/* a blue color as a generic focus style */
button:focus-visible {
  outline: 2px solid #4a90e2 !important;
  outline: -webkit-focus-ring-color auto 5px !important;
}
a {
  text-decoration: none;
}
/* @FONTWARNING[{"type": "restricted", "family": "Inter-Bold", "weight": "700", "style": "normal", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Inter-Bold";
  src: local("Inter-Bold");
}
/* @FONTWARNING[{"type": "restricted", "family": "Inter-BoldItalic", "weight": "700", "style": "italic", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Inter-BoldItalic";
  src: local("Inter-BoldItalic");
}
style.css
.android-compact {
  overflow: hidden;
  background-image: url(./img/android-compact-1.png);
  background-size: cover;
  background-position: 50% 50%;
  width: 100%;
  min-width: 410px;
  min-height: 922px;
  position: relative;
}

.android-compact .rectangle {
  position: absolute;
  top: 67px;
  left: 36px;
  width: 347px;
  height: 112px;
  background-color: #2abdbd;
}

.android-compact .text-wrapper {
  position: absolute;
  top: 89px;
  left: 68px;
  width: 303px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #e41f1f;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .div {
  position: absolute;
  top: 343px;
  left: 66px;
  width: 305px;
  height: 91px;
  background-color: #fa167d;
}

.android-compact .text-on-a-path {
  position: absolute;
  top: 534px;
  left: 233px;
  width: 317px;
  height: 95px;
}

.android-compact .img {
  position: absolute;
  top: 849px;
  left: 167px;
  width: 410px;
  height: 89px;
}

.android-compact .p {
  position: absolute;
  top: 365px;
  left: 96px;
  width: 262px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .rectangle-2 {
  position: absolute;
  top: 512px;
  left: 55px;
  width: 328px;
  height: 90px;
  background-color: #f10f7c;
}

.android-compact .text-wrapper-2 {
  position: absolute;
  top: 531px;
  left: 77px;
  width: 294px;
  font-family: "Inter-BoldItalic", Helvetica;
  font-weight: 700;
  font-style: italic;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .rectangle-3 {
  position: absolute;
  top: 853px;
  left: 0;
  width: 410px;
  height: 69px;
  background-color: #000000;
}

.android-compact .text-wrapper-3 {
  position: absolute;
  top: 877px;
  left: 27px;
  width: 356px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #f3e8e8;
  font-size: 36px;
  letter-spacing: 0;
  line-height: normal;
}

```
```
index.html
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="android-compact">
      <img class="sports" src="img/sports-2-1.png" />
      <div class="rectangle"></div>
      <div class="text-wrapper">VAHINI-25018547</div>
      <div class="div"></div>
      <div class="text-wrapper-2">REGISTRATION FORM</div>
      <div class="rectangle-2"></div>
      <div class="rectangle-3"></div>
      <div class="rectangle-4"></div>
      <div class="rectangle-5"></div>
      <div class="rectangle-6"></div>
      <div class="rectangle-7"></div>
      <div class="text-wrapper-3">REG NO:</div>
      <div class="text-wrapper-4">NAME:</div>
      <div class="text-wrapper-5">MOBILE NO:</div>
      <div class="text-wrapper-6">EMAIL ID:</div>
      <div class="text-wrapper-7">EVENTS:</div>
      <div class="text-wrapper-8">NO.OF.MEMBERS:</div>
    </div>
  </body>
</html>

global.css
@import url("https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css");
* {
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
html,
body {
  margin: 0px;
  height: 100%;
}
/* a blue color as a generic focus style */
button:focus-visible {
  outline: 2px solid #4a90e2 !important;
  outline: -webkit-focus-ring-color auto 5px !important;
}
a {
  text-decoration: none;
}
/* @FONTWARNING[{"type": "restricted", "family": "Inter-Bold", "weight": "700", "style": "normal", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Inter-Bold";
  src: local("Inter-Bold");
}
/* @FONTWARNING[{"type": "restricted", "family": "Inter-BoldItalic", "weight": "700", "style": "italic", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Inter-BoldItalic";
  src: local("Inter-BoldItalic");
}
style.css
.android-compact {
  background-color: #ffffff;
  overflow: hidden;
  width: 100%;
  min-width: 396px;
  min-height: 922px;
  position: relative;
}

.android-compact .sports {
  position: absolute;
  top: 0;
  left: 0;
  width: 396px;
  height: 922px;
  aspect-ratio: 1.5;
  object-fit: cover;
}

.android-compact .rectangle {
  position: absolute;
  top: 859px;
  left: 1px;
  width: 396px;
  height: 63px;
  background-color: #000000;
}

.android-compact .text-wrapper {
  position: absolute;
  top: 885px;
  left: 34px;
  width: 348px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #ffffff;
  font-size: 36px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .div {
  position: absolute;
  top: 0;
  left: 1px;
  width: 396px;
  height: 91px;
  background-color: #9dc6d6;
}

.android-compact .text-wrapper-2 {
  position: absolute;
  top: 26px;
  left: 21px;
  width: 361px;
  font-family: "Inter-BoldItalic", Helvetica;
  font-weight: 700;
  font-style: italic;
  color: #0804f5;
  font-size: 32px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .rectangle-2 {
  position: absolute;
  top: 154px;
  left: 28px;
  width: 335px;
  height: 73px;
  background-color: #e29de2;
}

.android-compact .rectangle-3 {
  position: absolute;
  top: 277px;
  left: 34px;
  width: 329px;
  height: 64px;
  background-color: #c68dd6;
}

.android-compact .rectangle-4 {
  position: absolute;
  top: 393px;
  left: 34px;
  width: 329px;
  height: 74px;
  background-color: #f48df4;
}

.android-compact .rectangle-5 {
  position: absolute;
  top: 518px;
  left: 28px;
  width: 335px;
  height: 63px;
  background-color: #b982bd;
}

.android-compact .rectangle-6 {
  position: absolute;
  top: 628px;
  left: 34px;
  width: 329px;
  height: 65px;
  background-color: #dd94da;
}

.android-compact .rectangle-7 {
  position: absolute;
  top: 741px;
  left: 34px;
  width: 329px;
  height: 63px;
  background-color: #cf97df;
}

.android-compact .text-wrapper-3 {
  position: absolute;
  top: 296px;
  left: 54px;
  width: 309px;
  font-family: "Inter-BoldItalic", Helvetica;
  font-weight: 700;
  font-style: italic;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-4 {
  position: absolute;
  top: 173px;
  left: 50px;
  width: 280px;
  font-family: "Inter-BoldItalic", Helvetica;
  font-weight: 700;
  font-style: italic;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-5 {
  position: absolute;
  top: 417px;
  left: 58px;
  width: 272px;
  font-family: "Inter-BoldItalic", Helvetica;
  font-weight: 700;
  font-style: italic;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-6 {
  position: absolute;
  top: 532px;
  left: 50px;
  width: 263px;
  font-family: "Inter-BoldItalic", Helvetica;
  font-weight: 700;
  font-style: italic;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-7 {
  position: absolute;
  top: 648px;
  left: 34px;
  width: 255px;
  font-family: "Inter-BoldItalic", Helvetica;
  font-weight: 700;
  font-style: italic;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-8 {
  position: absolute;
  top: 762px;
  left: 34px;
  width: 272px;
  font-family: "Inter-BoldItalic", Helvetica;
  font-weight: 700;
  font-style: italic;
  color: #000000;
  font-size: 24px;
  letter-spacing: 0;
  line-height: normal;
}


```
```
index.html
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="android-compact">
      <img class="prize" src="img/prize-1.png" />
      <div class="rectangle"></div>
      <div class="text-wrapper">CASH PRIZE DETAILS</div>
      <div class="div"></div>
      <div class="text-wrapper-2">VAHINI-25018547</div>
      <p class="p">For any sports their is a cash prize for winners</p>
      <div class="rectangle-2"></div>
      <div class="rectangle-3"></div>
      <img class="img" src="img/rectangle-18.svg" />
      <div class="text-wrapper-3">3rd-3000/-</div>
      <div class="text-wrapper-4">2nd-4000/-</div>
      <div class="text-wrapper-5">1st-5000/-</div>
    </div>
  </body>
</html>

global.css
@import url("https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css");
* {
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
html,
body {
  margin: 0px;
  height: 100%;
}
/* a blue color as a generic focus style */
button:focus-visible {
  outline: 2px solid #4a90e2 !important;
  outline: -webkit-focus-ring-color auto 5px !important;
}
a {
  text-decoration: none;
}
/* @FONTWARNING[{"type": "restricted", "family": "Inter-BoldItalic", "weight": "700", "style": "italic", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Inter-BoldItalic";
  src: local("Inter-BoldItalic");
}
/* @FONTWARNING[{"type": "restricted", "family": "Inter-Bold", "weight": "700", "style": "normal", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Inter-Bold";
  src: local("Inter-Bold");
}

style.css


.android-compact {
  background-color: #ffffff;
  width: 100%;
  min-width: 412px;
  min-height: 917px;
  position: relative;
}

.android-compact .prize {
  position: absolute;
  top: 0;
  left: 0;
  width: 412px;
  height: 917px;
  aspect-ratio: 1.5;
  object-fit: cover;
}

.android-compact .rectangle {
  position: absolute;
  top: 0;
  left: 0;
  width: 412px;
  height: 90px;
  background-color: #474642;
}

.android-compact .text-wrapper {
  position: absolute;
  top: 22px;
  left: 44px;
  width: 368px;
  font-family: "Inter-BoldItalic", Helvetica;
  font-weight: 700;
  font-style: italic;
  color: #ffffff;
  font-size: 32px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .div {
  position: absolute;
  top: 844px;
  left: 0;
  width: 412px;
  height: 73px;
  background-color: #000000;
}

.android-compact .text-wrapper-2 {
  position: absolute;
  top: 867px;
  left: 56px;
  width: 356px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #ffffff;
  font-size: 32px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .p {
  position: absolute;
  top: 104px;
  left: 27px;
  width: 330px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #e2fa04;
  font-size: 32px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .rectangle-2 {
  position: absolute;
  top: 284px;
  left: 43px;
  width: 300px;
  height: 81px;
  background-color: #b5b281;
}

.android-compact .rectangle-3 {
  position: absolute;
  top: 398px;
  left: 43px;
  width: 300px;
  height: 74px;
  background-color: #d0d19b;
}

.android-compact .img {
  position: absolute;
  top: 504px;
  left: 43px;
  width: 300px;
  height: 66px;
}

.android-compact .text-wrapper-3 {
  position: absolute;
  top: 515px;
  left: 99px;
  width: 244px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #000000;
  font-size: 32px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-4 {
  position: absolute;
  top: 420px;
  left: 96px;
  width: 250px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #000000;
  font-size: 32px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .text-wrapper-5 {
  position: absolute;
  top: 304px;
  left: 95px;
  width: 252px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #000000;
  font-size: 32px;
  letter-spacing: 0;
  line-height: normal;
}


```
```
index.html
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta charset="utf-8" />
    <link rel="stylesheet" href="globals.css" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="android-compact">
      <div class="rectangle"></div>
      <div class="text-wrapper">VAHINI-25018547</div>
      <div class="div">!...THANKYOU...!</div>
      <p class="p">COME AND PARTICIPATE AND WIN THE PRIZE...!</p>
    </div>
  </body>
</html>

global.css
@import url("https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css");
* {
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
html,
body {
  margin: 0px;
  height: 100%;
}
/* a blue color as a generic focus style */
button:focus-visible {
  outline: 2px solid #4a90e2 !important;
  outline: -webkit-focus-ring-color auto 5px !important;
}
a {
  text-decoration: none;
}
/* @FONTWARNING[{"type": "restricted", "family": "Inter-Bold", "weight": "700", "style": "normal", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Inter-Bold";
  src: local("Inter-Bold");
}
/* @FONTWARNING[{"type": "restricted", "family": "Inter-ExtraBold Italic", "weight": "800", "style": "italic", "allowsCrossOrigin": false}] */

@font-face {
  font-family: "Inter-ExtraBold Italic";
  src: local("Inter-ExtraBold Italic");
}

style.css

.android-compact {
  background-color: #e3acd5;
  width: 100%;
  min-width: 412px;
  min-height: 917px;
  position: relative;
}

.android-compact .rectangle {
  position: absolute;
  top: 824px;
  left: 0;
  width: 412px;
  height: 93px;
  background-color: #000000;
}

.android-compact .text-wrapper {
  position: absolute;
  top: 850px;
  left: 29px;
  width: 353px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #ffffff;
  font-size: 32px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .div {
  position: absolute;
  top: 77px;
  left: 34px;
  width: 348px;
  font-family: "Inter-Bold", Helvetica;
  font-weight: 700;
  color: #510941;
  font-size: 40px;
  letter-spacing: 0;
  line-height: normal;
}

.android-compact .p {
  position: absolute;
  top: 333px;
  left: 56px;
  width: 340px;
  font-family: "Inter-ExtraBold Italic", Helvetica;
  font-weight: 800;
  font-style: italic;
  color: #1924bb;
  font-size: 32px;
  letter-spacing: 0;
  line-height: normal;
}

```


## OUTPUT:


<img width="1920" height="1080" alt="Screenshot (87)" src="https://github.com/user-attachments/assets/21edd589-7919-4c1c-9d51-19ca6f66df06" />

## RESULT:
The program to design, develop and deploy a web application for event registration using Figma UI tool is completed successfully.
