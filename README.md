# Learning.repo
This will be an unconventional README consisting of advice on approaching web development as a beginner. If you’re a self-learning student like me with a full-time job, this is for you. 

One of the things I have learned in this journey is that getting into a coding career requires a solid roadmap. Free Code Camp will provide an excellent roadmap to follow. Further, it would be best if you also had a lot of discipline, organization skills, and self-awareness to keep yourself motivated along the way. Trust me; it won’t be easy. Nonetheless, the moment you start building things with code and seeing them materialize will be gratifying… Just don’t get too comfortable with the basics. It’s about the journey, not the ending.

I will update my learning journey in this REPO until I complete the entire FCC curriculum.

The first thing you’ll learn is HTML basics. Most parts of this course are straightforward. But I suggest you understand the concepts by incorporating multiple learning materials other than Free Code Camp practice tests. Great resources include YouTube, Mozilla (MDN Web Docs), Udemy, Stack Overflow, and Frontend Mentor (for challenges). Remember, it’s about understanding the concepts, not just the syntax.

Most of the HTML concepts are easy to understand. The only area you are likely to face a little challenge is when creating forms and labels. You’ll learn about buttons, checkboxes, inputs, and attributes that make these elements work. Do not just rely on one source for this if you want to understand the concepts of forms.

On CSS, you will immediately realize that it relies heavily on HTML DOM, reinforcing your understanding of this markup language even further. The CSS ruleset will demand you learn how various selectors interact with HTML. Don’t be overwhelmed by the jargon; trust me, you’ll learn them with time.


There is a LOT to learn in CSS, especially about styling tables and lists. Do not skimp on this area.


Today I learned about the use of media query in CSS to change various aspects of a webpage following user interaction.
I also learned about the use of "pattern" attribute to force users to input specific content in input such as "tel".

When inputing pattern, the parenthesis indicate range while curly brackets limit the number of digits. maxlength attribute also includes spaces in the phone numbers as directed to the user.
For example, in pattern="[0-9]{4}[0-9]{3}[0-9]{3}" maxlength="10", [0-9] means only number from 0 to 9, while {4} means only four numbers can be used in this part. Please remember that in patterns, spaces or dashes between curly bracket and subsequent parenthesis also count! (eg pattern="[0-9]{4}-[0-9]{3}-[0-9]{3}" maxlength="10" will requires users to input even the dashes, but since the maxlegth in this case is 10, then the last two digits will not be allowed. Changing max digits to 12 is the only way to accomodate everything).

I have learned about using the autocomplete="off" feasture in the form element to prevent browsers from autocompleting inputs.




Today I have learned about the use of !important to override styles in CSS. While cascade, inline styles, and specifity rule always compete, using !important stops this competition to a specific value.

I have also learned about the use of CSS variables to help avoid repetition in styles and ensure that styles can be easily changed without seeking every property value. Variables are annotated as --variable:value;. For example, --desmond:blue;. If you want this variable to be used "globally," you must set it in the :root, which is the html element. For instance, 

:root{
--desmond-color:blue;
}
.


I have also learned that variables, when declared in rulesets, must have fallback value. eg

form{
background-color:  var(--desmond-color, green);
}

In this case, if the variable is misspelt, the fallback wiill be green.


Media quiries are powerful tools to help you define conditions for styles. for example:

@media (max-width: 35rem){
	img{
		width:9rem;
		border-radius:50%;
	}
}

This will set width to 9rem and border-radius to 50% if an element is within the width of 35rem.
