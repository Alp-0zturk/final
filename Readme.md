## Python documentation guide
1. 

The folder structure should look like this:

 - Tutorial <br />
|&nbsp;	 - Resources <br />
|&nbsp;	|---->	- object_one.py <br />
|&nbsp;	|		class One(): <br />
|&nbsp;	|		def __init__(self): <br />
|&nbsp;	|		print(“object One”) <br />
|       |<br />
|	|---->	- object_two.py <br />
|	|		class Two(): <br />
|	|		def __init__(self): <br />
|	|		print(“object Two”) <br />
|       |<br />
|	----->	- __init__.py <br />
|			from resources.object_One import One <br />
|			from resources.object_Two import Two <br />
----->	- tutorial.py <br />
		import Resources <br />
		o = Resorces.One() <br />
		t = Resources.Two()		
		
The folder structure example: https://github.com/lpwj/five_minutes_tutorials/tree/python_examples/sphinx_documentation/src

2.

3.

4.


Python documentation tutorial video: https://www.youtube.com/watch?v=BWIrhgCAae0&list=PPSV

Sphinx official page: https://www.sphinx-doc.org/en/master/usage/installation.html
