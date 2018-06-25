# Robot-Framework-Quality-Checklist
The quality checklist of Robot Framework code
This checklist can be used in testing projects as a general identifier of quality.  It always depends on the context of testing, type of project and its requirements. It is suitable to customize the checklist based on the project’s requirements.


Functionality
	Tests serve their purpose. They test what is expected from them.
	Test scripts properly catches and evaluates the defect
	Test scripts contain suitable assertions linked to the tested element of functionality
	Result of test execution does not fail due to a defect not linked with the AUT
o	Error in a test script
o	Not properly chosen timeout
o	Unstable internet connection
o	Incompatible version of browser / webdriver
o	Error in test data (missing, wrong, obsolete, insufficient rights)
	Execution of automated tests helps in the whole area of testing. It could replace some manual tests
	Test script tests only one functionality

Maintainability
	Test script is not overly dependent on GUI changes
o	Does not contain absolute xpath
o	Not dependent on specific configuration, physical machine
o	Not using absolute system path for accessing the files
	Test script does not contain unused code
	There is a consistent form used throughout the whole testing project
o	Keyword names have one of the forms: infinitive, -ing form, 3rd person form
o	Each word in a keyword name is separated by space
o	Each word in a test case name is separated by space
o	Each word in a test set name (file name) is separated by underscore
o	For variables and arguments name use camelCase notation
	One language is used consistently throughout the testing project
	Test scripts should not contain sleep
o	Better to use wait instead - wait until element is (not) visible, wait until page (does not) contain(s), wait until keyword succeeds etc.

Clarity
	Test project is clearly structured
o	Contains folders Tests for test script, Resources for implementation of keywords, variables and Results for saving the results of test execution
o	Contains folders Libraries for user-defined libraries, Data for external source data needed for test execution (if applicable)
	Usage of suitable names – clear & simple
o	Test set (id, name of test set)
o	Test cases
o	Keywords
o	Variables
o	Arguments
	No repetition of code – DRY principle, usage of keywords instead
	Test set contains similar type of test cases
	Tests are logically structured
	Test case consists primarily of high-level keywords
	It should be clear what the test case is about, which keywords it uses to achieve the goal. These keywords should give a clear understanding about the whole process of test execution
	Code is visually aligned, uses suitable indentation
	None of the rows in code is too long – there is no need for horizontal scrolling
o	Separate the row using “…”
	New members of the team are capable to quickly adapt to the project and can create the test scripts based on the keywords

Reusability
	It is possible to reuse the keywords in various tests
	Keywords use suitable arguments to make them reusable
	Keywords are independent from each other
o	Simple change in one keyword does not affect the others

Documentation
	Test set can contain documentation
o	Documentation does not only restate the name of the set
o	It should give new information
o	For simple test sets the documentation is not necessary
	Test cases do not need a documentation
o	It is better to use [Tags] instead
	Keywords do not need a documentation
o	Their functionality should be that simple so it’s clear and straight-forward from the name

Comments
	Test scripts do not contain comments describing the functionality (of test case, keyword)
o	Try to simplify instead, divide into smaller & simpler parts
o	Choosing a better & more precise naming
	It is clear to which part of the code a comment belongs
	Test scripts do not contain obsolete comments
	Comments are clear, simple and short

