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
import image from "./image.svg";
import textOnAPath from "./text-on-a-path.svg";

export const AndroidCompact = (): JSX.Element => {
  return (
    <div className="overflow-hidden bg-[url(/android-compact-1.png)] bg-cover bg-[50%_50%] w-full min-w-[410px] min-h-[922px] relative">
      <div className="absolute top-[67px] left-9 w-[347px] h-28 bg-[#2abdbd]" />

      <p className="absolute top-[89px] left-[68px] w-[303px] [font-family:'Inter-Bold',Helvetica] font-bold text-[#e41f1f] text-2xl tracking-[0] leading-[normal]">
        SPORTS DAY EVENTS AND REGISTER
      </p>

      <button
        className="absolute top-[343px] left-[66px] w-[305px] h-[91px] bg-[#fa167d] cursor-pointer"
        type="button"
        aria-label="Click here to view events"
      >
        <p className="absolute top-[22px] left-[58px] w-[262px] [font-family:'Inter-Bold',Helvetica] font-bold text-black text-2xl tracking-[0] leading-[normal]">
          CLICK HERE TO VIEW EVENTS
        </p>
      </button>

      <img
        className="absolute top-[518px] left-[22px] w-[317px] h-[95px]"
        alt="Sports day graphic"
        src={image}
      />

      <img
        className="absolute top-[833px] -left-11 w-[410px] h-[89px]"
        alt="Text on a path"
        src={textOnAPath}
      />

      <button
        className="absolute top-[512px] left-[55px] w-[328px] h-[90px] bg-[#f10f7c] cursor-pointer"
        type="button"
        aria-label="Click here to register for events"
      >
        <p className="absolute top-[19px] left-[22px] w-[294px] [font-family:'Inter-BoldItalic',Helvetica] font-bold italic text-black text-2xl tracking-[0] leading-[normal]">
          CLICK HERE TO REGISTER FOR EVENTS
        </p>
      </button>

      <div className="absolute top-[853px] left-0 w-[410px] h-[69px] bg-black" />

      <div className="absolute top-[877px] left-[27px] w-[356px] [font-family:'Inter-Bold',Helvetica] font-bold text-[#f3e8e8] text-4xl tracking-[0] leading-[normal]">
        VAHINI-25018547
      </div>
    </div>
  );
};

```
```
import { useState } from "react";
import sports21 from "./sports-2-1.png";

