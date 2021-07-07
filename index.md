
<!---
## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/PisanA/checkstyle-webpage/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.
--->

# Checkstyle

![image](https://user-images.githubusercontent.com/54456351/119812559-1ec06400-be9d-11eb-907d-e1b71a97a447.png) <br>
![image](https://user-images.githubusercontent.com/54456351/119814435-3f89b900-be9f-11eb-8578-2272566be21c.png) <br>

Checkstyle is a tool for checking Java source code for adherence to the Google Java Style Guide.<br>
Click "checkstyle" to view the report. The report should look like this:
![image](https://user-images.githubusercontent.com/54456351/120709943-5ec1b100-c472-11eb-93a1-1aafa7de830a.png) <br>
<br /> <br /> <br />
You can access each code line violating the coding standard through "Findings(37)"
![image](https://user-images.githubusercontent.com/54456351/120710983-b01e7000-c473-11eb-873d-e57b75aeab5c.png) <br>

The following is some comments you might find in the report:
## 'method def modifier' has incorrect indentation level 4, expected level should be 2.
Google style uses an indentation of 2 spaces, but most IDEs use 4 spaced indentation. Therefore, if you want to use 4 spaced indentation, you can ignore this comment. 
<br><br>

## Line is longer than 100 characters (found 109).
A normal computer screen cannot show more than 100 characters horizontally. The long line should be broken into shorter lines to ensure readability. 
<br><br>

## '{' at column 5 should be on the previous line.
'{' should not be in a new line. For example,  <br>
```
if (condition) {  
    statement; 
} 
```
<br><br>

## 'if' construct must use '{}'s.
Even when you only have 1 statement in your constructor, you should uses '{}' 
<br><br>

## Only one statement per line allowed.
Code should only have 1 statement per line for readability.
<br><br>

## WhitespaceAround: '=' is not preceded with whitespace **and** WhitespaceAround: '=' is not followed by whitespace. Empty blocks may only be represented as {} when not part of a multi-block statement (4.1.3).
There should be a space before and after `+`, `-`, `*`, `/`, `=`, `<`, `>`, ... <br>
`;` should be followed by a space if there is anything after it
<br><br>

## '(' is preceded with whitespace.
Some '(' should not have whitespace(s) before it. For example, `Scanner scan = new Scanner (System.in);` violates the rules because there is a space before '('. The correct format is `Scanner scan = new Scanner(System.in);`
<br><br>

## '(' is followed by whitespace.
Similar with the above warning, some '(' should not have whitespace(s) after it. For example, `System.out.println( "Hello World");` violates the rules because there is a space after '('. The correct format is `System.out.println("Hello World");`

## '}' at column 9 should be on the same line as the next part of a multi-block statement (one that directly contains multiple blocks: if/else-if/else, do/while or try/catch/finally).
If you have multiple if-else statements. The next one should be on the same line with the previous ending bracket '}' <br>
The following is the correct format:
```
if (condition) {  
    statement; 
} else if (condition2) {  
    statement2; 
} else { 
    statement3; 
}
```
<br><br>

## Line contains a tab character.
This mean your code line contains a tab character. <br>
Using the tab key inserts an actual invisible tab character into your text, which can mess up the formatting later when your publisher tries to reformat your document for publication. <br>
Different IDEs have different size of tab. Tab character is commonly 2 or 4 spaces in most IDEs. The differences can cause inconsistent code style while copying and pasting code. Therefore, programmers should use spaces instead of tab charater. 
<br><br>

## Using the '.*' form of import should be avoided - java.util.*.
The library is divided into packages and classes. Meaning you can either import a single class (along with its methods and attributes), or a whole package that contain all the classes that belong to the specified package. <br>
You should import specific classes that are used in the program instead of import the whole package <br>
If you use Scanner in your code, you should import `java.util.Scanner` instead of `java.util.*`
<br><br>

## Wrong lexicographical order for 'org.junit.Assert' import. Should be before 'org.junit.contrib.java.lang.system.TextFromStandardInputStream'.
The import should  be in lexicographical order
<br><br>

## Extra separation in import group before 'java.io.*'
There should be no separation (new lines) within the import section.
<br><br>
<!---

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/PisanA/checkstyle-webpage/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
--->
