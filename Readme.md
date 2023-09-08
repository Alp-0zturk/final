## Python documentation guide
1. 

The folder structure should look like this:

 - Tutorial <br />
|&ebsp;	 - Resources <br />
|&ebsp;	|---->	- object_one.py <br />
|&ebsp;	|&ebsp;		class One(): <br />
|&ebsp;	|&ebsp;		def __init__(self): <br />
|&ebsp;	|&ebsp;		print(“object One”) <br />
|&ebsp; |<br />
|&ebsp;	|---->	- object_two.py <br />
|&ebsp;	|&ebsp;		class Two(): <br />
|&ebsp;	|&ebsp;		def __init__(self): <br />
|&ebsp;	|&ebsp;		print(“object Two”) <br />
|&ebsp; |<br />
|&ebsp;	----->	- __init__.py <br />
|&ebsp;			from resources.object_One import One <br />
|&ebsp;			from resources.object_Two import Two <br />
----->	- tutorial.py <br />
	&ebsp;	import Resources <br />
	&ebsp;	o = Resorces.One() <br />
	&ebsp;	t = Resources.Two()		
		
The folder structure example: https://github.com/lpwj/five_minutes_tutorials/tree/python_examples/sphinx_documentation/src

2.

3.

4.


Python documentation tutorial video: https://www.youtube.com/watch?v=BWIrhgCAae0&list=PPSV

Sphinx official page: https://www.sphinx-doc.org/en/master/usage/installation.html
