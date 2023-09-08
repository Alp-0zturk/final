## Python documentation guide
1. 

The folder structure should look like this:

 - Tutorial <br />
| &emsp; &emsp;	 - Resources <br />
| &emsp; &emsp;	|---->	- object_one.py <br />
| &emsp; &emsp;	| &emsp;		class One(): <br />
| &emsp;	| &emsp;		def __init__(self): <br />
| &emsp;	| &emsp;		print(“object One”) <br />
| &emsp; |<br />
| &emsp;	|---->	- object_two.py <br />
| &emsp;	| &emsp;		class Two(): <br />
| &emsp;	| &emsp;		def __init__(self): <br />
| &emsp;	| &emsp;		print(“object Two”) <br />
| &emsp; |<br />
| &emsp;	----->	- __init__.py <br />
| &emsp;			from resources.object_One import One <br />
| &emsp;			from resources.object_Two import Two <br />
----->	- tutorial.py <br />
  &emsp;	import Resources <br />
  &emsp;	o = Resorces.One() <br />
  &emsp;	t = Resources.Two()		
		
The folder structure example: https://github.com/lpwj/five_minutes_tutorials/tree/python_examples/sphinx_documentation/src

2.

3.

4.


Python documentation tutorial video: https://www.youtube.com/watch?v=BWIrhgCAae0&list=PPSV

Sphinx official page: https://www.sphinx-doc.org/en/master/usage/installation.html
