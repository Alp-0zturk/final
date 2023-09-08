## Python documentation guide
1. Open the project you want to create a documentation <br />
   Use cd /path/to/project to be in the project directory. <br />
   
The folder structure should look like this in order to create python documentation from the project: <br />

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

3. Create docs folder under the main project folder by using mkdir docs command <br />
	
4. Go to docs directory and use sphinx-quickstart command to create a documentation base. <br />
	- After executing the command it will ask you project name, author name and version. <br />
 
5. Create __init__.py file for all subfolders that have python code that you want to document. <br />

6. Go back to the project folder by using "cd .." command and then use the command below to create .rst (reStructuredText files for python files)<br />

		sphinx-apidoc -o docs .
  > with this command .rst files will be created under the docs folder. <br />
  > reStructuredText (RST, ReST, or reST) is a file format for textual data used primarily in the Python programming language community for technical documentation.

7. After .rst files have been created open conf.py file and change the code by adding  <br />
	
 		import os
		import sys
		sys.path.insert(0, os.path.abspath(".."))
	- And add these codes below to create documentation succesfully and add a theme to the created .html documentation files. <br />

  			extensions = ["sphinx.ext.todo", "sphinx.ext.viewcode", "sphinx.ext.autodoc"]

			html_theme = 'sphinx_rtd_theme'
			html_static_path = ['_static']
9. Go to index.rst file and type modules to include modules (subfolders that are going to be documented to .html) like in the example below: <br />
   			.. toctree:: <br />
   			:maxdepth: 2 <br />
   			:caption: Contents: <br />

      			modules

10. 

# Debugging, finding errors

To find files that cause error you can create the docs subfolder inside project modules and generate documentation for each project subfolder.

Python documentation tutorial video: https://www.youtube.com/watch?v=BWIrhgCAae0&list=PPSV

Sphinx official page: https://www.sphinx-doc.org/en/master/usage/installation.html
