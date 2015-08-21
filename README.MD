###FREE CODE CAMP###
####Bonfire 106: Title Case a Sentence####
[Link to Test](http://freecodecamp.com/challenges/bonfire-title-case-a-sentence)
<p>
In this test we are tasked with taking a sentence and converting it to title case (first letter of every word capitalized, including a, an, the etc...)
<p>
My initial thoughts were the following:
<li>Convert to all lowercase</li>
<li>Convert to an array of words (split(" "))</li>
<del><li>pop first letter of  each array off</li></del>
<li>capitalize first letter</li>
<li><del>rejoin to word</del></li>
<p>
After thinking about it, that seemed like a few too many steps, and with a bit of research [here](http://www.w3schools.com/jsref/jsref_charat.asp) I learned about charAt() as a method of finding a character in a specific location within an array.  This means I didn't need to pop the first letter off the array, I simply needed to grab the desired character (and since I've already converted the entire string to lowerCase, it will always be <em>only</em> the first character) and convert it to upperCase.  
<p>
![image](https://cloud.githubusercontent.com/assets/12467136/9418453/fb47c952-4808-11e5-968d-072adcb36423.png)
<p>After I tried this I realized that I was only returning the first letters of each word and I did, in fact, need to concatenate the words back together. This need lead me [here](http://www.w3schools.com/jsref/jsref_slice_array.asp) where I learned about slice() being able to move into a specific location within an array. 
<p>
![image](https://cloud.githubusercontent.com/assets/12467136/9418414/b2e2281a-4808-11e5-8b3e-f8b65c442ed3.png)
<p>
So now concatenation was as simple as bringing the the first letter of each word together with its respective  string (str[i]). All that was needed from this point was simply re-joining the array of words back into a String (join()) to give the test the answer it wanted, in the format it wanted. <p>
![image](https://cloud.githubusercontent.com/assets/12467136/9418405/981c7c56-4808-11e5-9ffd-a838eb426ced.png)