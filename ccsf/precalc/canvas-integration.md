[edtech site](citycollegesf.sharepoint.com/sites/OnlineLearningandEducationalTechnologyOLET/SitePages/OLET-Forms-and-Links.aspx?ga=1&xsdata=MDV8MDJ8amxvdmVAY2NzZi5lZHV8MTdjODkxZjc5N2RhNGZkNThlMjUwOGRlZDg1NDEwY2R8NWUwZjIyZDY4YTE2NDE3ZWJmM2FkMDgxYzk4YjM4ZDh8MHwwfDYzOTE4NjA1MjcyMzg3ODMzOXxVbmtub3dufFRXRnBiR1pzYjNkOGV5SkZiWEIwZVUxaGNHa2lPblJ5ZFdVc0lsWWlPaUl3TGpBdU1EQXdNQ0lzSWxBaU9pSlhhVzR6TWlJc0lrRk9Jam9pVFdGcGJDSXNJbGRVSWpveWZRPT18MHx8fA%3d%3d&sdata=RlhhaWVSSVN5dnFQdWlKdlVKTHpyY1FsQ012ZzJrYk4yUmJHYkJSOUhxYz0%3d&CT=1783285168290&OR=OWA-NT-Mail&CID=c9a0c2e3-f7d7-79a0-df07-6f4a71e10b5a&SI=NonSentItems)

# using the webwork app directly in canvas

To sync the WeBWorK exercises for Matt Boelkins' _[Active Prelude to Calculus](https://www.google.com/search?q=active+prelude+to+calculus&kgmid=/g/11hzwd64dn#sv=CBwSrAQK5QMS4gMKogNBSmlUNHRMOUhQbnhuWTNxaTNoMGR2UFFLTW0zdmVDMnVOR1d6VjdmYUJiU1ViNXotV2xWbGhnaHRXMHlaWW5xTlNpZnVYVnFIM2J3bk9vR2ZwckRaQU1DWkMwZkJ2X0trZzFTNkdSVzNCLVA5SUhCUjBuaWFwMm1QUUpnSDBwUDZPYmNZOGJWR0JRMkMzeHY0MFdObGZwbWRacy1JR3VzMDl0YmpKOVgwVXFieVBxcVNVZVdqZ25tc1dQNEctNmJqUWl6dkZNUTlFeVJUWmlKb19nNHRmcG1jSkhOb01aaEEwR19zRDBKUnM5UTM1ckJJaWxwS2xzMlZHUHRRWTl1WF9jU3Z5RDdCdmRZQTN5SGFxVW5IMnMxMW9zX2Q2bnRMb3BadUtORDJ1Z0VQUzRaLWo2TmNFT0RXcnMySGdlR2VyemthOVJzdjY2WU1Uc1dZY1ZyUzdvbTEyaml5SE5nb2M0a2I0TE1RbWlmTkcxRjliclIxZTQ0N2wwMjhlcWZVUndMTGhDa0ZnamZDN0ZxZWJteEdha2dGODBRUGhmbDFREhdIMjVNYXZtMkRvbTgwUEVQZ3ZyZm9RYxoiQURzcjlmVDNpUVFuX0JxbThKZnN6bVlvQnRyVjkzVmlOZxIENzg1NBoBMyIfCgFxEhphY3RpdmUgcHJlbHVkZSB0byBjYWxjdWx1cyIWCgVrZ21pZBINL2cvMTFoendkNjRkbigAGEUgyLWU5Qg)_ textbook with your Canvas shell, you need to connect Canvas to your school’s WeBWorK server using an LTI (Learning Tools Interoperability) External Tool integration. This setup allows single sign-on for students and automatically passes WeBWorK grades back to your Canvas gradebook. [1, 2, 3]

_(Note: The embedded WeBWorK exercises inside the free HTML version of the textbook are strictly anonymous. To track student grades, you must deploy the official problem sets from the WeBWorK Open Problem Library (OPL) or use a commercial bridge like Edfinity)._ [2, 4, 5]

