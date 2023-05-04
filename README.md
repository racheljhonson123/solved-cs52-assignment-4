Download Link: https://assignmentchef.com/product/solved-cs52-assignment-4
<br>
<strong>Background:</strong>The purpose of this assignment is to get practice working with classes and objects.  Unlike a C program which is defined by its flow of control, C++ programs are defined by the classes and objects that are a part of it.  Thinking in terms of classes and objects is challenging for those new to these ideas.  It takes times to understand how they work and what is involved in using them.  The purpose of this homework is to introduce these ideas and get you thinking about them.  The first part is to get you thinking about design.  There are many many correct answers to Part A.  What I am looking for is a box diagram that represents a class.  You don’t have to write code for Part 1.  Object-oriented programmers often use diagrams to convey programming ideas.  As they say, a picture is worth a thousand words  (or lines of code…)  Part B introduces the class FlashDrive.  We will be doing a number of different homeworks with the FlashDrive class, so you will get to know it very well…  Similarly, you don’t have to write implementation code for Part B, but I will offer you extra-credit if you do (and do it correctly… &#x1f642;

<h3><strong>part_a: mahjong_design</strong></h3>

Think of three classes that would be used in a Mahjong solitaire game. At least one of these classes must have multiple instances in the game. For each of these classes, describe two attributes (instance variables) and two operations (methods). A one line, simple description is sufficient for each attribute and operation. Do not worry about all the details that would be involved in finally implementing these classes in C++. Concentrate on modeling the objects.  Represent each class using the class diagram (box) notation described during lecture.

If you are not familiar with Mahjong Solitaire, here is a brief description:Mahjong is a single-play tile game played in turns.  The object of Mahjong is to remove all the tiles from the board, a pair at a time by matching tiles.   Remove all tiles from the board by finding matching pairs of free tiles.  Two tiles match if they have the same picture and number.  However, only “free” tiles can be removed by a player during their turn.  A free tile is one that has no other tiles on top of it, and is unblocked on either its right or left side.  The game also includes a time and turn counter.  Players should try to finish as quickly as they can in as few turns as possible.

To help you, a screen shot of Mahjong is shown below.  Look at the items in the picture. Almost anything you see on the screen could be an object. Reread the above description of the game. Objects are frequently nouns in the specification of a program.

If the game is quite unfamiliar to you, try playing it!

<table id="AutoNumber1" border="1" width="26%" cellspacing="0" cellpadding="0">

 <tbody>

  <tr>

   <td width="40%"><img decoding="async" width="413" height="326" data-recalc-dims="1" data-src="https://i0.wp.com/www.howardstahl.com/cs52/mahjong.jpg?resize=413%2C326" class="lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

    <noscript>

     <img decoding="async" src="https://i0.wp.com/www.howardstahl.com/cs52/mahjong.jpg?resize=413%2C326" width="413" height="326" data-recalc-dims="1">

    </noscript></td>

  </tr>

 </tbody>

</table>

<h3><strong>part_b: flashdrive_driver</strong></h3>

I have provided you with a sample class named FlashDrive which has been diagrammed below and described in the online course content.  For this unit, I’d like you to identify additional member variables (data) that would be appropriate for the class FlashDrive.  I would also like you to identify additional methods (functions) that would be appropriate for the class FlashDrive.  Submit a .h file for FlashDrive with the new possible methods and members you have identified commented and explained.  YOU ARE NOT REQUIRED TO CODE UP ANYTHING MORE THAN THE .H FILE, BUT I MAY AWARD YOU EXTRA CREDIT IF YOU DO…

<table border="1" width="98%" cellspacing="0" cellpadding="0">

 <tbody>

  <tr>

   <td width="38%">

    <table border="1" width="98%" cellspacing="0" cellpadding="0">

     <tbody>

      <tr>

       <td width="100%"><strong>FlashDrive</strong></td>

      </tr>

      <tr>

       <td width="100%">FlashDrive( );FlashDrive( int capacity, int used, bool pluggedIn );void plugIn( );void pullOut( );void writeData( int amount );void eraseData( int amount );void formatDrive( );int getCapacity( );void setCapacity( int amount );int getUsed( );void setUsed( int amount );bool isPluggedIn( );</td>

      </tr>

      <tr>

       <td width="100%">int my_StorageCapacity;int my_StorageUsed;bool my_IsPluggedIn;</td>

      </tr>

     </tbody>

    </table></td>

   <td width="105%">

    <table border="1" width="100%" cellspacing="0" cellpadding="0">

     <tbody>

      <tr>

       <td width="100%"><strong>Sample Driver Code</strong></td>

      </tr>

      <tr>

       <td width="100%">#include &lt;iostream&gt;#include “FlashDrive.h”void main( ){int i;cout &lt;&lt; “Welcome to Howie’s Flash USB Drive Store!”&lt;&lt; endl;cout &lt;&lt; “How much memory do you need? “;cin &gt;&gt; i;FlashDrive f( i, 0,false );cout &lt;&lt; “Let’s format the drive…” &lt;&lt; endl;f.formatDrive();cout &lt;&lt; “Let’s plug in the drive…” &lt;&lt; endl;f.plugIn();cout &lt;&lt; “Let’s write some data…” &lt;&lt; endl;f.writeData( 10 );cout &lt;&lt; “Let’s unplug the drive…” &lt;&lt; endl;f.pullOut();cout &lt;&lt; “Enjoy your drive!!” &lt;&lt; endl;}</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>




<h3><strong>Overall</strong></h3>

<ul>

 <li>Your submission should follow this organization:

  <ul>

   <li>part_a

    <ul>

     <li>mahjong_design.pdf</li>

    </ul></li>

   <li>part_b

    <ul>

     <li>flashdrive.h</li>

    </ul></li>

  </ul></li>

</ul>