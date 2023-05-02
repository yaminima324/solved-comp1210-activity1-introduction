Download Link: https://assignmentchef.com/product/solved-comp1210-activity1-introduction
<br>
<table width="613">

 <tbody>

  <tr>

   <td width="180"><strong>Terminology  </strong></td>

   <td width="163"><strong> </strong></td>

   <td width="106"> </td>

   <td width="164"> </td>

  </tr>

  <tr>

   <td width="180">Object-oriented programmingJava API (class library)DocumentationCommentsClassMethod</td>

   <td width="163">IdentifiersReserved wordsWhite spaceMachine languageAssembly languageHigh-level languageEditor</td>

   <td width="106">CompilerInterpreterSource codeJava bytecodeIDEDebuggerSDK / JDK</td>

   <td width="164">SyntaxSemanticsCompile-time errorRun-time errorLogic error</td>

  </tr>

 </tbody>

</table>




<h1>Comments in Java</h1>

Java has three types of comments: single line (//), multiple line (/*  */), and Javadoc (/**   */).

// single line comment – goes through the end of the line




/* multiple line comment – begins on this line but may end on another line; ends with */

/** Javadoc comment – begins on this line but may end on another line; ends with */




<h1>Course Coding Standard</h1>

A <strong>coding standard</strong> consists of guidelines that are used by developers when writing source code to ensure a consistent format.  The course coding standard is supported by Checkstyle, which is an automated tool that works with the jGRASP IDE and the Web-CAT program grading system to automatically detect style errors based on the rules or checks adopted for the course.  The first two rules are introduced below. •           For <u>activity</u> and <u>project</u> assignments, all pubic classes and public methods require Javadoc comments.  In the HelloWorldCommented program below, the text in <em>italics</em> describes the information that goes on the line.  The information shown should be replaced by your own information.

/**

<ul>

 <li>Simple program to print Hello World. <em>Description of your program goes here</em>.</li>

</ul>

*

<ul>

 <li>Activity 1 <em>(your activity or project number goes here)</em>.</li>

 <li>@author <em>your name</em> – <em>course </em>–<em> section as appropriate</em></li>

 <li>@version <em>date</em></li>

</ul>

*/

public class HelloWorldCommented {

/**

<ul>

 <li>Prints Hello World one time. <em>Usually shorter description here.</em></li>

 <li>@param args Command line arguments – not used.</li>

</ul>

*/

public static void main(String[] args) {

System.out.println(“Hello World”);

} }

<ul>

 <li>Lines of code must not exceed 80 characters (including indentation). You can continue string literals on a new line by using string concatenation which creates a string from two or more other strings).</li>

</ul>

For example<strong>: </strong>

System.out.println(“Suppose this is a long output string.”);

Can be rewritten as:

System.out.println(“Suppose this is a long ”

+ “output string.”);

The output of these two statements is the same; i.e., the concatenation does not change the output.

<strong>        </strong>

<strong>Page 1 of 6</strong>




<h1>Goals</h1>

By the end of this activity you should be able to do the following:

<ul>

 <li>Create a program then compile and run it</li>

 <li>Add Javadoc comments to your program</li>

 <li>Generate documentation for your program</li>

 <li>Correct your source code structure using Checkstyle</li>

 <li>Submit your completed program to Web-CAT for grading</li>

</ul>

<h1>Directions</h1>

<h2>               Part A: Using jGRASP and Checkstyle</h2>

<ul>

 <li><strong>Set up file folder</strong> – Open a file browser on your computer (e.g., File Browser on Windows or Finder on MacOS), and set up an appropriately named file folder for this activity (e.g., Activity_01).</li>

 <li><strong>Open jGRASP</strong> – e.g, On Windows, click the <strong>Start</strong> button in the lower left corner of the screen, then in the Search window, enter <strong>jgrasp</strong> then when <strong>jGRASP</strong> On MacOS, enter Cmd-space, enter <strong>jgrasp</strong>, then double-click on it.</li>

 <li>Using the top menu in jGRASP, open a new Java window (<strong>File &gt; New &gt; Java</strong>). Enter the following Java statements to create a class called StudentInfo:</li>

</ul>

<strong>public</strong> <strong>class</strong> StudentInfo

{




}

<strong>         </strong>

<ul>

 <li>Click the Save  button on the top menu, then in the Save As dialog, use the buttons to the far right of “Look In” near the top of the dialog to navigate up           to the folder where you</li>

</ul>

