## 2.1 Fundamentals of Programming with VBA

### Overview

In today's class, you’ll introduce students to fundamental programming with Visual Basic for Applications (VBA). Today's class will cover foundational concepts, like variables, arrays, and conditionals, and serve as the prelude to upcoming work in Python and JavaScript.

### Class Objectives

By the end of this lesson, the students will be able to:

* Define building blocks of all programming languages: variables, arrays, conditionals, loops, and functions.
* Create simple VBA macros to trigger pop-ups and change cell values.
* Write VBA subroutines that use variables and conditionals.
* Develop essential coding skills including syntax recollection, pattern recognition, problem decomposition, and debugging.

---
### Instructor Notes

* Today marks the class’s first foray into fundamental programming. Emphasize that our goal is to understand fundamental concepts that will apply across all programming languages. VBA syntax is **not** what makes this week valuable for the rest of the course.

* Don’t worry if you are new to VBA: VBA syntax is easy to pick up, and the language is similar to most fundamental programming languages. VBA is a user-friendly language that combines basic programming tools with a GUI interface and familiar spreadsheet-manipulation methods. By the end of the week, you and your students may be surprised by how much fun you can have writing VBA code.

* Take time before class to familiarize yourself with this unit’s exercises and activities. More importantly, practice your workflow before class. Navigating between the VBA code and Microsoft Excel can be tricky. We suggest keeping your activities folder open in VS Code.

* As class progresses, demonstrate the VBA code in VS Code before opening it in Microsoft Excel and running the script. This may be helpful to students as Microsoft Excel has limited zoom capabilities in its VBA editor. However, you may find it easier to stick to Excel's VBA editor rather than copying and pasting code to and from VS Code.

* Pay close attention to time today. There are many "mini-exercises" in today's class, and it’s easy to lose time along the way. If necessary, feel free to cut the “Choose Your Story” conditional exercise and share it with students to review independently.

---

### Class Slides

