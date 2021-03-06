# Website and Lab Manual

## Website

### Details

URL: [pielab-science.com](https://pielab-science.com)

Username and password: email Sara or David for this information.

### Purpose

PR for the PIE lab
 - Who's part of the PIE lab
 - What are we currently doing?
 - (If actively recruiting) landing page for new recuirts
 - (If ongoing study) landing page for study participants
 
### Current sections

- [What we study](https://pielab-science.com/research)
- About
- Current lab members (with a page for each)
- Friends of the lab
- [Cooling on the rack](https://pielab-science.com/blog/) (news)
 
### How to update
  - Go to [pielab-science.com/admin](https://pielab-science.com/admin) and log in (see above for username/password details)
  - See sections below for updating specific aspects

#### Your profile
 - Go to the Media section (on the left-hand menu) and click Add New
 - Drop file into box, or select using menus
 - Go to Pages (left-hand menu) and hover over your page -- select Edit with Elementor
 - Use the interface to change text, upload a new picture, include links to other pages, whatever you want!
 - Be sure to click Update before leaving the page.
  
#### Your CV
 - Go to the Media section (on the left-hand menu) and click Add New
 - Drop file into box, or select using menus
 - Go to Pages (left-hand menu) and hover over your page -- select Edit with Elementor
 - Hover over the box that contains the text. A pencil will show up in the corner; click on it.
 - On the left-hand side, an Edit Text Editor menu will show up. Find the link to your CV. If you click on it, the link to the PDF will appear. You can either
       - Edit the link to match the new upload (involves changing the year and month of upload and the name of the file as it was uploaded to Wordpress), or
       - Delete the current link to the CV and add a new one with the Add Media button.
 - Be sure to click Update before leaving the page.
 
#### Troubleshooting

*If the page doesn't update*

- Wait 15 minutes and reload the webpage. 
- Clear the wordpress Cache
     - On the wordpress dashboard, click on Mangaged Wordpress (top) and select Flush Cache. This will take a minute or so.
- Clear your browser Cache
     - This will be under your browser's settings. 
     - Try opening the webpage in an incognito window as well, to see if this is a problem.


## Lab Manual

### Clone lab manual to your computer

*Notes*:

  1. *this is only available to current graduate students and PIs in the lab.*
  2. *the steps listed here only need to be followed on the first use.*

**Necessary materials:**

- Git
- GitHub account with access to [PIElab organization](https://github.com/orgs/pie-lab) 
- Rstudio that is connected to GitHub through your personal account.

1. Go to [manual repository](https://github.com/pie-lab/manual). 
2. Click on the green *Clone or download* button. 
3. Copy the link that appears. 
4. Open RStudio. Create a New Project.
5. Select Version Control and then Git. Name the project ``manual'' (so it matches the Rproj file that already exists in the repository. Save this project somewhere you will remember.

### Updating the manual [using the RStudio GUI]

**Before you make ANY changes:**

1. Open the manual RStudio project. 
2. Pull the most recent version of the manual using the blue down arrow. 

**Make any changes to the manual as you think are necessary.**

3. In the Build tab in Rstudio, click on *Build Book*.
4. In the Git tab, click Commit. In the commit message section, briefly (4-5 words max) describe the changes you made. Example: wrote updating manual section. In the window on the left, the easiest thing to do is select everything and click *Stage*. Ensure all the boxes are checked. This will be slower than only selecting the parts of the book that have changed. However, the nature of an RMarkdown book is many changes affect most parts of the book (because it changes you navigate to them). If you miss a change you have made, the book may not render properly online. Click the *Commit Button*.
5. Click on the green up arrow to push the book to GitHub, which will update the book online.

### Updating the manual [using the terminal in Rstudio]

**Before you make ANY changes:**

1. Open the manual RStudio project. 
2. In the terminal window of RStudio, pull the most recent version using this code:


```git
git pull
```


**Make any changes to the manual as you think are necessary.**

3. In the Build tab in Rstudio, click on *Build Book*.
4. In the Terminal, commit your changes. The easiest way to do this is to type:


```git
git add .
```

where the period indicate to include anything. Alternatively, you can add only specific files, if you don't want to commit everything. For example:


```git
git add file.R
```
or:

```git
git add path/file.R
```
To commit your changes, type:

```git
git commit -m "message here"
```
Be sure to include a message describing the changes. Keep the message short.

Finally upload your changes with:

```git
git push
```
You're done!

### Requesting updates

You may be unable to make changes to the lab manual because you are not authorized to make changes or don't know the answer to the question. In either of those cases, you make create an issue on the GitHub page to alert the lab to the need for additional material. To do so:

1. Go to the [Issues tab](https://github.com/pie-lab/manual/issues) on the GitHub page for the lab manual.
2. Click on New Issue and complete the form. Be sure to include as much detail as you can about the issue you have. The more detailed your request, the better the information in the manual will be. 

*Note: create one issue request for each question you have. Don't put lots of requests into a single issue.*

Other lab members can take responsibility for this issue by self-assigning the issue. Once material has been added to the manual, the member responsible for resolving the issue should reply to the original poster, including a link to the relevant section. If this meets the need of the original poster, they should reply so and the issue can be marked as closed. 