want to save your program. If you have not yet created a course folder (and within it a folder for this activity) you can do that now by clicking the folder  button to create a new folder.  Click once on the name “New folder” to select it then click on it again and change the name to number of this course.  Double-click the folder to open it, then (as above) create a folder for this activity and open it.  If your program code is correct, you should see StudentInfo.java as the file name.  If this is not the case, enter the file name manually.  Now click the Save button at the bottom of the dialog.

<ul>

 <li>Click the Compile button , and fix any compile-time errors.</li>

 <li>Generate your CSD by either pressing F2 or by clicking the Generate CSD button on the toolbar at the top of the jGRASP desktop.  <u>Now turn on Auto Generate CSD (<strong>View &gt;</strong> then</u> <u>check the <strong>Auto Generate CSD</strong> box), so that the CSD will be generated each time you Load</u> <u>or Compile a file</u>. You may turn this off/on at any time.</li>

 <li>Add a main method to the class. Be sure to replace the blank in the code below with the method name (don’t forget to re-generate the CSD):</li>

</ul>

<strong>2</strong>




<ul>

 <li></li>

 <li>Now add the Javadoc comments for <u>the class </u>and <u>the main method</u> of this program by adapting the Javadoc comments on page 1 so that they describe this program and have your name, course info, and today’s date.</li>

 <li>Inside the main method, write three or more print statements: (1) the first prints Name: followed by your name (first and last) on the first line, (2) the second that prints Previous Computer Courses: on the second line, (3) the third <u>prints three spaces</u> followed by the name of a computer course you have had (or None if this is your first course), (4) if you have had more than one computer course, print an additional line for each course (be sure to begin each course line with three spaces). Don’t forget to put double quotes around the String literals in the println statements.</li>

 <li>Click the Run Checkstyle button on the jGRASP toolbar and correct any issues identified by Checkstyle.  <em>If you don’t see the Checkstyle button then Checkstyle has likely not been installed on your machine. On your personal computer, you will need to download and install (unzip) Checkstyle.  You may also need to configure Checkstyle in jGRASP (<strong>Tools &gt; Checkstyle &gt; Configure</strong>) so that jGRASP can find the folder containing the Checkstyle JAR file.</em></li>

 <li>Toggle line numbers on/off by clicking on the toolbar.  Most users leave line numbers on.</li>

 <li>Click the Browse button on the toolbar.  This opens the jGRASP Browse tab on the folder that contains the file in the CSD window.  You should see StudentInfo.java underlined in the Browse tab. You should also see the corresponding .class file (StudentInfo.class) that was generated by the compiler if your file compiled successfully. <u>This file contains the bytecode</u> <u>for your program that is used to run your program when you click the Run button </u>.</li>

</ul>




<strong>In Part B you will develop a second program CourseInfo.java and then submit both StudentInfo.java and CourseInfo.java at the same time to Web-CAT.   </strong>

<strong>3</strong>

<strong>Part B: Using Checkstyle, Web-CAT, and jGRASP Projects</strong>

<strong> </strong>

<h2>1. Using Checkstyle to Find and Correct Style Errors</h2>

<ul>

 <li>Download the Part B zip file and <u>save it in your folder for this activity</u>. Then extract the CourseInfo.java file (Windows: right-click on the zip file then select <strong>Extract All …</strong>; Mac OS X: just open the zip file).</li>

 <li>Open CourseInfo.java by double-clicking on the file in the Browse tab. You will be responsible for correcting style errors and logic errors that are present in the program. The first step is to modify the program to adhere to the course coding standard. To do this, run Checkstyle and correct all of the formatting issues that appear.

  <ul>

   <li>HINT: Checkstyle states that the main method is missing a Javadoc comment, and this is true. Hint: Make sure that you know the difference between a <strong>// </strong><em>to end of line comment</em>, a <strong>/*</strong> <em>single or multiple line comment</em> <strong>*/</strong>, and a <strong>/**</strong> Javadoc comment <strong>*/</strong>.</li>

   <li>HINT: For dealing with a source line over 80 characters, see page 1 of this activity.</li>

  </ul></li>

 <li>The program’s <strong>expected output</strong> is shown below (<u>the line numbers on the left are <strong>not</strong> part of</u> <u>the expected output</u>):</li>

</ul>




<table width="619">

 <tbody>

  <tr>

   <td width="24">1 23 45</td>

   <td width="595">This course provides an introduction to Java and  object-oriented programming. The course also introduces the basics of software development.</td>

  </tr>

 </tbody>

</table>




