# Tableau_Python_Integration
We have used Tableau 10.3 and Python 3.6 


Tableau Integration with Python - Step by Step

What is Python
•	Python is a widely used general-purpose programming language, popular among academia and industry alike.
•	It provides a wide variety of statistical and machine learning techniques and is highly extensible.
•	Together, Python and Tableau is the data science dream team to cover any organization’s data analysis needs.
•	In 2013 Tableau introduced the R Integration [since Tableau 8.1], the ability to call R scripts in calculated fields using R Server [ Rserve()].
•	With the release of Tableau 10.1, you can use Python scripts as part of your calculated fields in Tableau, just as you’ve been able to do with R. I have used Tableau 10.3 professional Edition and Python 3.6. 
•	The Python Integration happens through the Tableau Python Server - [TabPy].

Install tableau python server: TabPy
•	You can Download TabPy from the Link : GitHub - tableau/TabPy: Execute Python code on the fly and display results in Tableau visualizations
•	Click on the Clone or download button in the upper right corner ( see below ) of the TabPy repository page, downloading the zip file and extracting it.
Extract TabPy-master.zip
•	Within the TabPy-master directory, execute setup.bat (or setup.sh if you are on Mac).
•	This script downloads and installs Python, TabPy and all necessary dependencies.
•	After completion, TabPy starts up and listens on port 9004.
•	Open Tableau and use Superstore dataset. 
•	Help > Settings and Performance > Manage External Service Connection..
•	Select TabPy/External API
 

•	With this message we have successfully setup the TabPy and Tableau.
•	  State and Sum (Profit) sheet. But now we want to identify states with profit (+). 
•	We have use SCRIPT_BOOL, which return True if the value of that column is positive otherwise False.

•	 Drag State field to rows.

•	Add SUM(profit) to columns.
•	Drag New Created Profitable_state field to Marks – Color.

•	 Click on Hide Mark label for more text details
 
•	Replace according field to sheet if you want need color according to range.
