# i am getting this error while i run my code which consists of resipy package. Can anyone help me to get work.

---------------------------------------------------------------------------
ImportError                               Traceback (most recent call last)
File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\resipy\meshTools.py:38
     37 try: 
---> 38     from resipy.cext import meshCalc as mc 
     39 except Exception as e:

ImportError: cannot import name 'meshCalc' from 'resipy.cext' (unknown location)

During handling of the above exception, another exception occurred:

Exception                                 Traceback (most recent call last)
Cell In[2], line 9
      7 import os
      8 import time
----> 9 from resipy import R2
     11 no_of_model_runs = 1
     12 tic = time.time()

File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\resipy\__init__.py:2
      1 name = "resipy"
----> 2 from resipy.Project import ResIPy_version, sysinfo
      3 from resipy.Project import Project, R2
      4 from resipy.Survey import Survey

File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\resipy\Project.py:40
     38 from resipy.parsers import geomParser
     39 from resipy.r2in import write2in
---> 40 import resipy.meshTools as mt
     41 from resipy.meshTools import cropSurface
     42 from resipy.template import startAnmt, endAnmt

File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\resipy\meshTools.py:42
     40     print('Could not import meshCalc extension see the following error:')
     41     print(e)# meshCalc needs to be compiled 
---> 42     raise Exception('Could not import meshCalc extension to fix the problem try, '\
     43                     'updating ResIPy, updating Numpy or recompiling the extension.')
     45 # import pyvista if available
     46 try:

Exception: Could not import meshCalc extension to fix the problem try, updating ResIPy, updating Numpy or recompiling the extension.