The original author of the program claims the program is correct because it “gets the point across,” but you know that it is incorrect because the <strong>actual output</strong> of the program does not match the <strong>expected output</strong> above when you run it during testing. Correct the output errors by modifying the program.   <em>Hint: Look for issues in formatting/spacing, spelling, capitalization, etc. One way to skip a line is print an empty line with the statement: </em><em> </em>

System.out.println();

<strong> </strong>

<h2>2. Using Web-CAT to Grade Your Program</h2>

In jGRASP, navigate to <strong>Tools &gt; Web-Cat &gt; Configure</strong>. In the Web-CAT Tool Settings dialog, delete the current entry (if any) for Assignment Definition URL.  <u>Select</u> (rather than click) the URL below, right-click and select <strong>Copy</strong>, and then, right click and select <strong>Paste</strong>. Finally, click OK. You should now have a Web-CAT button  on the toolbar.  (See the WebCAT documentation on the class website for more information.)




<strong>https://webcat.eng.auburn.edu:8443/Web-CAT/WebObjects/Web-CAT.woa/wa/assignments/eclipse   </strong>




<strong>4</strong>

<ul>

 <li>Open the Java file that you want to submit then you can submit your program via Web-CAT.</li>

</ul>

Click the Web-CAT toolbar button  (or go to <strong>Tools &gt; Web-Cat &gt; Submit File</strong>), and the Web-CAT submission dialog will open with a list of courses and assignments open for submission.  If multiple courses are listed, be sure to select the one in which you are enrolled; otherwise, your submission will fail. For example, in the figure below the COMP 1210 course folder is shown opened with the assignment labeled <strong>Activity 01.  </strong>Click<strong> Activity 01 </strong>to select it, click <strong>Next</strong>; click <strong>Add</strong> to add the other file for this activity so that both CourseInfo.java and StudentInfo.java are listed.  Then click <strong>Next</strong>, login to Web-CAT, and click <strong>Submit</strong>.  A web page should open indicating your Web-CAT submission is being processed and usually within a few seconds you should see your results.







<strong> </strong>

<ul>

 <li>You should try for the maximum number of points in Web-CAT for Style/Coding + Correctness/Testing (TA points will be assigned latter).  You will have 10 tries so if you make changes/corrections, be sure that your files compile/run as expected in jGRASP and that they pass the Checkstyle audit <u>before</u> you submit your files again to Web-CAT.</li>

</ul>




<ul>

 <li>Remember, in order to submit the two or more files, you can press the Web-CAT button on one file and then add the other files prior to submission (as described above) OR you can create a jGRASP project (see below).</li>

</ul>




<h2>3. Creating a jGRASP Project and submitting to Web-CAT   (recommended when submitting multiple files)</h2>




You can create a jGRASP project, add both Java files to the project, and then submit the project to Web-CAT.  This will simplify the submission process and save time, especially as the number of files in assignments increases.




<ul>

 <li>To create a project in jGRASP, go to <strong>Project &gt; New</strong> and make sure that you are in the same directory as your source code files. For <em>Project Name</em>, enter a project name (e.g., <strong>Activity_01</strong>) and click <strong>Next</strong>. Click <strong>Next</strong> again to create the project.</li>

</ul>




<ul>

 <li>Now in the lower part of the Browse tab you should see an <strong>Open Projects</strong> Rightclick the project name and select <strong>Add Files</strong>. Add your java files to the project.</li>

</ul>




<strong>5</strong>







<ul>

 <li>Once all files are added, click the Web-CAT symbol <u>on the <strong>Open Projects</strong> tab</u>.</li>

</ul>




<ul>

 <li>Select the <strong>Activity 01</strong> assignment, click <strong>Next</strong>, make sure that all files in the are included, click <strong>Next</strong>, login to Web-CAT (if not already logged in), and click <strong>Submit</strong>.</li>

</ul>







<ul>

 <li>Automatically <strong>generate project documentation</strong> in the form of linked web pages from your</li>

</ul>

Javadoc comments. As a last exercise for this activity, find the Open Projects toolbar in

Browse tab click the Show/generate project documentation button .  A web page should open showing your project documentation.  Most software organizations require Javadoc (or similar) comments in all programs to support the automatic generation of documentation from the programs, where each program may range from a few files to thousands of files.




<ul>

 <li>In the future, you should always begin each activity or project by creating a separate folder for it. After you have created one or more .java files and saved them to the folder, you should create a jGRASP project and add the .java files. In addition to saving time when you submit to Web-CAT, using jGRASP projects has a number of other advantages that we will explore as the course progresses.</li>

</ul>