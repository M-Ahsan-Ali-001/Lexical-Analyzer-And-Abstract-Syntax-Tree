# Lexical Analyzer:

<br>•	Firstly, take the  expression from the user  and store that in string.
<br>•	splitFunction() , in this function we store the characters one by one in a list and remove the white spaces.
<br>•	Print_Before_Tokenization() ,in this function we print the entered equation.
<br>•	tokenFinder(), in this function  we check the elements of split list one by using regular Expression to check form which category the current element belongs to.
<br>•	We get a match, we put that element in a dictionary along with is category type. 
<div style=" margin-left: 1000px;">
 <h2>       Regex used: </h2>
 
<br>      o	Re.search(‘[a-zA-Z]’ , element) :  it returns the if string contains alphabets.
<br>      o	Re.search(‘[0-9]’, element) :  it returns the if string contains constants.
<br>      o	Re.search(‘[+ , / , * ]’ , element) it returns the if string contains operators.
<br>      o	Re.search(‘[{ , }  , ( , ) ]’ , element) it returns the if string contains punctuators.
<br>      o	Re.search(‘[& , %  , $ ]’ , element) it returns the if string contains Speical Characters.
</div>
