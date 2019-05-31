# TransversalExercise-TankProblem
A python coded numerical model that tries to prepare a model i.e. simplification of the reality; within step                    by step modifications in it. Here, to understand and to prepare a hydrological cycle model for a watershed.

<h2>
    <ul>
        <li>Objective</li>
    </ul>
</h2>
<blockquote>
            <font size="4">To integrate the concepts of Conditionals, Loops, File Manipulation, Functions, Matrix Manipulation using Python to create a virtual watershed model. 
            </font>
</blockquote>
<h2>
    <ul>
        <li>INTRODUCTION</li>
    </ul>
</h2>
<blockquote>
            <font size="4">The activity is based on, preparing a model i.e. simplification of the reality; within step
                   by step modifications in it. Here, to understand and to prepare a hydrological cycle model for a 
                   watershed(Sugawara) we have considered a small tank which receives water and produces a discharge. 
                   The model develops through several steps with different number of variables at each step.
            </font>
            <font size="4">
                   <li>Tank model with two outlets using 'if...elif...else' conditional concepts</li>
                   <li>Tank model discharge with time series using concepts of 'For Loop'</li>
                   <li>Read and store precipitation data using concepts of 'File Manipulation'</li>
                   <li>Calculation of river discharge at the outlet following the 'flow accummulation 
                   approach' from upstream cells to the downstream using 'Matrix 
                   Manipulation'concepts</li>
                   <li>Function to estimate Q using concepts of
                   'Functions'</li>
            </font>          
</blockquote>
***
<h2><ul><li>Exercise 1. Tank model with Two Outlets</li></ul></h2>
***
![TransversalExercise1.JPG](attachment:TransversalExercise1.JPG)
<p><center><font size="3"><strong>Figure 1. Tank model with two outlets</strong></font></center></p>

### <u>Discription</u> :
<blockquote><font size="4">
<p>General idea behind this exercise is that, we considered a general flow condition in a watershed in reality and genrated a model based on it following into different steps.</p>
<p>In this first step, we have considered a tank with two outlets considering two typs of flow through a watershed and calculated the discharge depending on the depth of water in it.We also applied the 'if...elif...else' conditional concepts to get the solution.</p>

<p>In this Exercise, we have prepared a code that will ask the user to enter the three values (i.e. __k__, __h__ and __d__ as mentioned in the figure above) which will be stored into the three variables. The program will then asess the given input especially values of h and d (as shown in the figure above). Program will then either calculate the discharge from both outlets and store it into two variables named __Q1__ and __Q2__ or it will calculate discharge from only Q2 or there could be the condition of no discharge also. Finally, if there is a condition to generate any discharge the calculated value of disharge will be stored in a variable named '__Qtotal__' to print the result or if there is no flow condition occur then suitable message will be produced.</p>

</font></blockquote>


<blockquote>
    <font size="3">
        __Following is the Console we get when entered above mentioned values:
        <ul>
            <li>Example 1:
                <br>>>> Enter the value of k:
                <br>>>> a
                <br>>>> Invalid Input!...Please Enter a valid input! (i.e. any real number)
                <br>>>> 1.5
                <br>>>> Enter the value of h:
                <br>>>> sfsdfs
                <br>>>> Invalid Input!...Please Enter a valid input! (i.e. any real number)
                <br>>>> 5
                <br>>>> Enter the value of d:
                <br>>>> oefi
                <br>>>> Invalid Input!...Please Enter a valid input! (i.e. any real number)
                <br>>>> 3
                <br>>>> (Q)1 =  3.0 m^3/sec
                <br>>>> (Q)2 =  7.5 m^3/sec
                <br>>>> (Q)total =   10.5 m^3/sec
            </li>
        </ul>
        <ul>
            <li>Example 2:
                <br>>>> 1.5
                <br>>>> Enter the value of h:
                <br>>>> 5
                <br>>>> Enter the value of d:
                <br>>>> 3
                <br>>>> (Q)1 =  3.0 m<sup>3</sup>/ sec
                <br>>>> (Q)2 =  7.5 m<sup>3</sup>/ sec
                <br>>>> (Q)total =   10.5 m<sup>3</sup>/ sec__
            </li>
        </ul>
    </font>
</blockquote>

***
### <u>Code</u> :
