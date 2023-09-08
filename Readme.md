## Python documentation guide
1. 

The folder structure should look like this:

 - Tutorial
|	 - Resources
|	|---->	- object_one.py
|	|		class One():
|	|		def __init__(self):
|	|		print(“object One”)
|       |
|	|---->	- object_two.py
|	|		class Two():
|	|		def __init__(self):
|	|		print(“object Two”)
|       |
|	----->	- __init__.py
|			from resources.object_One import One
|			from resources.object_Two import Two
----->	- tutorial.py
		import Resources
		o = Resorces.One()
		t = Resources.Two()		
		
The folder structure example: https://github.com/lpwj/five_minutes_tutorials/tree/python_examples/sphinx_documentation/src

2.

3.

4.


Python documentation tutorial video: https://www.youtube.com/watch?v=BWIrhgCAae0&list=PPSV

Sphinx official page: https://www.sphinx-doc.org/en/master/usage/installation.html
