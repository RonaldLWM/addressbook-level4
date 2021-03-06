# User Guide

* [Getting Started](#getting-started)
* [Features](#features)
* [FAQ](#faq)
* [Command Summary](#command-summary)

## Getting Started

1. Ensure you have Java version `1.8.0_60` or later installed in your Computer.<br>
   > Having any Java 8 version is not enough. <br>
   This app will not work with earlier versions of Java 8.
   
2. Download the latest `simply.jar` from the [releases](../../../releases) tab.
3. Copy the file to the folder you want to use as the home folder for your Simply.
4. Double-click the file to start the app. The GUI should appear in a few seconds. 
  
 <img src="images/StartUp.PNG" width="600"><br>

5. Type the command in the command box and press <kbd>Enter</kbd> to execute it. <br>
   e.g. typing **`help`** and pressing <kbd>Enter</kbd> will open the help window. 

6. Refer to the [Features](#features) section below for details of each command.<br>


## Features

###4.1 Add Command
There are three variations to the add command. You are able to choose a task to be categorized under events, deadlines or to-dos. To differentiate the formatting for these commands, refer to the section below.

####4.1.1 Add an event
Format : **Add** [&lt;event description&gt;, &lt;date(DDMMYY)&gt;, &lt;start time&gt;, &lt;end time&gt;]

<img src="images/Capture2.PNG" width="600"><br>

Example: Add [Siloso beach event, 121216, 1600, 2200]

<img src="images/Capture 3.PNG" width="600"><br>

>Note: The start time and end time is optional when adding an event. 
Important: The square brackets are compulsory when adding an event.

####4.1.2 Add a deadline
Format: **Add** &lt;deadline description&gt;, &lt;date(DDMMYY)&gt;, &lt;end time&gt;

<img src="images/Capture4.PNG" width="600"><br>

Example: Add complete report, 120916, 1900

<img src="images/Capture5.PNG" width="600"><br>

>Important: The date and end time are compulsory when adding an deadline

####4.1.3 Add a todo
Format: **Add** &lt;todo descrption&gt;

<img src="images/Capture6.PNG" width="600"><br>

Example: Add go swimming

<img src="images/Capture7.PNG" width="600"><br>

>Note: To do tasks do not have a date or time.

<img src="images/tags1.PNG" width="600"><br>

>Note: To add a tag, simply add a # followed by the tag name. 
To add a priority, simply add a ! at the back of the task.

<img src="images/tags2.PNG" width="600"><br>

###4.2 Editing a task

The edit task function enables you to update the task description which includes start time, end time, tags and priority and category. By typing the command and the task index followed by [enter], Simply will output the task details into the command bar for editing. After editing and pressing [enter], Simply will make the necessary changes to the task.


Format: **Edit** &lt;index&gt; [enter]

<img src="images/Capture8.PNG" width="600"><br>

Example: Edit D1 [enter]

Command Bar: Index task details are added to the back of the edit command

<img src="images/Capture9.PNG" width="600"><br>

Command bar: complete report, 120916, 1900 (Original task details are added to the end)

Format: Changes to task details [enter]

<img src="images/Capture10.PNG" width="600"><br>

Changes: **Report, 180916, 1900 #CS2103** [enter]

This will edit the current deadline task from CS2103 report to Report with an additional tag called #CS2103.

<img src="images/Capture11.PNG" width="600"><br>

<img src="images/Capture12.PNG" width="600"><br>

Example: Edit T1 [enter]

<img src="images/Capture13.PNG" width="600"><br>

Command Bar: go swimming (Original task details are added to the end)

<img src="images/Capture14.PNG" width="600"><br>

Changes: go swimming, **140516, 1600** [enter]

<img src="images/Capture15.PNG" width="600"><br>

This will edit the current todo task into a deadline task with the deadline on **140516 at 1600H**.

###4.3 Search Task by Partial Keyword

The search by partial keyword command enables you to search for any events, deadlines, to-dos that have been added to Simply. If the searched task have not been entered, an error message will be shown.

Format: 

**Search** &lt;keyword&gt;

<img src="images/Capture16.PNG" width="600"><br>

Example: 

Search **siloso**

Search 050316

Search 2359

Search #CS2103

<img src="images/Capture17.PNG" width="600"><br>

Only the tasks with the keyword are displayed.

###4.4 Marking Task as Complete 

The marking task as complete command enables you to mark the task as complete and hide the task.

Format: 

Complete &lt;index&gt;

Complete &lt;index&gt;-&lt;index&gt;

Complete &lt;index&gt;, &lt;index&gt;
    
<img src="images/Capture18.PNG" width="600"><br>    
    
Example: 
Complete T1

Complete T1-T3

Complete T1, T3

<img src="images/Capture19.PNG" width="600"><br>

>Note: if you want to select more than one task to complete, you can separated the task by a - to complete all tasks that are within the range. In addition, you also separate the task by a , to individually delete them.

###4.5 Display completed task

The display command will display the completed tasks in their respective categories.

Format: Display

<img src="images/Capture20.PNG" width="600"><br>

Example: Display

<img src="images/Capture21.PNG" width="600"><br>

###4.6 Undo the Most Recent Commands

The undo command enables you to undo the most recent command that have been executed.

Format: Undo &lt;number of operations&gt;

<img src="images/Capture22.PNG" width="600"><br>

Example: 
Undo

Undo 2

<img src="images/Capture23.PNG" width="600"><br>

>Note: The undo command can only undo a maximum of 5 commands that have been executed

###4.7 Deleting task

The delete command enables you to delete the tasks that you no longer need.

Format: 
Delete &lt;index&gt;

Delete &lt;index&gt;-&lt;index&gt;

Delete &lt;index&gt;, &lt;index&gt; 

<img src="images/Capture24.PNG" width="600"><br>

Example: 
Delete T3

Delete T1-T3

Delete T1, T3

<img src="images/Capture25.PNG" width="600"><br>

>Note: The delete command is flexible and allows you to delete more than 1 task at a time. If the indexes entered are separated by a -, Simply will delete all tasks between the numbers including the numbers enter. If the indexes are separated by a , Simply will delete the tasks entered individually. 

>Note: If no number is being adding, the default number of times the command will undo is 1.

###4.8 Exiting the program

This command enables you to close the program.

Format: **Exit**

Example: Exit

###4.9 Help

The help command will display the commands and their functionalities.

Format: **Help**

<img src="images/Capture26.PNG" width="600"><br>

Example : Help

<img src="images/Capture27.PNG" width="600"><br>

###Command Summary

 No. | Command | Format 
 -------- | :-------- | :--------- | :-----------
1| Add event| add [event_description, date, start_time, end_time] 
2| Add deadline | add deadline_description, date,end_time  
3| Add to-do | add to-do_description 
4| Add with tags and priorities | add [event_description, date, start_time, end_time] #tag !
5| Edit | edit &lt;index&gt; &lt;new_event_description&gt; 
6| Search | search &lt;keywords&gt; 
7| Complete | complete &lt;index&gt;&lt;index&gt;... 
8| Undo | undo &lt;number of times to undo, up to 5&gt; 
9| Delete | delete &lt;index&gt;&lt;index&gt; 
10| Exit | exit 
11| help | help 


