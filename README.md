# How to Work with Markdown for Technical Writers Using VS Code
- [Markdown](#markdown)
- [Understanding Docs-as-Code and DITA](#understanding-docs-as-code-and-dita)
  - [1. Introduction](#1-introduction)
  - [2. Docs-as-Code Overview](#2-docs-as-code-overview)
    - [Key Features:](#key-features)
    - [List number](#list-number)
  - [Table](#table)
  - [Code](#code)
    - [Hyperlinks](#hyperlinks)
    - [Image](#image)
  - [HTML Code](#html-code)

# User Manual: How to Work with Markdown for Technical Writers Using VS Code
## 1. Introduction
Markdown is a lightweight markup language used widely for creating formatted text using plain text editors. VS Code (Visual Studio Code) is a free, powerful code editor that offers excellent Markdown support. This guide walks technical writers through setting up and writing in Markdown using VS Code.

## 2.What is Markdown?

Markdown allows you to format text using simple syntax. It's commonly used for README files, documentation, and blogging. Files use the `.md` extension..

##  3. Installing VS Code

- Visit https://code.visualstudio.com

- Download the appropriate version for your OS

- Install and launch VS Code

## 4. Setting Up Markdown in VS Code

Open VS Code

- Install the Markdown All in One extension:

- Go to Extensions tab (or press `Ctrl+Shift+X`)

- Search "Markdown All in One"

- Click Install

Optional:

- Install Markdown Preview Enhanced for better export options

## 5. Creating a Markdown File

- Open VS Code

- Click File > New File

- Save it as `filename.md`

- Start typing Markdown content

## 6. Basic Markdown Syntax

Here are some commonly used Markdown elements:
```
# Heading 1
## Heading 2
### Heading 3

**Bold text**  
*Italic text*  

- Bullet list item
1. Numbered list item

[Link text](https://example.com)  
`Inline code`  

```javascript
// Code block
console.log("Hello World");
```
Blockquote
```

---

### 7. Writing Technical Documentation in Markdown
Use Markdown to structure content logically:
- Use headings (`#`) to define sections
- Bullet lists for features or steps
- Code blocks for commands or programming examples
- Tables for data

Example table:
```markdown
| Feature | Description |
|---------|-------------|
| Bold    | `**text**`  |
| List    | `- item`    |
```
## 8. Using Extensions for Markdown in VS Code

Recommended extensions:

- **Markdown All in One:** Autocomplete, shortcuts, table of contents

- **Markdown Preview Enhanced:** Advanced preview and export

- **Prettier:** Code formatting for consistency

## 9. Previewing Markdown Files

- Click **Open Preview** icon in the top right

- Or press `Ctrl+Shift+V`

- Split screen view available with Ctrl+K V

## 10. Exporting Markdown to PDF or HTML

Use ****Markdown Preview** Enhanced:

- Open Markdown file

- Click the export icon (top right of preview window)

- Choose ****PDF, HTML**, or **PNG**

Or use VS Code CLI with Pandoc (advanced users)








### Key Features:
* list 1
* list 2
    * n
    *   * 
* List 3
* list 4
* 
-  Uses Git-based workflows for version control
- Supports automation through CI/CD pipelines
- Often relies on Markdown or reStructuredText for authoring
### List number
1. b

2. b
3. bnb
4. nnnm

## Table
Name | Category | Profession
---- | ----| ---- |
Maddy | _C01_ | TW |
Julia | _Co5_ | TW1 |

## Code
```
{

    "status":"OK",

    "data":

        {

            "message": "Welcome, world!"


        }

}
```
### Hyperlinks
[TWT](https://techwriterstribe.com/dita-reg-form/)

Cross-reference
<!— Do not show this line. —>

### Image
![Image](https://www.palaiszelda.com/images/z15/st_link_et_spectre.jpg)

## HTML Code
```
<table class="table table-striped">
<caption>Caption for this Table</caption>
<thead class="thead-dark">
<tr>
    <th width="30%">Property</th>
    <th width="70%">Description</th>
    </tr>
</thead>
<tbody>
<tr>
    <td>Topic1 </td>
    <td>Topic2
        <ul>
        <li>Bullet item</li>
        <li>Bullet item</li>
        </ul>
        </td>
    </tr>
<tr>
    <td>TopicA</td>
    <td>TopicB</td>
    </tr>
</tbody>
</table>
 
```

![](/Images/Screenshot.png)



