
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
You can access each code line violating the coding standard through "Findings(6)"
![image](https://user-images.githubusercontent.com/54456351/126027336-b869520f-6061-48b3-937d-2ceb9c95baf9.png)
<br>

The following is some comments you might find in the report:
## 'method def modifier' has incorrect indentation level 4, expected level should be 2.
Checkstyle uses an indentation of 2 spaces, but most IDEs use 4 spaced indentation. Therefore, if you want to use 4 spaced indentation, you can ignore this comment. 
<br><br>

## Line is longer than 100 characters (found 109).
A normal computer screen cannot show more than 100 characters horizontally. The long line should be broken into shorter lines to ensure readability. <br>
![image](https://user-images.githubusercontent.com/54456351/126028286-b6396342-31e5-40b2-9de9-567957605454.png)
<br><br>

## '{' at column 5 should be on the previous line.
CheckStyle follows K&R style that `{` is in the same line with the control statement (if, while, for...). If you want to use Allman or other styles, you can ignore this warning.<br>
![image](https://user-images.githubusercontent.com/54456351/126028275-0b9359a6-0368-4d82-a836-04fcf6ec563f.png)
<br><br>

## 'if' construct must use '{}'s.
Even when you only have 1 statement in your constructor, you should uses '{}'. For example: <br>
![image](https://user-images.githubusercontent.com/54456351/126028318-99d0c385-7a7c-410f-944c-beec18a816b2.png)
<br><br>

## Only one statement per line allowed.
Code should only have 1 statement per line for readability. <br>
![image](https://user-images.githubusercontent.com/54456351/126028246-9a27aabf-7a2f-48ea-80c1-23a2cde3e735.png)
<br><br>

## WhitespaceAround: '=' is not preceded with whitespace **and** WhitespaceAround: '=' is not followed by whitespace. Empty blocks may only be represented as {} when not part of a multi-block statement (4.1.3).
There should be a space before and after all operators (`+`, `-`, `*`, `/`, `=`, `<`, `>`,  `&&`, `||`, `!=`, `>=`, `<=`, `==`). <br>
`;` should be followed by a space if there is anything after it <br>
![image](https://user-images.githubusercontent.com/54456351/126028552-f7155f96-9494-438a-95f2-64a76b2fe93c.png)
<br><br>

## '(' is preceded with whitespace.
There should be no spaces before the parentheses in a method call or a constructor creation. <br>
![image](https://user-images.githubusercontent.com/54456351/126028488-7bf86f74-ffb4-419f-b8dd-7ff7107c6004.png)
<br><br>

## '(' is followed by whitespace.
There should be no spaces after `(` and before `)`.  <br>
![image](https://user-images.githubusercontent.com/54456351/126028564-1a793175-a37e-4192-84c2-7d52a942b373.png)
<br><br>

## '}' at column 9 should be on the same line as the next part of a multi-block statement (one that directly contains multiple blocks: if/else-if/else, do/while or try/catch/finally).
CheckStyle follows K&R style that if you have multiple if-else statements, the next one should be on the same line with the previous ending bracket '}' 
If you want to use Horstmann or other styles, you can ignore this warning.<br>
![image](https://user-images.githubusercontent.com/54456351/126028730-2bc9e484-6702-4ac9-97dd-5bc7a20dc562.png)
<br><br>

## Line contains a tab character.
This mean your code line contains a tab character. <br>
Using the tab key inserts an actual invisible tab character into your text, which can mess up the formatting later when your publisher tries to reformat your document for publication. <br>
Different IDEs have different size of tab. Tab character is commonly 2 or 4 spaces in most IDEs. The differences can cause inconsistent code style while copying and pasting code. Therefore, programmers should use spaces instead of tab charater. 
<br><br>

## Using the '.*' form of import should be avoided - java.util. \* .
The library is divided into packages and classes. Meaning you can either import a single class (along with its methods and attributes), or a whole package that contain all the classes that belong to the specified package. <br>
You should import specific classes that are used in the program instead of import the whole package <br>
![image](https://user-images.githubusercontent.com/54456351/126028774-d9834472-38af-4ef2-b176-c22a8f95b8dc.png)
<br><br>

## Wrong lexicographical order for 'java.util.Array' import. Should be before 'java.util.Scanner'.
The import should  be in lexicographical order (alphabetical order A-Z). For example, `io` shoud be before `util` and `Array` should be before `Scanner`. The following is an example of import section in correct lexicographical order. <br>
![image](https://user-images.githubusercontent.com/54456351/126028878-d46bcefa-38d7-48b9-a83a-1f69e6e25dd2.png)
<br><br>

## Extra separation in import group before 'java.util.Array'
There should be no separation (new lines) within the import section.
![image](https://user-images.githubusercontent.com/54456351/126028962-7b03a77a-fad8-4f13-a9b4-39974b8b7806.png)
<br><br>

## Local variable name 'Num' must match pattern '^[a-z]([a-z0-9][a-zA-Z0-9]*)?$'
<br><br>

## Abbreviation in name 'NUM' must contain no more than '2' consecutive capital letters.
<br><br>
