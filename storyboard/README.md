## Storyboard (Round 2)

Experiment 1: N Queen Problem
### 1. Story Outline:

This problem is to find an arrangement of N queens on a chess board, such that no queen can attack any other queens on the board.
The chess queens can attack in any direction as horizontal, vertical, horizontal and diagonal way.
A binary matrix is used to display the positions of N Queens, where no queens can attack other queens.

### 2. Story:

The N Queen is the problem of placing N chess queens on an N×N chessboard so that no two queens attack each other. For example, following is a solution for 4 Queen problem.
The N Queen is the problem of placing N chess queens on an N×N chessboard so that no two queens attack each other. For example, following are two solutions for 4 Queen problem.
	Q		
			Q
Q			
		Q	

#### 2.1 Set the Visual Stage Description:
Input and Output
Input:
The size of a chess board. Generally, it is 8. as (8 x 8 is the size of a normal chess board.)
Output:
The matrix that represents in which row and column the N Queens can be placed.
If the solution does not exist, it will return false.

1 0 0 0 0 0 0 0
0 0 0 0 0 0 1 0
0 0 0 0 1 0 0 0
0 0 0 0 0 0 0 1
0 1 0 0 0 0 0 0
0 0 0 1 0 0 0 0
0 0 0 0 0 1 0 0
0 0 1 0 0 0 0 0

In this output, the value 1 indicates the correct place for the queens.
The 0 denotes the blank spaces on the chess board.

#### 2.2 Set User Objectives & Goals:
User will be able to explain Backtracking algorithm.
User will be able to describe Time Complexity
User will be able toanalyze the matrices.
User can able to evaluate the place of queens in such a way that no queen attack each other


#### 2.3 Set the Pathway Activities:

isValid(board, row, col)
Input: The chess board, row and the column of the board.
Output − True when placing a queen in row and place position is a valid or not.
Begin
   if there is a queen at the left of current col, then
      return false
   if there is a queen at the left upper diagonal, then
      return false
   if there is a queen at the left lower diagonal, then
      return false;
   return true //otherwise it is valid place
End
solveNQueen(board, col)
Input − The chess board, the col where the queen is trying to be placed.
Output −  The position matrix where queens are placed.
Begin
   if all columns are filled, then
      return true
   for each row of the board, do
      if isValid(board, i, col), then
         set queen at place (i, col) in the board
         if solveNQueen(board, col+1) = true, then
            return true
         otherwise remove queen from place (i, col) from board.
   done
   return false
End


##### 2.4 Set Challenges and Questions/Complexity/Variations in Questions:

Challenges:No queen will attack each other.

Questions/Complexity/Variation:There can be multiple solutions, so we have to check all solutions.


##### 2.5 Allow pitfalls:
Describe the pitfalls here: (guide : (while traversing or while solving challenge, how will we bring a situation in front of him that he commits mistake if he is not attentive , or not following procedure , descriptive))

##### 2.6 Conclusion:
Describe conclusion here : (guide: This may include displaying: how much time did the user take to solve the questions/ How many questions were right?/ How many hints did the learner use. Based on this the evaluation/marking to be suggested to the user. (once he is towards the completion of the experiment, what LO he is taking along with him, what will be his probable, interpretation/conclusion , descriptive) )

##### 2.7 Equations/formulas: NA
Type equations here : (guide : ( a separate sheet having equations / programs for the lab exper3ment to be shared along with the Story submissions (1) . You can mark it as numerical reference numbers within the story narration (like we cite in the research papers) and then separately share these equations/programs sheets as a reference, do not include the equations as a whole in the narration))
Tool can be used to integrate formula in Markdown <b> [here](http://latex.codecogs.com/eqneditor/samples/example3.php) </b>


### 3. Flowchart 4
<img src="flowchart/flowchart.png"/><br>
link to flow chart Here : Store in the  /flowchart folder within Round2 folder in your repo
<br>
(guide :The lab proposer should extract logic from the story, prepare a flowchart from the story narration and write the algorithm to execute the black box.  use Google Drawings https://docs.google.com/drawings/ (send the link to your flowchart and also attach .png by exporting it )

### 4. Mindmap:
<img src="mindmap/mindmap.png"/>
 Link to mindmap here : Store the mindmap in both .mm & .png extension in the  /mindmap folder and include link of only .pdf verison here
 <br>
 (guide : An elaborate mind map (connecting all the points in the experiment flow ) should be prepared and submitted by the lab proposer. The mind map should be a clear and detailed document that takes into account all minute intri5acies involved in the development of virtual lab. The mindmap should be self-content and any developer across the globe should be able to code it with all those details. using only FreeMind http://freemind.sourceforge.net/wiki/index.php/Main_Page (send the .png file and also the original .mm extension project file. )

### 5. Storyboard :
Storyboard: <a href="Storyboard/carwiper.gif"> [here]</a>
Link to storybaord (.gif file ) here :
(guide: This document should include sketching and description scene wise (duration, action, description). Software to be used for storyboarding : https://wonderunit.com/storyboarder/ (Its a FOSS tool) . tutorial on how to use it https://www.youtube.com/watch?v=LAeCEpG0KX4