export const AndroidCompact = (): JSX.Element => {
  const [formData, setFormData] = useState({
    name: "",
    regNo: "",
    mobileNo: "",
    emailId: "",
    events: "",
    noOfMembers: "",
  });

  const handleChange = (e: React.ChangeEvent<HTMLInputElement>) => {
    const { name, value } = e.target;
    setFormData((prev) => ({ ...prev, [name]: value }));
  };

  const formFields = [
    {
      id: "name",
      label: "NAME:",
      name: "name",
      type: "text",
      top: "top-[154px]",
      left: "left-7",
      width: "w-[335px]",
      height: "h-[73px]",
      bg: "bg-[#e29de2]",
      labelTop: "top-[173px]",
      labelLeft: "left-[50px]",
      labelWidth: "w-[280px]",
      inputTop: "top-[173px]",
      inputLeft: "left-[160px]",
      inputWidth: "w-[180px]",
    },
    {
      id: "regNo",
      label: "REG NO:",
      name: "regNo",
      type: "text",
      top: "top-[277px]",
      left: "left-[34px]",
      width: "w-[329px]",
      height: "h-16",
      bg: "bg-[#c68dd6]",
      labelTop: "top-[296px]",
      labelLeft: "left-[54px]",
      labelWidth: "w-[309px]",
      inputTop: "top-[296px]",
      inputLeft: "left-[180px]",
      inputWidth: "w-[160px]",
    },
    {
      id: "mobileNo",
      label: "MOBILE NO:",
      name: "mobileNo",
      type: "tel",
      top: "top-[393px]",
      left: "left-[34px]",
      width: "w-[329px]",
      height: "h-[74px]",
      bg: "bg-[#f48df4]",
      labelTop: "top-[417px]",
      labelLeft: "left-[58px]",
      labelWidth: "w-[272px]",
      inputTop: "top-[417px]",
      inputLeft: "left-[210px]",
      inputWidth: "w-[130px]",
    },
    {
      id: "emailId",
      label: "EMAIL ID:",
      name: "emailId",
      type: "email",
      top: "top-[518px]",
      left: "left-7",
      width: "w-[335px]",
      height: "h-[63px]",
      bg: "bg-[#b982bd]",
      labelTop: "top-[532px]",
      labelLeft: "left-[50px]",
      labelWidth: "w-[263px]",
      inputTop: "top-[532px]",
      inputLeft: "left-[190px]",
      inputWidth: "w-[155px]",
    },
    {
      id: "events",
      label: "EVENTS:",
      name: "events",
      type: "text",
      top: "top-[628px]",
      left: "left-[34px]",
      width: "w-[329px]",
      height: "h-[65px]",
      bg: "bg-[#dd94da]",
      labelTop: "top-[648px]",
      labelLeft: "left-[34px]",
      labelWidth: "w-[255px]",
      inputTop: "top-[648px]",
      inputLeft: "left-[170px]",
      inputWidth: "w-[170px]",
    },
    {
      id: "noOfMembers",
      label: "NO.OF.MEMBERS:",
      name: "noOfMembers",
      type: "number",
      top: "top-[741px]",
      left: "left-[34px]",
      width: "w-[329px]",
      height: "h-[63px]",
      bg: "bg-[#cf97df]",
      labelTop: "top-[762px]",
      labelLeft: "left-[34px]",
      labelWidth: "w-[272px]",
      inputTop: "top-[762px]",
      inputLeft: "left-[240px]",
      inputWidth: "w-[110px]",
    },
  ];

  return (
    <div className="bg-white overflow-hidden w-full min-w-[396px] min-h-[922px] relative">
      <img
        className="absolute top-0 left-0 w-[396px] h-[922px] aspect-[1.5] object-cover"
        alt="Sports"
        src={sports21}
      />

      <div className="absolute top-[859px] left-px w-[396px] h-[63px] bg-black" />

      <div className="absolute top-[885px] left-[34px] w-[348px] [font-family:'Inter-Bold',Helvetica] font-bold text-white text-4xl tracking-[0] leading-[normal]">
        VAHINI-25018547
      </div>

      <div className="absolute top-0 left-px w-[396px] h-[91px] bg-[#9dc6d6]" />

      <div className="absolute top-[26px] left-[21px] w-[361px] [font-family:'Inter-BoldItalic',Helvetica] font-bold italic text-[#0804f5] text-[32px] tracking-[0] leading-[normal]">
        REGISTRATION FORM
      </div>

      {formFields.map((field) => (
        <div key={field.id}>
          <div
            className={`absolute ${field.top} ${field.left} ${field.width} ${field.height} ${field.bg}`}
          />
          <label
            htmlFor={field.id}
            className={`absolute ${field.labelTop} ${field.labelLeft} ${field.labelWidth} [font-family:'Inter-BoldItalic',Helvetica] font-bold italic text-black text-2xl tracking-[0] leading-[normal]`}
          >
            {field.label}
          </label>
          <input
            id={field.id}
            name={field.name}
            type={field.type}
            value={formData[field.name as keyof typeof formData]}
            onChange={handleChange}
            className={`absolute ${field.inputTop} ${field.inputLeft} ${field.inputWidth} h-[32px] bg-transparent border-b border-black [font-family:'Inter-BoldItalic',Helvetica] font-bold italic text-black text-xl tracking-[0] leading-[normal] focus:outline-none`}
            aria-label={field.label}
          />
        </div>
      ))}
    </div>
  );
};

```
```


import prize1 from "./prize-1.png";
import rectangle18 from "./rectangle-18.svg";

