# Devin Harris' work through of [The Odin Project](https://www.theodinproject.com/) [Foundations Path](https://www.theodinproject.com/paths/foundations/courses/foundations/)
## Installation Overview
- It's important to learn how to setup an **actual** development environment even though online in-browser editors can be helpful
- Running a Mac makes this easy because Odin Project assumes a unix-based system
  - Windows is not **OFFICIALLY** supported, we could use Windows with virtualization but Odin Project doesn't officially support it
## Text Editors
- We need to use a **true** **plain-text** code editor 
  -  There are a number of code editors but the Odin Project officially recommends using [VSCode](https://code.visualstudio.com/)
  -  Odin Project links out to [Microsoft's Basics Video Series on VS Code](https://code.visualstudio.com/docs/introvideos/basics)
## Command Line Basics
- It's important for a developer to know how to navigate around and interact with the computer through a command-line interface or terminal
- Odin Project walked through setting up the VS Code `code` invocation from terminal in VS Code
- Provided some great resources for working from the command line
  - [The art of the command line](https://github.com/jlevy/the-art-of-command-line#readme)
  - [Learn Enough Command Line to be Dangerous](https://www.learnenough.com/command-line-tutorial)
  - [ExplainShell.com](http://explainshell.com/)
  - [Unix/Linux Command Cheatsheet](https://files.fosswire.com/2007/08/fwunixref.pdf)
  - [Command Line Flashcards](https://flashcards.github.io/command_line/introduction.html)
  - [LearnLinuxTV - Command Line Video Series](https://www.youtube.com/playlist?list=PLT98CRl2KxKHaKA9-4_I38sLzK134p4GJ)
## Setting up Git
- Git is the most popular **version control system**, [GitHub](https://github.com/) is the most popular service with Git but GitHub is not Git
- We setup git
- We sign up for GitHub
- We create an SSH key
- We link that key with GitHub
- We test the SSH connection between GitHub and our machine
## Introduction to Git 
- The Odin Project walks us through version control with Git
- Git works on the local machine, we use GitHub as a remote repository where we can push Git files to
- Linked out to
  - [The Odin Project on GitHub](https://github.com/TheOdinProject)
  - [A great video on how Git can improve workflow](https://www.youtube.com/watch?v=8oRjP8yj2Wo)
  - [Git and GitHub in Plain English](https://blog.red-badger.com/blog/2016/11/29/gitgithub-in-plain-english)
## Git Basics 
- There is a basic **Git workflow**
  - These are the commands we will use 70-80% of the time we are working with Git 
### Git Workflow
- Create/Edit file
- `git status` - shows unstaged new/changed files
- `git add` - allows us to stage new/changed files
- `git status` - ensure all files we want committed are now staged
- `git commit -m {message}` - commit the staged files to the local repository with {message} as the commit message
- `git status` - verify that the working tree is clean
- `git log` - Verify that the commit was logged
- `git push origin main` - allows the local repository to be pushed up to GitHub for remote storage
- `git status` - verify that the working tree is clean
## Introduction to HTML and CSS
- **HTML** and **CSS** are the two foundational building blocks of the web
- HTML is the raw data (markup) of a page
- CSS is the language that adds style/adjusts presentation of the HTML
- HTML and CSS are not **technically** programming languages, they are markup languages
- Links out to [HTML vs CSS vs JavaScript](https://brytdesigns.com/html-css-javascript-whats-the-difference/)
## Elements and Tags
- Hypertext markup language (HTML) defines the structure and content of webpages
- HTML is made up of **Elements** and **Tags**
- HTML elements are made up of **opening** and **closing** **tags**
  - We can look at HTML **elements** as containers for content
- The Odin Project links out to a [listing of pre-defined HTML tags](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)
- It is important to use the **correct elements** to ensure that your sites can be indexed correctly, they also help assistive technologies like screen readers
- [Kevin Powell's Introdution to HTML](https://www.youtube.com/watch?v=LGQuIIv2RVA&list=PL4-IK0AVhVjM0xE0K2uZRvsM7LkIhsPT-)
## HTML Boilerplate
- ALL HTML documents need the same **basic structure** to be useful, this is called **boilerplate**
- **DOCTYPE** - all HTML pages start with a **DOCTYPE** element
  - `<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">`
  
  **We can Shorten this to**
  
  - `<!DOCTYPE html>`
- **HTML** - this element wraps the entire page
  - `<html>`
  - `</html>` 
- **HEAD** - this element is where metadata about the page is stored, this metadata can help browsers render our pages correctly
  - `<head>`
  - `</head>` 
  - **TITLE** - this element is nested within the **HEAD** element and gives each page a **human readable** title
    - `<title>{Title of Page}</title>` 
  - **CHARSET** - The meta tag describing the content encoding of the page; this ensures all characters and symbols display correctly
    - `<meta charset="utf-8" />`  
- **BODY** - The final element needed to create the HTML boilerplate. All the page's visible content is stored here we have all kinds of things here including **text**, **images**, **lists**, **links**, etc...
- We can see the full HTML boilerplate below
```
<HTML>
  <HEAD>
    <TITLE>Site Title</TITLE>
    <META charset="UTF-8" />
    <BODY>
    </BODY>
  </HEAD>
</HTML>
```
- VS Code allows us to use a simple shortcut for developing boilerplate we can just type `!` on the first line
### Assignments
- [x] Watch and follow along Kevin Powell's [Building Your First Web Page video](https://www.youtube.com/watch?v=V8UAEoOvqFg&list=PL4-IK0AVhVjM0xE0K2uZRvsM7LkIhsPT-&index=2)
- [x] Delete the contents of index.html and write the boilerplate from memory several times
- [x] Check boilerplate within an [HTML Validator](https://validator.w3.org/)
### Additional Resources
- [charsets we should use with HTML pages](https://www.bitdegree.org/learn/html-encoding)
## Working with Text
- Most data on the web is `text based` so it is important to know how to work with text
- There are several important text type **elements** we need to learn to work with:
  - **paragraphs**
    - `<p>`
    - `</p>` 
  - **headings**
    - `<h1>` **through** `<h6>`
    - `</h1>` **through** `</h6>`
    - **NOTE** - Using the correct heading level is important to ensure proper hiearchy 
  - **bold text**
    - `<strong>`
    - `</strong>` 
  - **italicized text**
    - `<em>`
    - `</em>` 
- **Nesting** and **Indentation** are important in HTML. When we place one element inside another we call it **nesting** this creates a **parent**:**child** relationship
- **COMMENTS** - Comments are not visible to the browser 
  - `<!-- {comment text} -->`
### Assignment
- [x] Watch Kevin Powell's [HTML Paragraph and Headings Video](https://www.youtube.com/watch?v=yqcd-XkxZNM&list=PL4-IK0AVhVjM0xE0K2uZRvsM7LkIhsPT-&index=3)
- [x] Watch Kevin Powell's [HTML Bold and Italic Text Video](https://www.youtube.com/watch?v=gW6cBZLUk6M&list=PL4-IK0AVhVjM0xE0K2uZRvsM7LkIhsPT-&index=4)
- [x] Create a sample blog article with multiple headings, maybe use the [Lorem Ipsum Generator](https://loremipsum.io/)
## Lists
- Lists are everywhere on the web, HTML makes lists easy
- **unordered lists** - are used when the ordering of list items don't matter, think a bulleted list
```
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```
- **ordered lists** - are used when the ordering is important think numbered lists
```
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>
```
### Assignment
- [ ] Create an **unordered** shopping list of your FAVORITE FOODS
- [ ] Create an **ordered** list of TODAY'S TO-DO Items
- [ ] Create an **unordered** list of PLACES you'd like to visit
- [ ] Create an **ordered** list of top 5 favorite video games/movies/books/etc...
### Additional Resources
- [Microsoft Developer Network - Unordered List](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul)
- [Microsoft Developer Network - Ordered List](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol)
- [Shay Howe's HTML lists tutorial](https://learn.shayhowe.com/html-css/creating-lists/)
## Links and Images
- Links and images are both super important for the web
- **anchor elements**
  - `<a>`
  - `</a>` 
  - Without additional context this doesn't do anything, we need attributes an **attribute** is made up of a **name** and a **value**
  - `<a href="https://www.theodinproject.com/about">Click me</a>` - will link us to the Odin Project with the text `Click me`
  - **href** is an attribute that accepts a URL as a value
- **ABSOLUTE** vs **RELATIVE** links
  - **absolute** links link to other pages or sites on the internet and look like; **absolute** links always contain the protocol and domain of the destination
    - `protocol://domain/path`
  - **relative** links link to pages and resources within our own site's structure; they do not contain the domain name, they assume the domain name are the same
- **Images** allow us to display more than just text we can use the image tag to do this with images
  - `<img/>`
  -  Just like the **anchor** tag, to be useful we need to use an **attribute** with the Image tag
    - `<img src="{URL}">`
    - there is also an **alt** attribute which we should always strive to use it describes an image, if the image can't be loaded this will be shown it will also allow assisitve technologies to read what the image is showing
### Assignment
- [ ] Watch Kevin Powell's [HTML Link's Video](https://www.youtube.com/watch?v=tsEQgGjSmkM&list=PL4-IK0AVhVjM0xE0K2uZRvsM7LkIhsPT-&index=5)
- [ ] Watch Kevin Powell's [HTML Images Video](https://www.youtube.com/watch?v=0xoztJCHpbQ&list=PL4-IK0AVhVjM0xE0K2uZRvsM7LkIhsPT-&index=6)
- [ ] Watch Kevin Powell's [File Structure Video](https://www.youtube.com/watch?v=ta3Oxx7Yqbo&list=PL4-IK0AVhVjM0xE0K2uZRvsM7LkIhsPT-&index=7)
- [ ] Read about the [four main image formats](https://www.internetingishard.com/html-and-css/links-and-images/#image-formats) that can be used on the web
## [Project - Recipes]()
- We want to build a classic recipe website which will have several pages:
- [ ] A main **index** page - with links to several recipes
- [ ] several **recipe** pages
- We will walk this project out in at least 4 iterations
  1. Iteration 1: Initial Structure
  2. Iteration 2: Recipe Page
  3. Iteration 3: Recipe Page Content
  4. Iteration 4: Add More Recipies 
