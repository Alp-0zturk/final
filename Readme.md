## Python documentation guide
1. Open the project you want to create a documentation
   Use cd /path/to/project to be in the project directory.
   
The folder structure should look like this in order to create python documentation from the project:

 - Tutorial <br />
| --->	 - Resources <br />
| &emsp; &emsp;	|---->	- object_one.py <br />
| &emsp; &emsp;	| &emsp; &emsp; &emsp;	class One(): <br />
| &emsp; &emsp;	| &emsp; &emsp; &emsp;	def __init__(self): <br />
| &emsp; &emsp;	| &emsp; &emsp; &emsp;	print(“object One”) <br />
| &emsp; &emsp; |<br />
| &emsp; &emsp;	|---->	- object_two.py <br />
| &emsp; &emsp;	| &emsp; &emsp; &emsp;	class Two(): <br />
| &emsp; &emsp;	| &emsp; &emsp; &emsp;	def __init__(self): <br />
| &emsp; &emsp;	| &emsp; &emsp; &emsp;	print(“object Two”) <br />
| &emsp; &emsp; |<br />
| &emsp; &emsp;	----->	- __init__.py <br />
| &emsp; &emsp;	&emsp; &emsp; &emsp; from resources.object_One import One <br />
| &emsp; &emsp;	&emsp; &emsp; &emsp; from resources.object_Two import Two <br />
| <br />
----->	- tutorial.py <br />
  &emsp; &emsp;	&emsp; &emsp; import Resources <br />
  &emsp; &emsp;	&emsp; &emsp; o = Resorces.One() <br />
  &emsp; &emsp;	&emsp; &emsp; t = Resources.Two()	<br />	
		
The folder structure example: https://github.com/lpwj/five_minutes_tutorials/tree/python_examples/sphinx_documentation/src <br />

2. Install sphinx to your workspace by using the command below:<br />
	for Mac:<br />

   		brew install sphinx-doc

   	for Linux:<br />

   		apt-get install python3-sphinx

4.
5. 
6. 

7.

8.


Python documentation tutorial video: https://www.youtube.com/watch?v=BWIrhgCAae0&list=PPSV

Sphinx official page: https://www.sphinx-doc.org/en/master/usage/installation.html
