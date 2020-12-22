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

4. **[Browser Testing](#Browser-testing)**

5. **[Bugs](#Bugs)**

---

# **Code Validators**
Code validators were used on all .html and .css pages to ensure the code used was valid.

## W3C Markup Validation Service (https://validator.w3.org/)

Code was validated through Direct Input by copying and pasting the html content directly in to the validator:

index.html

- No errors or warnings to show on index.html

![index.html Markup validation](tests/index.html_MarkupValidation.PNG)


gallery.html

- 2x error messages were generated initially.  Both references spaces in .jpg names: these spaces will be removed and the img source updated accordingly.  
- Retesting indicated no additional issues remain.

![gallery.html Markup Validation](tests/gallery.html_MarkupValidation.PNG)

contact-us.html

- 2x error messages were generated initially.  Both referenced datetime value used: having reviewed the relevant documentation datetime is a legal value and so no change will be made at this time.

![contact-us.html Markup Validation](tests/contact-us.html_MarkupValidation.PNG)


## W3C Markup CSS Service (https://jigsaw.w3.org/css-validator/validator.html.en)

Code was validated by Direct Input by copying and pasting directly in to the validator:

style.css

- 2x error messages and 1x warning message were generated initially.  Error messages referenced missing units from margins: these margin values were updated accordingly.
- Retesting indicated no additional issues remain.
- The error message outlined that imported style sheets have not been checked; this error has been noted and no further action will be taken at this time.

![style.css CSS Validation](tests/style.css_CSSValidation.PNG)

---
# **User story testing**

The user stories from the README.md file were used as a basis for testing.  For each test case the test acceptance criteria, evidence/observations and outcome have been recorded:

**1. "As a user I want to find out which sample bottle/type I require so that I can sample my patient correctly"**

Acceptance criteria:
- End users should be able to get information for P-L Services website on laboratory tests and which bottles they should use.  
- This information should be available on all device sizes.

Evidence/Oservations:
- Each department section (Clinical Biochemsitry, Haematology, Microbiology) on the index.html page contains clickable links to testing information.  Sample information, Expected Turnaround time and notes are detailed on each pop-out modal
- All buttons/pop out checked on desktop (MS-Edge, Chrome and Firefox).
- All buttons operate as expected on ipad/safari browser.
- All buttons operate as expected on android mobile phone (running Android 10 and MS Edge mobile version)
- Following minor issues noted:
    - Word Department missing from Clinical Biochemistry section (index.html will be amended accordingly)
    - Group/AB Screen does not open at correct size on desktop (index.html will be amended accordingly)
    - LFT Notes section related to different assay (index.html will be updated accordingly)
    - Micro Invest pop out details MRSA information (index.html will be updated accordingly)

Outcome: Test successful

---

**2. "As a user I want to be able to tell why my patients blood results are taking longer than normnal so I can discharge patients as quickly as possible"**

Acceptance criteria:
- End users should be able to tell immediately from the P-L Services website of any issues with the laboratories services  
- This information should be available on all device sizes.

Evidence/Oservations:
- This information should have been displayed on the homepage; however it cannot be seen displayed on any device size.  Inspection of index.html shows code for a Warning Bar is present but is currently commented out - this is because the developer is not able to utilise the functionality which would be needed for this feature to operate correctly.  This feature has been added to the features for futher releases section of the README.md file.

Outcome: Test unsuccessful

---

**3. "As a user I want to have the most suitable staff member contact me about a laboratory result so that I can treat my patient properly**

Acceptance criteria:
- End users should be able to find laboratory contact information on the P-L Services website 
- This information should be available on all device sizes.

Evidence/Oservations:
- Contact information for each department is listed on the contact-us.html page.  That page also has a form which allows users to cantact the laboratory about any issues they have with samples.
- Contacts & form checked on desktop (MS-Edge, Chrome and Firefox).
- Contacts & form checked on ipad/safari browser.
- Contacts & form checked on android mobile phone (running Android 10 and MS Edge mobile version)
- Following minor issues noted:
    - Margin/spcing below words of contact card on desktop is not correct (style.css will be amended accordingly)
    - Color of telephone numbers on ipad is not correct (style.css will be amended accordingly)

Outcome: Test successful

---

**4. "As a user I want to find out what goes on behind those closed doors in the laboratory so I have confidence in the work they're doing"**

Acceptance criteria:
- End users should be able to see media, on the P-L Services website, which outlines what goes on within the laboratory 
- This information should be available on all device sizes.

Evidence/Oservations:
- The gallery page has images which show the work of the laboratory
- Gallery images and text checked on desktop (MS-Edge, Chrome and Firefox).
- Gallery images and text checked on ipad/safari browser.
- Gallery images and text checked on android mobile phone (running Android 10 and MS Edge mobile version)

Outcome: Test successful

---

**5. "As a business manager I want end users not to be calling asking about sample bottles/test so laboratory staff can concentrate on testing"**

Acceptance criteria:
- End users should have an alternative means, on the P-L Services website, to contact the laboratory 
- This alternative means should be available on all device sizes.

Evidence/Oservations:
- Contact Us form on the contact-us.html page gives users an alterntive means of contacting laboratory
- Contact Us form displays correctly on desktop (MS-Edge, Chrome and Firefox).
- Contact Us form displays correctly on ipad/safari browser.
- Contact Us form displays correctly on android mobile phone (running Android 10 and MS Edge mobile version)

Outcome: Test successful

---

**6. "As a business manager I want to showcase the laboratory in the best light so that I can get additional funding"**

Acceptance criteria:
- The P-L Services website, should display high quality content throughout 
- This information should be available on all device sizes.

Evidence/Oservations:
- The gallery page has high quality images which show the work of the laboratory
- The website itself displays responsively on all device sizes to aid with the user experience

Outcome: Test successful

---

**7. "As an organisation I want to highlight the achievements of our laboratory and staff so I can demonstrate excellence of service"**

Acceptance criteria:
- Achievements of laboratory and staff should be displayed on P-L Services website 
- This information should be available on all device sizes.

Evidence/Oservations:
- Additional content could be added to index.html and the gallery.html pages to further highlight specific laboratory achievements; however none are currently displayed.  This has been added to the features for futher releases section of the README.md file.

Outcome: Test unsuccessful

---

# **Responsiveness Testing**

The website has been designed to be responsive to different screen sizes. The following has been checked on both mobile (android mobile phone running Android 10 and MS Edge mobile version) and tablet (ipad/safari browser) sized devices.

## Mobile

- Header - the navigation elements of the header section collapse under a menu button as expected. Separation markers between items (seen on larger screens) are not visible as expected. Clicking the logo returns the user to the Home page from all pages.  Clicking the Home, Gallery and Contact Us links navigate the user to the respective pages successfully
- Hero section - hero image is not displayed on mobile as expected and has been replaced with coloured background
- 3 department sections - buttons are reduced in size with smaller font sizing used; layout has been amended (2x columns of buttons side by side) with the departmental information pushed beneath the buttons filling the entire width of the screen. All buttons previously tested in User stories testing. All buttons size and align correctly
- Footer - the separation markers have been removed at this screen size as expected. Links display in 2x columns. Clicking each of the social media links opens the relevant website (Facebook, Youtube or Twitter) in new windows as expected.  The hospital link opens a new window with the P-L Services website as this is not yet linked to a larger organisation website.

## Tablet 

- Header - the navigation elements have their font size reduced as expected. Separation markers between items remain as expected. Clicking the logo returns the user to the Home page from all pages.  Clicking the Home, Gallery and Contact Us links navigate the user to the respective pages successfully
- Hero section - hero image is displayed at this screen size as expected
- 3 department sections - size of the buttons has been amended to ensure they can be clicked easily on this device size with smaller font sizing used; layout has been amended (2x columns of buttons side by side) with the departmental information pushed beneath the buttons filling the entire width of the screen. All buttons previously tested in User stories testing and size/align correctly
- Footer - Links display across the page with the font size being reduced to reflect the screen size. Clicking each of the social media links opens the relevant website (Facebook, Youtube or Twitter) in new windows as expected.  The hospital link opens a new window with the P-L Services website as this is not yet linked to a larger organisation website.

---

# **Browser testing**
The website has been tested on the following browsers:
- Firefox browser (Version 84.0 (64-bit))
- Microsoft Edge browser (Version 87.0.664.66 (Official build) (64-bit))
- Chrome Browser (Version 87.0.4280.88 (Official Build) (64-bit))
- Safari Browser
- MS Edge Mobile (Version45.11.24.5118)

---

# Bugs
The following bugs were noted during development of the P-L Services website:
- 