* The slides for this lesson can be viewed on Google Drive here: [Lesson 2.1 Slides](https://docs.google.com/presentation/d/1TWgnpDnWSOI1U12OeHVBiMALAuvWS2C3KKQPrBeicWw/edit?usp=sharing).

* To add the slides to the student-facing repository, download the slides as a PDF by navigating to File, selecting "Download as," and then choosing "PDF document." Then, add the PDF file to your class repository along with other necessary files. You can view instructions for this [here](https://docs.google.com/document/d/1XM90c4s9XjwZHjdUlwEMcv2iXcO_yRGx5p2iLZ3BGNI/edit).

* **Note:** Editing access is not available for this document. If you wish to modify the slides, create a copy by navigating to File and selecting "Make a copy...".

---

### Time Tracker

| Start Time | Number | Activity                                           | Duration |
| ---------- | ------ | -------------------------------------------------- | -------- |
| 6:30 PM    | 1      | Instructor Do: Fundamentals of Programming with VBA Slides | 0:15     |
| 6:45 PM    | 2      | Instructor Do: Hello, World                        | 0:10     |
| 6:55 PM    | 3      | Students Do: Hello, VBA                            | 0:10     |
| 7:05 PM    | 4      | Review: Hello, VBA                                 | 0:05     |
| 7:10 PM    | 5      | Instructor Do: Button Clicks                       | 0:05     |
| 7:15 PM    | 6      | Students Do: Choose Your Button - Subroutines      | 0:10     |
| 7:25 PM    | 7      | Review: Choose Your Button                         | 0:05     |
| 7:30 PM    | 8      | Instructor Do: Cells And Ranges                    | 0:05     |
| 7:35 PM    | 9      | Students Do: Chess Board                           | 0:15     |
| 7:50 PM    | 10     | Review: Chess Board                                | 0:05     |
| 7:55 PM    | 11     | BREAK                                              | 0:15     |
| 8:10 PM    | 12     | Instructor Do: Variables                           | 0:05     |
| 8:15 PM    | 13     | Students Do: Total Calculator                      | 0:10     |
| 8:25 PM    | 14     | Review: Total Calculator                           | 0:05     |
| 8:30 PM    | 15     | Instructor Do: Arrays                              | 0:05     |
| 8:35 PM    | 16     | Instructor Do: Splitting Strings                   | 0:05     |
| 8:40 PM    | 17     | Students Do: Sentence Breaker                      | 0:20     |
| 9:00 PM    | 18     | Review: Sentence Breaker                           | 0:10     |
| 9:10 PM    | 19     | Instructor Do: Conditionals                        | 0:05     |
| 9:15 PM    | 20     | Students Do: Choose Your Story - Conditionals      | 0:05     |
| 9:20 PM    | 21     | Review: Choose Your Story                          | 0:05     |
| 9:25 PM    | 22     | Instructor Do: Intro Homework Assignment           | 0:05     |
| 9:30 PM    |        | END                                                |          |

---
### 1.  Instructor Do: Fundamentals of Programming with VBA Slides (15 min)

Welcome students back, and begin the day’s slideshow.

Today might be some students’ first experience with programming. Use the slides to introduce the concepts of variables, arrays, functions, loops, and conditionals. Don't spend too much time on syntax; in fact, avoid the topic entirely until you begin the code demonstrations. Instead, focus on the _concepts_ and _capabilities_ during your presentation. Students will get plenty of code-writing practice code after your presentation.

When prompted, have students complete the steps to confirm activation of the Developer tab in Microsoft Excel. Have TAs provide assistance as needed.

  * On Macs running Excel 365, to activate the Developer tab, open the Excel menu and select “Preferences,” then open the preferences for the Ribbon and Toolbar.

---

### 2. Instructor Do: Hello, World  (10 min)

**Corresponding Activity:** [01-Ins_HelloWorld](Activities/01-Ins_HelloWorld)

**File:** [hello_world_solution.xlsm](Activities/01-Ins_HelloWorld/Solved/hello_world_solution.xlsm)

* Once you've completed the slideshow, introduce the first VBA script. Open the VBA editor, and navigate to Module 1. All examples in this lesson plan and the ones in the rest of the unit can be found in Module 1, as in the following images:

  ![Images/developer.png](Images/developer.png)

  ![Images/module1.png](Images/module1.png)

Introduce the students to the editor’s interface, and be sure to discuss the following points:

  * Modules are organizational units of VBA code that are usually attached to a workbook or worksheet. We can create modules by right-clicking on a workbook or worksheet and then selecting "Insert Module."

  * Once inside a module, we can start writing a VBA script. In our case, we've already created a script that will trigger Excel to deliver a pop-up message.

VBA will run subroutines based on where the cursor is. Make sure your cursor is inside the `HelloWorld` subroutine, then the play button in your VBA editor to trigger the “Hello World” pop-up message box, as in the following images.

  ![Images/01-HelloWorld_2.png](Images/01-HelloWorld_2.png)

  ![Images/01-HelloWorld_3.png](Images/01-HelloWorld_3.png)

After demonstrating the code, open the [HelloWorld_solution.vbs](Activities/01-Ins_HelloWorld/Solved/hello_world_solution.vbs) script in your IDE. From the IDE, guide students through the key aspects of the subroutine. Be sure to discuss the following points:

  * The code begins with the keyword `Sub`, which is short for subroutine. This line is followed by `HelloWorld()`, which marks the title of our subroutine. The empty brackets indicate that our subroutine takes in no arguments. Explain that we'll cover functions, which _do_ take in arguments, at a later point.

  * Then, explain that our subroutine has one objective&mdash;to create a pop-up message box (`MsgBox`) containing the phrase "Hello World".

  * Finally, explain that once our subroutine has triggered our pop-up message, its work is done, and the subroutine is complete, which is denoted by the `End Sub` keywords. Emphasize that every subroutine must begin with the keyword `Sub` and end with `End Sub`.

```vb
Sub HelloWorld():
	MsgBox("Hello World")
End Sub
```

Answer any questions before proceeding to the next activity.

---

### 3.  Students Do: Hello, VBA  (10 min)

**Corresponding Activity:** [02-Stu_HelloVBA](Activities/02-Stu_HelloVBA)

**Instructions:** [README.md](Activities/02-Stu_HelloVBA/README.md)

Next, open the Excel Workbook [hello_vba_solution.xlsm](Activities/02-Stu_HelloVBA/Solved/hello_vba_solution.xlsm), and run the macro, as in the following image:

  ![Images/macro.png](Images/macro.png)

After demonstrating the three pop-ups, have students reproduce this effect on their machines. Send them the instructions.

---

### 4. Review: Hello, VBA (5 min)

Once time is up, share the solution found in [hello_vba_solution.vbs](Activities/02-Stu_HelloVBA/Solved/hello_vba_solution.vbs), and guide students through the code. Note that this exercise simply required that students create three sequential message boxes with text inside each box, as in the following code:

```vb
Sub HelloVBA():
  MsgBox ("Hello VBA!")
  MsgBox ("I have come to master your vicissitudes.")
  MsgBox ("And benefit from your automation.")
End Sub
```

Ask if there are any questions before sending out the solution and proceeding to the next example.

---

### 5. Instructor Do: Button Clicks (5 min)

**Corresponding Activity:** [03-Ins_ButtonClicks](Activities/03-Ins_ButtonClicks)

Next, return to the Developer tab, where you’ll demonstrate to students how to insert a button in their spreadsheet. The Mac layout is slightly different, so be patient with students if they have any difficulty finding features across operating systems.

First, create a button, as in the following image:

![Images/03-ButtonClicks_2.png](Images/03-ButtonClicks_2.png)

Once the button is created, the "Assign Macro" window will pop up, where you can choose to create a new macro or select an existing one, as in the following image:

![Images/03-ButtonClicks_3.png](Images/03-ButtonClicks_3.png)

If you accidentally close this window, you can always re-open it by right-clicking your button and selecting "Assign Macro"

If using the Excel file provided in [03-Ins_ButtonClicks](Activities/03-Ins_ButtonClicks), the button will be associated with a macro that simply prints "You clicked me" when the button is pressed, as in the following image:

![Images/03-ButtonClicks_4.png](Images/03-ButtonClicks_4.png)

---

### 6. Students Do: Choose Your Button - Subroutines (10 min)

**Corresponding Activity:** [04-Stu_ChooseYourButton-Subroutines](Activities/04-Stu_ChooseYourButton-Subroutines)

**Instructions:** [README.md](Activities/04-Stu_ChooseYourButton-Subroutines/README.md)

Next, open the Excel file [choose_your_button_solution.xlsm](Activities/04-Stu_ChooseYourButton-Subroutines/Solved/choose_your_button_solution.xlsm), and run the macro. Inform students that for this exercise, they will create two buttons that each run a different subroutine that trigger different messages when clicked.

---

### 7. Review: Choose Your Button (5 min)

Once time is complete, open and share the solution file [choose_your_button_solution.vbs](Activities/04-Stu_ChooseYourButton-Subroutines/Solved/choose_your_button_solution.vbs). Guide students through the VBA script. Be sure to cover the following points:

  * We created two VBA subroutines&mdash;one for each button.

  * Return to the Excel solution file, and point out that each button is associated with a different subroutine.

```vb
' Subroutine for Button 1
Sub Button1_Click()
    MsgBox ("You clicked Button 1!")
End Sub

' Subroutine for Button 2
Sub Button2_Click()
    MsgBox ("You clicked Button 2!")
End Sub
```

Answer any questions before proceeding to the next example.

---

### 8. Instructor Do: Cells And Ranges (5 min)

**Corresponding Activity:** [05-Ins_CellsAndRanges](Activities/05-Ins_CellsAndRanges)

Open the Excel file [cells_and_ranges_solution.xlsm](Activities/05-Ins_CellsAndRanges/Solved/cells_and_ranges_solution.xlsm), and run the `CellsAndRanges` macro. The macro can be run from the VBA editor; or you can navigate to the “Tools” menu in Excel, then to the “Macro” submenu where you select “Macros …”.

Be sure to clear out the contents of Sheet1 before you run the macro so you can demonstrate its effect. As you run the macro, explain the following points:

  * VBA provides two primary ways to modify the contents of a spreadsheet: `Cells` and `Ranges`.

  * `Ranges` provide a more customary Excel-based method for specifying cells of a spreadsheet. Ranges can be contiguous (e.g., `"F5:F7"`) or noncontiguous (e.g. `"R2,D2"`).

  * `Cells` provide a numeric, coordinate-based method for referencing cells in a spreadsheet. Point out to students that `Cells` are organized in a `(Row, Column)` format where integers 1, 2, and 3 denote columns A, B, and C, etc.
  * `.Value` is a method that we add to the end of our `Cell` or `Range` references to specify that we want to change the content value of these cells. This is worth noting because it may help students realize that `Cells(X, X)` isn't just capturing the contents of the cell; instead, it is capturing the entire "Cell Object," including the formatting, style, and other aspects of the cell beyond the content itself.

    ```vb
    ' Inserting Data Via Cells
    Cells(2, 1).Value = "Cat"
    Cells(2, 2).Value = "In"
    Cells(2, 3).Value = "The"
    Cells(2, 4).Value = "Hat"

    ' Inserting Data Via Ranges
    Range("F1").Value = "I"
    Range("F2").Value = "Am"
    Range("F3").Value = "Sam"
    ```

  * Ranges allow us to insert data across multiple cells simultaneously, as in the following code:

    ```vb
    ' Inserting Data Across Ranges
    Range("F5:F7").Value = 5
    ```

    * Therefore, ranges are used more often, but referring to cells can be especially useful in "loop-based" programs because we can iterate the coordinates and manipulate the cells that are referenced. Let students know that they will refine their understanding of this concept as the week progresses.

Answer any questions before sending out the XLSM file to students.

---

### 9. Students Do: Chess Board (15 min)

**Corresponding Activity:** [06-Stu_ChessBoard-CellsAndRanges](Activities/06-Stu_ChessBoard-CellsAndRanges)

Next, proceed to the student activity. Open the solution file [chess_board_solution.xlsm](Activities/06-Stu_ChessBoard-CellsAndRanges/Solved/chess_board_solution.xlsm), and run the macro. Explain to students that they’ll be adding text-based chess pieces to a chessboard using a combination of `Cells` and `Ranges`.

![Images/06-ChessBoard_1.png](Images/06-ChessBoard_1.png)

Explain to students that iterators are marked using `i` and `j` for the following reasons:

  * They are widely accepted as iterator names in other programming languages, such as JavaScript and C++.

  * The use of `i` and `j` as iterators was commonplace in math before some higher-level languages were even created.

  * Practicing with these iterators now will help build confidence for when we encounter these iterators again&mdash;in the curriculum and then in the field.

Then, send students the following image, spreadsheet, and instructions:

**Files:**

  * [ChessBoard.png](Activities/06-Stu_ChessBoard-CellsAndRanges/Images/ChessBoard.png)

  * [chess_board.xlsm](Activities/06-Stu_ChessBoard-CellsAndRanges/Unsolved/chess_board.xlsm)

**Instructions:** [README.md](Activities/06-Stu_ChessBoard-CellsAndRanges/README.md)

---

### 10. Review: Chess Board (5 min)

**File:** [chess_board_solution.vbs](Activities/06-Stu_ChessBoard-CellsAndRanges/Solved/chess_board_solution.vbs)

Once time is up, open the solution file, send it out to students, and guide students through the code.

To begin, review the `Range` examples for the top cells; in particular, point out how we used the syntax of `Range("A1", "H1")` to place multiple pieces at one time.

```vb
  ' Insert Pawns
  Range("A2:H2").value = "Pawn"

  ' Insert Rooks
  Range("A1, H1").value = "Rook"

  ' Insert Knights
  Range("B1, G1").value = "Knight"

  ' Insert Bishops
  Range("C1, F1").value = "Bishop"

  ' Insert Queen
  Range("D1").value = "Queen"

  ' Insert King
  Range("E1").value = "King"
```

Then, proceed through the bottom side of the board using `Cells`, as in the following image:

```vb
  ' Insert Pawns
  Cells(7, 1).value = "Pawn"
  Cells(7, 2).value = "Pawn"
  Cells(7, 3).value = "Pawn"
  Cells(7, 4).value = "Pawn"
  Cells(7, 5).value = "Pawn"
  Cells(7, 6).value = "Pawn"
  Cells(7, 7).value = "Pawn"
  Cells(7, 8).value = "Pawn"

  ' Insert Rooks
  Cells(8, 1).value = "Rook"
  Cells(8, 8).value = "Rook"

  ' Insert Knights
  Cells(8, 2).value = "Knight"
  Cells(8, 7).value = "Knight"

  ' Insert Bishops
  Cells(8, 3).value = "Bishop"
  Cells(8, 6).value = "Bishop"

  ' Insert Queen
  Cells(8, 4).value = "Queen"

  ' Insert King
  Cells(8, 5).value = "King"
```

As you discuss the solution, identify opportunities to engage students and ask them direct, pointed questions.

---

### 11. BREAK (15 min)

---

### 12. Instructor Do: Variables (5 min)

**Corresponding Activity:** [07-Ins_Variables](Activities/07-Ins_Variables)

Next, transition to the concept of variables. Remind students that variables are **named items** in programming. They can store strings (text), numerics (integers and doubles for decimals), booleans (true or false), and more. Then, open the `variables` script [variables_solution.vbs](Activities/07-Ins_Variables/Solved/variables_solution.vbs).

Guide students through each example:

  * Point out that VBA uses the single quote (`'`) to denote a comment: everything following a single quote is just for humans.

  * Break down the VBA syntax for creating variables. Explain that we create (declare) variables by using the `Dim` keyword followed by the name of the variable and the type `as String`.

  * Point out that by declaring the variable, we have created space in memory to store a value. We access that stored value by using the variable’s name.

  * We can "concatenate" strings by combining them, and we can perform mathematical functions by combining numeric variables with operators.

  ```vb
      ' Basic String Variable
      ' ----------------------------------------
      Dim name As String
      name = "Gandalf"

      MsgBox (name)

      ' Basic String Concatenation (Combination)
      ' ----------------------------------------
      Dim title As String
      title = "The Great"

      Dim fullname As String
      fullname = name + " " + title

      MsgBox (fullname)
  ```

  * We can also use these variables to set the values of our cells.

  ```vb
      ' Basic Numeric manipulation
      ' ----------------------------------------
      Cells(1, 1).Value = price * (1 + tax)
  ```

  * Finally, we can combine numerics and strings by "casting" our numerics into string format using the `Str()` method. Similarly, we can cast strings into integers using the `Int()` method.

  ```vb
      ' String, Numeric Combination (Casting)
      ' ----------------------------------------
      MsgBox ("I am " + Str(age1) + " years old.")
  ```

  * Check for any questions before running the script and sharing it with students.

---

### 13. Students Do: Total Calculator (10 min)

**Corresponding Activity:** [08-Stu_TotalCalculator-Variables](Activities/08-Stu_TotalCalculator-Variables)

Next, introduce the student exercise. This may be a challenge for students who are new to programming, so please be patient as they establish a rhythm switching between the code examples you provide and their own code editors.

In this exercise, students will create a basic VBA script that takes in user-provided `Price`, `Tax`, and `Quantity` values to calculate a total value. They will need to create variables to store these quantities before providing a final output.

Send out the following files and instructions to students:

**Files:**

  * [total_calculator.vbs](Activities/08-Stu_TotalCalculator-Variables/Unsolved/total_calculator.vbs)

  * [total_calculator.xlsm](Activities/08-Stu_TotalCalculator-Variables/Unsolved/total_calculator.xlsm)

**Instructions:** [total_calculator.xlsm](Activities/08-Stu_TotalCalculator-Variables/README.md)

---

### 14. Review: Total Calculator (5 min)

Once time is up, open the solution [total_calculator_solution.vbs](Activities/08-Stu_TotalCalculator-Variables/Solved/total_calculator_solution.vbs). Guide students through the final code, and be sure to cover the following points:

  * We created a set of variables for `Price`, `Tax`, `Quantity`, and `Total`, each as the data type `Double`.

  * We then used the value of the cells to assign values to `Price`, `Tax`, and `Quantity`.

  * The code then uses these variables to calculate `Total`.

  * Finally, we create a message box to print the `Total`, and set the value of our `Total` cell as the variable value.

```vb
    ' Create variables for the Price, Tax, Quantity, and Total
    Dim Price As Double
    Dim Tax As Double
    Dim Quantity As Double
    Dim Total As Double

    ' Retrieve and store the data values in each variable
    Price = Range("B2").Value
    Tax = Range("C2").Value
    Quantity = Range("D2").Value

    ' Calculate the total by using each of the variables
    Total = Price * (1 + Tax) * Quantity

    ' Create a Message Box for the Total and insert into cell
    MsgBox ("Your total is $" + Str(Total))
    Range("E2").Value = Total
```

Answer any questions before sharing the solution file.

---

### 15. Instructor Do: Arrays (5 min)

**Corresponding Activity:** [09-Ins_Arrays](Activities/09-Ins_Arrays)

Now, introduce the students to our next concept, **arrays**. Re-emphasize that students do not need to master or memorize VBA syntax. Our goal is to build an understanding of programming fundamentals, and arrays are an essential building block across programming languages.

Open and share the script in [simple_arrays_solution.xlsm](Activities/09-Ins_Arrays/Solved/simple_arrays_solution.xlsm), and guide students through the code. Be sure to cover the following points:

  * Arrays use zero-based numbering (0-indexed), meaning that the first element is 0 instead of 1. Note that zero-based numbering is a common paradigm across programming languages (Python, JavaScript, etc.).

  * We created an array called `Ingredients` to hold six strings, but because of zero-indexing, five is the final number that we pass in. So, (0,1,2,3,4,5) is an array with six spots or positions.

  * We then added elements to this array using the `Ingredients(X)` syntax.

  * We then retrieved these values by referencing our array with the index number.

```vb
    ' Basic Array Example
    ' ------------------------------------------
    ' Create the Ingredients Array
    Dim Ingredients(5) as String

    ' Add Ingredients to the Array
    Ingredients(0) = "Chocolate Bar"
    Ingredients(1) = "Peanut Butter"
    Ingredients(2) = "Jelly"
    Ingredients(3) = "Macaroni"
    Ingredients(4) = "Potato Salad"
    Ingredients(5) = "Dragonfruit"

    ' Retrieve specific elements of the array
    MsgBox(Ingredients(4))
    MsgBox(Ingredients(0))
```

Answer any questions before proceeding to the next example.

---

### 16. Instructor Do: Splitting Strings (5 min)

**Corresponding Activity:** [10-Ins_Splitting](Activities/10-Ins_Splitting)

Next, we’ll be introducing the `Split` method, which breaks apart strings based on a provided delimiter. These broken-down strings will then become elements of a larger array.

**Files:**

  * [splitting_solution.xlsm](Activities/10-Ins_Splitting/Solved/splitting_solution.xlsm)

  * [splitting_solution.vbs](Activities/10-Ins_Splitting/Solved/splitting_solution.vbs)

As you guide students through this example, be sure to cover the following points:

  * A `Words` array is created with an undefined number of string elements.

  * A variable `Shakespeare` is used to hold a line of text.

  * We then use the `Split` method to break apart the `Shakespeare` variable by spaces between words. The resulting array takes the form `["To", "be", "or", "not", "to", "be", ...]`.

  * We can then select individual words from the resulting array by referencing the word's index in the array.

```vb
' String Splitting Example
' ------------------------------------------
Dim Words() As String
Dim Shakespeare As String
Shakespeare = "To be or not to be. That is the question"

' Break apart the Shakespeare quote into individual words
Words = Split(Shakespeare, " ")

' Print individual word
MsgBox (Words(5))
```

Answer any questions before proceeding to the next example.

---

### 17. Students Do: Sentence Breaker (20 min)

**Corresponding Activity:** [11-Stu_SentenceBreaker-Splitting](Activities/11-Stu_SentenceBreaker-Splitting)

Be prepared for this exercise. It’s a challenging one! Be sure to check in with students and provide support as they work through their thinking process. They will be creating an Excel macro that identifies words based on user-provided word numbers.

  * For example, if a user provides the number 3 for a given sentence, "Any fool can know. The point is to understand," then their resulting script should print the word "can."

Open the solved Excel workbook [sentence_breaker_solution.xlsm](Activities/11-Stu_SentenceBreaker-Splitting/Solved/sentence_breaker_solution.xlsm), clear out the green boxes containing the results, and change the word numbers.

Then, run the script, and demonstrate to students that the macro "finds" the correct words based on the word number, as in the following image:

![Images/12-SentenceArray_2.png](Images/12-SentenceArray_2.png)

Then, send students the following files and instructions:

**Files:**

  * [sentence_breaker.vbs](Activities/11-Stu_SentenceBreaker-Splitting/Unsolved/sentence_breaker.vbs)

  * [sentence_breaker.xlsm](Activities/11-Stu_SentenceBreaker-Splitting/Unsolved/sentence_breaker.xlsm)

**Instructions:** [README.md](Activities/11-Stu_SentenceBreaker-Splitting/README.md)

---

### 18. Review: Sentence Breaker (10 min)

Once time is up, open the solution script [sentence_breaker_solution.vbs](Activities/11-Stu_SentenceBreaker-Splitting/Solved/sentence_breaker_solution.vbs). Then, guide students through the solution, and cover four key areas:

  * The first key area is where we declare and assign a variable to hold our sentence.

    ```vb
    ' Retrieve the user sentence and store in variable
    Dim Sentence As String
    Sentence = Cells(1, 2).Value
    MsgBox (Sentence)
    ```

  * The next key area is where we declare our variables associated with the word numbers. Each of these is drawn from the cell values where users provide their input.

    ```vb
    num1 = Cells(4, 1).Value
    num2 = Cells(5, 1).Value
    num3 = Cells(6, 1).Value
    ```

  * In our next key area, we break apart our sentence into an array using the `Split` method.

    ```vb
    ' Split the user's sentence into words
    Dim SentenceArray() As String
    SentenceArray = Split(Sentence, " ")
    ```

  * Finally, we use the word numbers provided to draw from the sentence array we created. We subtract one from the word number to account for the fact that users will provide word numbers beginning at 1, while our array indexes words starting at 0.

    ```vb
    ' Use the word numbers to retrieve the specific words in the sentence
    ' Remember to offset by the 0 index
    Cells(4, 2).Value = SentenceArray(num1 - 1)
    Cells(5, 2).Value = SentenceArray(num2 - 1)
    Cells(6, 2).Value = SentenceArray(num3 - 1)
    ```

Once you've broken down the code, send it to students to review. Encourage them to talk it over with the student next to them for a few moments, then check for any new questions that come out of this discussion.

---

### 19. Instructor Do: Conditionals (5 min)

**Corresponding Activity:** [12-Ins_Conditionals](Activities/12-Ins_Conditionals)

Next, open the files found in [12-Ins_Conditionals](Activities/12-Ins_Conditionals/Solved). Use these examples to guide students through the use of conditionals in VBA. Be sure to cover the following points:

  * Note that VBA conditionals have practical benefits over traditional Excel formulas. Gone are the days of squeezing conditionals into a single Excel formula. With VBA, we have cleaner syntax and more nuanced conditionals.

  * In VBA, the syntax for conditionals involves `If`, `Then`, and `End If`. Additional keywords include `ElseIf` and `Else`.

  * In VBA, we can combine conditions using the keywords `And` and `Or`.

Finally, send these files to students as a reference for the next activity.

```vb
' Simple Conditional Example
' ------------------------------------------
If Range("A2").Value > Range("B2").Value Then
    MsgBox ("Num 1 is greater than Num 2")
End If

' Simple Conditional with If, Else, and Elseif
' ------------------------------------------
If Range("A5").Value > Range("B5").Value Then
    MsgBox ("Num 3 is greater than Num 4")

ElseIf Range("A5").Value < Range("B5").Value Then
    MsgBox("Num 4 is greater than Num 3")

Else
    MsgBox("Num 3 and Num 4 are equal")

End If
```

---

### 20. Students Do: Choose Your Story - Conditionals (5 min)

**Corresponding Activity:** [13-Stu_ChooseYourStory-Conditionals](Activities/13-Stu_ChooseYourStory-Conditionals)

**Instructions:** [README.md](Activities/13-Stu_ChooseYourStory-Conditionals/README.md)

If time permits, begin the final exercise of the day. In this exercise, students are tasked with creating a simple game that outputs a message box based on a user's input number, as in the following image:

![Images/14-ChoosePath_1.png](Images/14-ChoosePath_1.png)

---

### 21. Review: Choose Your Story (5 min)

Once time is up, open the [solution](Activities/13-Stu_ChooseYourStory-Conditionals/Solved), and share it with students. Guide them through the code’s logic and use of VBA conditional syntax

```vb
' Use conditionals to change message box based on user input
If (Range("B1").Value = 1) Then
    MsgBox("You choose to enter the wooded forest of doom!")

Elseif (Range("B1").Value = 2) Then
    MsgBox("You choose to enter the fiery volcano of doom!")

Elseif (Range("B1").Value = 3) Then
    MsgBox("You choose to enter the terrifying jungle of doom!")

Elseif (Range("B1").Value = 4) Then
    MsgBox("You choose to enter the bathroom")

Else
    MsgBox("You decide to stay home instead.")

End If
```

Answer any questions before providing students with the solution.

---

### 22. Instructor Do: Intro Homework Assignment (5 min)

With whatever time remains, briefly introduce students to this week's homework. The homework assignment essentially tasks them with creating a VBA script to loop through stock market records to identify various stocks based on provided conditions. Let them know that they will be able to complete the homework by the end of module.

Wish them well, and then close out class!

---

© 2022 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.