export const AndroidCompact = (): JSX.Element => {
  const prizes = [
    {
      label: "1st-5000/-",
      bg: "bg-[#b5b281]",
      top: "top-[284px]",
      textTop: "top-[304px]",
      textLeft: "left-[95px]",
      height: "h-[81px]",
    },
    {
      label: "2nd-4000/-",
      bg: "bg-[#d0d19b]",
      top: "top-[398px]",
      textTop: "top-[420px]",
      textLeft: "left-24",
      height: "h-[74px]",
    },
  ];

  return (
    <div className="bg-white w-full min-w-[412px] min-h-[917px] relative">
      <img
        className="absolute top-0 left-0 w-[412px] h-[917px] aspect-[1.5] object-cover"
        alt="Prize"
        src={prize1}
      />

      <div className="absolute top-0 left-0 w-[412px] h-[90px] bg-[#474642]" />

      <div className="absolute top-[22px] left-11 w-[368px] [font-family:'Inter-BoldItalic',Helvetica] font-bold italic text-white text-[32px] tracking-[0] leading-[normal]">
        CASH PRIZE DETAILS
      </div>

      <div className="absolute top-[844px] left-0 w-[412px] h-[73px] bg-black" />

      <div className="absolute top-[867px] left-14 w-[356px] [font-family:'Inter-Bold',Helvetica] font-bold text-white text-[32px] tracking-[0] leading-[normal]">
        VAHINI-25018547
      </div>

      <p className="absolute top-[104px] left-[27px] w-[330px] [font-family:'Inter-Bold',Helvetica] font-bold text-[#e2fa04] text-[32px] tracking-[0] leading-[normal]">
        For any sports their is a cash prize for winners
      </p>

      <div className="absolute top-[284px] left-[43px] w-[300px] h-[81px] bg-[#b5b281]" />
      <div className="absolute top-[304px] left-[95px] w-[252px] [font-family:'Inter-Bold',Helvetica] font-bold text-black text-[32px] tracking-[0] leading-[normal]">
        1st-5000/-
      </div>

      <div className="absolute top-[398px] left-[43px] w-[300px] h-[74px] bg-[#d0d19b]" />
      <div className="absolute top-[420px] left-24 w-[250px] [font-family:'Inter-Bold',Helvetica] font-bold text-black text-[32px] tracking-[0] leading-[normal]">
        2nd-4000/-
      </div>

      <img
        className="absolute top-[504px] left-[43px] w-[300px] h-[66px]"
        alt="Rectangle"
        src={rectangle18}
      />
      <div className="absolute top-[515px] left-[99px] w-[244px] [font-family:'Inter-Bold',Helvetica] font-bold text-black text-[32px] tracking-[0] leading-[normal]">
        3rd-3000/-
      </div>
    </div>
  );
};

```
```
export const AndroidCompact = (): JSX.Element => {
  return (
    <div className="bg-[#e3acd5] w-full min-w-[412px] min-h-[917px] relative">
      <div className="absolute top-[824px] left-0 w-[412px] h-[93px] bg-black" />

      <div className="absolute top-[850px] left-[29px] w-[353px] [font-family:'Inter-Bold',Helvetica] font-bold text-white text-[32px] tracking-[0] leading-[normal]">
        VAHINI-25018547
      </div>

      <div className="absolute top-[77px] left-[34px] w-[348px] [font-family:'Inter-Bold',Helvetica] font-bold text-[#510941] text-[40px] tracking-[0] leading-[normal]">
        !...THANKYOU...!
      </div>

      <p className="absolute top-[333px] left-14 w-[340px] [font-family:'Inter-ExtraBold_Italic',Helvetica] font-extrabold italic text-[#1924bb] text-[32px] tracking-[0] leading-[normal]">
        COME AND PARTICIPATE AND WIN THE PRIZE...!
      </p>
    </div>
  );
};


```

## OUTPUT:


<img width="1920" height="1080" alt="Screenshot (87)" src="https://github.com/user-attachments/assets/21edd589-7919-4c1c-9d51-19ca6f66df06" />

## RESULT:
The program to design, develop and deploy a web application for event registration using Figma UI tool is completed successfully.
