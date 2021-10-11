
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

## The name of the outer type and the file do not match. (com.puppycrawl.tools.checkstyle.checks.OuterTypeFilenameCheck)
This is a compilation error where filename is different from class name. Your class name must always be the same with the filename. If you class name is `Main`, then the filename must be `Main.java`.

## Missing a Javadoc comment.
There is a special format for Javadoc if you want to put comments above a method. <br>
![image](https://user-images.githubusercontent.com/54456351/128497623-32d5bd4a-681d-4c2d-b339-9187facc98ac.png)
<br><br>

## Javadoc comment is placed in the wrong location.
Class level Javadoc should be after the `import` section and before `class`. <br>
Example of bad Javadoc:<br>
![image](https://user-images.githubusercontent.com/54456351/128498412-12dc1cf7-b9d8-4fa3-ae53-708abd7adea4.png) <br><br>
Example of good Javadoc:<br>
![image](https://user-images.githubusercontent.com/54456351/128498495-5c85c6ae-bb48-4272-b2c0-63eb3e5ae096.png)
<br><br>

## 'CLASS_DEF' should be separated from previous statement.
## 'METHOD_DEF' should be separated from previous line.
There should be some space between classes and methods for readability. <br>
![image](https://user-images.githubusercontent.com/54456351/136776497-b33c2f15-8698-487a-931b-77b899ae6d6e.png)


## 'method def modifier' has incorrect indentation level 4, expected level should be 2.
Checkstyle uses an indentation of 2 spaces, but most IDEs use 4 spaced indentation. Therefore, if you want to use 4 spaced indentation, you can ignore this comment. 
<br><br>

## Line contains a tab character.
This mean your code line contains a tab character. <br>
Using the tab key inserts an actual invisible tab character into your text, which can mess up the formatting later when your publisher tries to reformat your document for publication. <br>
Different IDEs have different size of tab. Tab character is commonly 2 or 4 spaces in most IDEs. The differences can cause inconsistent code style while copying and pasting code. Therefore, programmers should use spaces instead of tab charater. 
<br><br>

## Line is longer than 100 characters (found 109).
A normal computer screen cannot show more than 100 characters horizontally, preferably under 80 character. The long line should be broken into shorter lines to ensure readability. <br>
![image](https://user-images.githubusercontent.com/54456351/126028286-b6396342-31e5-40b2-9de9-567957605454.png)
<br><br>

## Local variable name 'Codingstyle' must match pattern '^\[a-z]([a-z0-9]\[a-zA-Z0-9]\*)?$'
The first letter of variable name should be in lowercase, and each new word start with a uppercase letter. <br>
![image](https://user-images.githubusercontent.com/54456351/126029123-0fe28fec-7d9e-4be6-b330-108c96081393.png)
<br><br>

## Abbreviation in name 'SML' must contain no more than '2' consecutive capital letters.
The variable name rule is the first letter should be in lowercase, and each new word start with a uppercase letter. Therefore, each uppercase letter will be counted as a word. 3 consecutive capital letters mean 3 words next to each other. The name is too short and and undescriptive. <br>
![image](https://user-images.githubusercontent.com/54456351/126029355-ab461cb7-5c27-4c37-985f-da31d3d224bf.png)
<br><br>

## Method name 'ToString' must match pattern '^[a-z][a-z0-9][a-zA-Z0-9_]*$'.
The first letter of method name should be in lowercase, and each new word start with a uppercase letter. <br>
![image](https://user-images.githubusercontent.com/54456351/126029492-b885881d-6341-46e2-981b-1fa5fb0a7c81.png)
<br><br>

## Only one statement per line allowed.
Code should only have 1 statement per line for readability. <br>
![image](https://user-images.githubusercontent.com/54456351/126028246-9a27aabf-7a2f-48ea-80c1-23a2cde3e735.png)
<br><br>

## 'if' construct must use '{}'s.
Even when you only have 1 statement in your constructor, you should uses '{}'. For example: <br>
![image](https://user-images.githubusercontent.com/54456351/126028318-99d0c385-7a7c-410f-944c-beec18a816b2.png)
<br><br>

## '{' at column 5 should be on the previous line.
CheckStyle follows K&R style that `{` is in the same line with the control statement (if, while, for...). If you want to use Allman or other styles, you can ignore this warning.<br>
![image](https://user-images.githubusercontent.com/54456351/126028275-0b9359a6-0368-4d82-a836-04fcf6ec563f.png)
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

## Array brackets at illegal position.
Brackets should be put right after the declaration type, not the name. <br>
![image](https://user-images.githubusercontent.com/54456351/128547554-4419c779-9116-49c9-899b-825b06e47dbb.png)
<br><br>

## Distance between variable 'size' declaration and its first usage is 5, but allowed 3. Consider making that variable final if you still need to store its value in advance (before method calls that might have side effects on the original value).
`size` and `5` can be different based on developer's code. 
When a variable is initilized, you should use it within the next 3 code lines. It helps to group related codes together and make them easier to read. <br> 
![image](https://user-images.githubusercontent.com/54456351/136779105-c1bb1a3c-7b00-4f9a-93b3-a46a0f3f81ff.png)

## New Warnings
If you don't see your warnings on the website, please fill this survey so that we can add them: <a href="https://docs.google.com/forms/d/e/1FAIpQLSf1M4lW8zU0gfX2b0JHl3O0-vluhYhtCcvS2Ox0z3LDCwWEHg/viewform">New CheckStyle Warning</a> <br>

#### For more information, view <a href="https://checkstyle.sourceforge.io/styleguides/google-java-style-20180523/javaguide.html">Google Java Style Guide</a> 


<!-- link to checkstyle word files: https://docs.google.com/document/d/1L7H60XW0bg_6tAjo4Lsm5I8Qmf-xCnGnXz3iHFH2jV0/edit-->