Follow this step-by-step process to sync the exercises.

---

## Step 1: Request Your Server Credentials

Before touching Canvas, you need information from your department's WeBWorK Server Administrator:

- The WeBWorK Server Domain/URL (e.g., `https://webwork.yourschool.edu/`)
- Consumer Key
- Shared Secret [1]

## Step 2: Add WeBWorK as an App in Canvas

You must register the WeBWorK server as a trusted external application inside your Canvas course settings. [6, 7]

1. Go to your Canvas course and click Settings at the bottom of the left navigation menu. [7]
2. Select the Apps tab at the top and click View App Configurations. [7]
3. Click the + App button. [7]
4. Set the Configuration Type to Manual Entry. [7]
5. Fill out the form fields:
    
    - Name: `WeBWorK`
    - Consumer Key: _(Paste the key from Step 1)_
    - Shared Secret: _(Paste the secret from Step 1)_
    - Domain: Your server domain (e.g., `webwork.yourschool.edu`)
    - Privacy: Set to Public (Crucial so WeBWorK can map usernames to the gradebook). [1, 6, 7]
    
6. Click Submit.

## Step 3: Find the Active Prelude Problems in WeBWorK

Matt Boelkins' exercises are hosted inside the global Open Problem Library. [5]

1. Log into your instructor account directly on your institution's WeBWorK platform.
2. Open your specific Precalculus course shell and click on Library Browser.
3. Click the OPL Directory button.
4. From the dropdown menus, look for the directory containing the author's target problems (usually titled under `Westmont/ActiveCalculus/...` or specifically indexed under `Active Prelude to Calculus`).
5. Select the relevant chapter and section, assign the problem sets to your WeBWorK course, and copy the URL of the assigned problem set. [3, 8]

## Step 4: Link the Individual Exercises into Canvas

Now, build the assignments in Canvas to sync the two systems. [1, 3]

1. In Canvas, navigate to the Assignments page and click + Assignment. [1]
2. Set your points, assignment group, and instructions. [1, 3]
3. Scroll down to Submission Type and select External Tool from the dropdown menu. [1, 3]
4. Paste your specific WeBWorK assignment URL into the Enter or find an External Tool URL box.
    
    - _URL format example:_ `https://yourschool.edu` [1, 3]
    
5. Critical Checkbox: Check the box that says "Load This Tool In A New Tab". _(WeBWorK mathematical notation often breaks or compresses poorly when squished inside a Canvas iframe)._ [1, 3]
6. Save and Publish the assignment. [3]

---

## ⚠️ Critical Warning for Grading Sync

Students must click the Canvas assignment link to access WeBWorK. If they log directly into the independent WeBWorK website without passing through Canvas, their scores will not sync to your Canvas gradebook. Instruct your students to always launch the assignments directly from your Canvas modules. [3]

Do you already have a WeBWorK course shell set up for this semester by your IT department, or do you need assistance looking into alternative platforms like Edfinity which provide commercial, pre-built _Active Prelude_ integration paths?

  

