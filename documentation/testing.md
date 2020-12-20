# **P&L Services Website Testing** 

The testing, which follows, has been completed on the initial version of the P&L Services Website between 20th December and 22nd December 2020.  
All testing was conducted on the site published on GitHub Pages (https://andrewboyd79.github.io/P-L-Services/)

## **Contents**
1. **[Code Validators](#Code-validators)**
    - [W3C Markup Validation Service](#W3C-markup)
    - [W3C CSS Validation Service](#W3C-CSS)
 
2. **[User Story testing](#User-story-testing)**

3. **[Responsiveness Testing](#Responsiveness-testing)**
    - [Mobile](#Mobile)
    - [Tablet](#Tablet)
    - [Desktop](#Desktop)

4. **[Browser Testing](#Browser-testing)**

5. **[Bugs](#Bugs)**

---

# **Code Validators**
Code validators were used on all .html and .css pages to ensure the code used was valid.

## W3C Markup Validation Service (https://validator.w3.org/)

Code was validated by Direct Input by copying and pasting directly in to the validator:

index.html

- No errors or warnings to show on index.html

![index.html Markup validation](documentation/tests/index.html_MarkupValidation.PNG)

gallery.html

- 2x error messages were generated initially.  Both references spaces in .jpg names: these spaces will be removed and the img source updated accordingly.  
- Retesting indicated no additional issues remain.

![gallery.html Markup Validation](documentation/tests/gallery.html_MarkupValidation.PNG)

contact-us.html

- 2x error messages were generated initially.  Both referenced datetime value used: having reviewed the relevant documentation datetime is a legal value and so no change will be made at this time.

![contact-us.html Markup Validation](documentation/tests/contact-us.html_MarkupValidation.PNG)

## W3C Markup CSS Service (https://jigsaw.w3.org/css-validator/validator.html.en)

Code was validated by Direct Input by copying and pasting directly in to the validator:

style.css

- 2x error messages and 1x warning message were generated initially.  Error messages referenced missing units from margins: these margin values were updated accordingly.
- Retesting indicated no additional issues remain.
- The error message outlined that imported style sheets have not been checked; this error has been noted and no further action will be taken at this time.

![style.css CSS Validation](documentation/tests/style.css_CSSValidation.PNG)