[1] [https://wiki.openwebwork.org](https://wiki.openwebwork.org/wiki/LTI_Authentication_%28for_WeBWorK_2.18_or_newer%29)

[2] [https://activecalculus.org](https://activecalculus.org/apc/)

[3] [https://www.youtube.com](https://www.youtube.com/watch?v=zV2PzqyXNBA)

[4] [https://textbooks.aimath.org](https://textbooks.aimath.org/textbooks/approved-textbooks/boelkins/)

[5] [https://rfcia.com.br](https://rfcia.com.br/wp-content/uploads/2023/09/active-prelude-to-calculus-matthew-boelkins.pdf)

[6] [https://forums.openwebwork.org](https://forums.openwebwork.org/mod/forum/discuss.php?d=5012)

[7] [https://webworkgoehle.blogspot.com](http://webworkgoehle.blogspot.com/2016/03/webwork-lti-authentication.html)

[8] [https://activecalculus.org](https://activecalculus.org/2016/08/10/active-calculus-preview-activities-in-webwork/)

# libretext adapt
https://adapt.libretexts.org/

## from the libretext side

_Active Prelude to Calculus_ is hosted on [Mathematics LibreTexts](https://math.libretexts.org/Bookshelves/Precalculus/Active_Prelude_to_Calculus_%28Boelkins%29). LibreTexts has its own free homework system called ADAPT. [5]

- What you can do: You can create a free instructor account on ADAPT. They have a massive centralized repository of WeBWorK questions, including those from the open-source _Active Calculus_ library.
- Canvas Link: ADAPT supports full LTI integration, allowing you to link assignments and sync grades to Canvas without charging students anything.

---

Finding the exact _Active Prelude to Calculus_ WeBWorK problems in LibreTexts ADAPT requires navigating their centralized library of over 300,000 open-source questions. Because ADAPT aggregates all public OER (Open Educational Resources) courses, the easiest way to pull these into your Canvas course is by searching for them globally or locating them through the WeBWorK Open Problem Library (OPL) addresses. [1, 2, 3, 4]

The exact steps to find and compile these problems into an assignment include:

### Step 1: Create an Assignment Shell

Before searching for questions, you need an assignment container ready to hold them. [1, 2]

1. Log into your instructor dashboard on [LibreTexts ADAPT](https://libretexts.org/academy/adapt).
2. Click into your Canvas-linked course shell (or click Create New Course if you haven't made one yet).
3. Go to the Assignments tab and click Create New Assignment. Give it a name (e.g., "Section 1.1 Homework") and save it. [1, 2, 5, 6, 7]

### Step 2: Search the ADAPT Question Repository

1. Click on the title of your newly created assignment, then select the Add Questions button.
2. At the top right of the dashboard, click Search Questions.
3. Change the search filter from "My Questions" to "Public Questions" or "All Questions". [1, 6, 7, 8]

### Step 3: Use the Correct Search Strategy

Because the problems originated in the WeBWorK Open Problem Library (OPL), you can find them using two main methods: [4, 9]

- Method A: Text & Author Search (Fastest)  
    In the search bar, type `Active Prelude Calculus` or `Boelkins`. This will bring up any questions or entire assignment blocks that other instructors have already imported publicly into ADAPT. [1, 6]
- Method B: WeBWorK OPL Directory Search  
    If a direct keyword search yields too many mixed results, filter your search technology to WeBWorK. The _Active Calculus_ family of problems is filed under the Open Problem Library directory path: `Westmont/ActiveCalculus/`. Look for folders or tags matching `ActiveCalculus/Preview_C_S` (where C is chapter, S is section). [3, 9]

### Step 4: Import the Problems to your Assignment

1. Review the search results. Click the "View" or eye icon to preview a question and ensure the mathematical algorithms are loading correctly.
2. Click the Add to Assignment (or Clone Question) button next to the problems you want.
3. Repeat this for each section's problem set. [1, 2, 6, 7]

---

Once your assignment is filled with the correct questions, would you like the steps to link this ADAPT assignment directly to your Canvas modules using the External Tool (LTI) settings? [2]

Linking your LibreTexts ADAPT assignments to Canvas Modules requires a one-time configuration in ADAPT followed by a standard external tool layout in Canvas. [1, 2]

Follow this exact blueprint to pair the systems and initiate automatic grade passback:

### Phase 1: Prep the ADAPT Course

Before switching to Canvas, you must explicitly allow the ADAPT course to communicate with an external learning management system. [3, 4]

1. Log into your [LibreTexts ADAPT Dashboard](https://libretexts.org/academy/adapt).
2. Click the Course Properties (gear icon) next to your _Active Prelude_ course.
3. Scroll down to the LMS section and tick the radio button to Yes.
4. Click Save. [2, 3, 4]

_Note: If your course features multi-section tracking, navigate to the Sections tab to copy the auto-generated Access Code. Students will need to input this code just once the first time they launch an assignment._ [4]

### Phase 2: Create the Graded Assignment in Canvas

Canvas acts as the gradebook anchor, so you must establish the assignment shell inside your native course menu first. [5]

1. Open your Canvas course and click Assignments → + Assignment.
2. Set your basic parameters: name it (e.g., _Section 1.1 Homework_), input your target points, and select your grading group.
3. Under Submission Type, select External Tool from the dropdown list.
4. Click Find, scroll through the application list until you locate ADAPT, and hit Select.
5. CRITICAL: Check the box for "Load This Tool In A New Tab". ADAPT requires a dedicated viewport to render the complex WeBWorK frames correctly.
6. Click Save and Publish. [1, 2, 5]

### Phase 3: Handshake the Two Platforms

Now you must map the Canvas assignment shell to the specific ADAPT module you built earlier. [5, 6]

1. Click the newly published assignment inside Canvas.
2. Click the large button labeled Load [Assignment Name] in a new window.
3. A pairing wizard will pop up in the new tab. Select your _Active Prelude_ course from the first dropdown menu.
4. Select the matching homework block from the second dropdown menu.
5. Click Link Assignment. The WeBWorK problem grid will load instantly, confirming a successful link. [5]

### Phase 4: Organize Into Your Modules

With the linkage active, you can drop the live tool cleanly into your regular module streams.

1. Go to Modules in your Canvas sidebar navigation menu.
2. Find your target week/topic module and click the + (Add Item) button.
3. In the dropdown menu, select Assignment (do _not_ select External Tool here, or it will skip the grade passback framework).
4. Choose the freshly mapped ADAPT assignment from the list and click Add Item. [7]

---

If you encounter any layout roadblocks, let me know:

- Do you see ADAPT listed under the External Tools menu in Canvas, or do we need to contact your IT admin to install it?
- Do you want to review how ADAPT calculates partial credit before passing it back to Canvas? [8]

## from the canvas side

Yes, CCSF Canvas supports the ADAPT tool, primarily through the Academic Senate for California Community Colleges (ASCCC) initiative for Open Educational Resources (OER). [1, 2]

### Key Integration Features

- LTI Integration: Instructors can embed ADAPT assignments directly inside their [CCSF Canvas](https://www.ccsf.edu/about-ccsf/administration/academic-institutional-affairs/office-instruction/office-online-learning-and-educational-technology/canvas) course modules.
- Gradebook Syncing: Grades earned by students on ADAPT assessments automatically pass back to the Canvas gradebook.
- Diverse Assessments: The tool enables native question formats like multiple-choice, matching, and fill-in-the-blank. [1, 3, 4, 5, 6]

### How to Access It

- Instructors: To use it, you must build your assignments directly via the LibreTexts ADAPT Platform and switch the course properties LMS setting to "Yes" to link it with Canvas. [5, 7]
- Students: You will typically interact with ADAPT seamlessly inside your daily Canvas assignments unless a system outage occurs, in which case your instructor may prompt you to log in directly via [LibreTexts](https://commons.libretexts.org/insight/adapt-switching-to-direct-access-during-the-canvas-instructure-outage). [5]

Are you a faculty member trying to set up ADAPT in your shell, or a student trying to complete a specific assignment? Let me know so I can provide the right troubleshooting or setup steps!

To set up LibreTexts ADAPT in your CCSF Canvas shell, you will need to link your courses using an LTI External Tool configuration. Because CCSF operates under the ASCCC OERI guidelines, the global LTI keys are typically managed at the institutional level, meaning you won’t need to input raw secret keys yourself. [1]

### Step 1: Configure Course Properties in ADAPT

Before linking to Canvas, you must enable LMS integration on your assignment or course within the ADAPT portal.

1. Log into your account on the LibreTexts ADAPT Platform.
2. Open the Course you want to link.
3. Click on Course Properties (or settings).
4. Locate the LMS (Learning Management System) configuration option.
5. Toggle or set LMS Enabled to Yes.
6. Keep this tab open; you will need the specific Assignment/Course ID numbers generated by ADAPT. [2]

### Step 2: Add the ADAPT Tool to a Canvas Assignment

Do not look for ADAPT in the left-hand navigation sidebar; it is embedded directly inside Canvas Assignments.

1. Log into your [CCSF Canvas Faculty Account](https://www.ccsf.edu/about-ccsf/administration/academic-institutional-affairs/office-instruction/office-online-learning-and-educational-technology/canvas) and open your course shell.
2. Navigate to Assignments and click + Assignment.
3. Scroll down to the Submission Type area.
4. Click the dropdown menu and select External Tool.
5. Click the Find button.
6. Scroll through CCSF's preconfigured tool list and click ADAPT (or _LibreTexts ADAPT_). [2, 3]

### Step 3: Link the Specific Assessment

1. Once you select ADAPT from the list, a mini-window will prompt you to log into your ADAPT account (if you aren't already logged in within the same browser session).
2. Select the specific ADAPT Course and Assignment you want to map to this Canvas entry.
3. Click Link/Submit.
4. Check the box that says Load This Tool In A New Tab (this provides a cleaner user experience for students and avoids iframe rendering errors).
5. Set your point value, assign dates, and click Save and Publish. [4]

### Important Faculty Tips

- Automatic Grade Passback: Once synced, grades from ADAPT sync automatically back to your Canvas gradebook. However, the sync triggers _after_ a student submits the assignment in ADAPT.
- Canvas Shell Sharing: If you are collaborating with other CCSF faculty using pre-built question banks—such as the regional OpenStax Microbiology Ancillary (OSMA) ADAPT Project led out of CCSF—you can export and import these shared modules directly into your sandbox. [1, 5]

Are you building your own custom question banks in ADAPT, or are you importing a shared textbook blueprint from another instructor? I can give you explicit steps for either workflow!

  

[1] [https://libretexts.org](https://libretexts.org/2024/11/19/spotlight-on-the-openstax-microbiology-ancillary-osma-adapt-project)

[2] [https://www.ccsf.edu](https://www.ccsf.edu/about-ccsf/administration/academic-institutional-affairs/office-instruction/office-online-learning-and-educational-technology/canvas)

[3] [https://www.uab.edu](https://www.uab.edu/ctl/learning-technologies/guides/great-river-learning-instructor-access)

[4] [https://www.scribd.com](https://www.scribd.com/document/905566010/How-Do-I-Use-Files-as-a-Student-Instructure-Community-484)

[5] [https://community.instructure.com](https://community.instructure.com/en/kb/articles/660893-how-do-i-send-a-module-to-another-instructor)

[1] [https://www.asccc.org](https://www.asccc.org/events/integrating-adapt-canvas)

[2] [https://asccc-oeri.org](https://asccc-oeri.org/2023/09/08/integrating-adapt-in-canvas/)

[3] [https://de.santarosa.edu](https://de.santarosa.edu/adapt)

[4] [https://www.ccsf.edu](https://www.ccsf.edu/about-ccsf/administration/academic-institutional-affairs/office-instruction/office-online-learning-and-educational-technology/canvas)

[5] [https://commons.libretexts.org](https://commons.libretexts.org/insight/adapt-switching-to-direct-access-during-the-canvas-instructure-outage)

[6] [https://de.santarosa.edu](https://de.santarosa.edu/adapt)

[7] [https://www.youtube.com](https://www.youtube.com/watch?v=ELN_348JNYA)
## links

[1] [https://researchguides.mvc.edu](https://researchguides.mvc.edu/libretexts/adapt)

[2] [https://chem.libretexts.org](https://chem.libretexts.org/Courses/Remixer_University/Mastering_ADAPT%3A_A_User%27s_Guide/04%3A_Using_ADAPT_as_an_Instructor/4.11%3A_Coupling_ADAPT_Assignment_to_Canvas_Assignments)

[3] [https://tic.miracosta.edu](https://tic.miracosta.edu/adapt-libretexts-free-homework-system/)

[4] [https://canvashelp.fullerton.edu](https://canvashelp.fullerton.edu/m/LibreTexts/l/1612109-how-do-i-set-my-libretexts-adapt-course-to-communicate-with-canvas)

[5] [https://canvashelp.fullerton.edu](https://canvashelp.fullerton.edu/m/LibreTexts/l/1610170-how-do-i-connect-libretexts-adapt-to-my-course-gradebook)

[6] [https://commons.libretexts.org](https://commons.libretexts.org/insight/coupling-adapt-courses-to-canvas-via-lti-only)

[7] [https://tuftsedtech.screenstepslive.com](https://tuftsedtech.screenstepslive.com/s/18992/m/73355/l/1273150-how-do-i-add-link-files-assignments-discussions-or-quizzes-to-a-canvas-module)

[8] [https://commons.libretexts.org](https://commons.libretexts.org/insight/adapt-canvas-coupling-behavior-via-api)

  

[1] [https://www.youtube.com](https://www.youtube.com/watch?v=LaPrV2WtipM&t=3)

[2] [https://www.youtube.com](https://www.youtube.com/watch?v=Cbda2SOmemU&t=3)

[3] [https://www.youtube.com](https://www.youtube.com/watch?v=SpAeENtBf6k&t=12)

[4] [https://chem.libretexts.org](https://chem.libretexts.org/Courses/Remixer_University/LibreTexts_Construction_Guide_1e/05%3A_Interactive_Elements/5.11%3A_Adding_WeBWorK_Problems_to_LibreTexts)

[5] [https://bio.libretexts.org](https://bio.libretexts.org/Workbench/Neil%27s_Sandbox_Project/01%3A_WeBWorK_writing_guide/1.06%3A_Create_your_own_WeBWorK_problem_in_ADAPT)

[6] [https://libretexts.org](https://libretexts.org/academy/adapt)

[7] [https://libretexts.org](https://libretexts.org/academy/adapt)

[8] [https://researchguides.mvc.edu](https://researchguides.mvc.edu/libretexts/questionbanks)

[9] [https://activecalculus.org](https://activecalculus.org/2016/08/10/active-calculus-preview-activities-in-webwork/)

  

[1] [https://activecalculus.org](https://activecalculus.org/about/)

[2] [https://runestone.academy](https://runestone.academy/ns/books/index)

[3] [https://activecalculus.org](https://activecalculus.org/apc/)

[4] [https://edfinity.com](https://edfinity.com/products/5e155430bf3c011f3c2d13b8)

[5] [https://math.libretexts.org](https://math.libretexts.org/Bookshelves/Precalculus/Active_Prelude_to_Calculus_%28Boelkins%29)

# email from chrissy

Yes, with some work and a spirit of adventure. :-)

Thanks to Oscar Levin, it is now possible to have a page with WeBWorK exercises on it (and some other types of exercises) be zipped and uploaded to Canvas as a SCORM assignment, and students would open the Canvas assignment, see the page with the problems on it, complete the problems on the page right inside Canvas, and Canvas records the score for the assignment.  Each problem on the page is worth an equal amount. 

Someone could clone AC’s source, use PreTeXt to build a separate SCORM file for each of the end-of-section exercises without any of the other content, and then those zip files could be uploaded to Canvas as SCORM assignments.  I believe it would only take one person building the files once, and then all the files could be shared and uploaded by anyone.  (Except that not all the images in the WeBWorK exercises have alt-text yet, so the build process would likely need to be redone after that work is completed).

Someone tested and said that the SCORM assignment files also appeared to work in Moodle, but last I heard Blackboard was proving troublesome.  This is cutting edge work, so anyone wanting to try the SCORM method would need a tolerance for unexpected issues!

More established methods of assigning the end-of-section exercises to students for a grade including hosting the problems on a WeBWorK server, or using Runestone Academy, which can connect to Canvas via LTI 1.3 if your institution allows it: [https://landing.runestone.academy/instructors.html](https://landing.runestone.academy/instructors.html)

CSafranski@franciscan.edu

