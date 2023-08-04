# Comparing `tmp/pqinput-0.0.409.tar.gz` & `tmp/pqinput-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqinput-0.0.409.tar", last modified: Fri Aug  4 11:09:12 2023, max compression
+gzip compressed data, was "pqinput-0.0.5.tar", last modified: Mon Jul  3 16:40:09 2023, max compression
```

## Comparing `pqinput-0.0.409.tar` & `pqinput-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-08-04 11:09:12.271068 pqinput-0.0.409/
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     1075 2023-08-04 10:44:06.000000 pqinput-0.0.409/LICENSE.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     3887 2023-08-04 11:09:12.271068 pqinput-0.0.409/PKG-INFO
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     3314 2023-08-04 10:44:06.000000 pqinput-0.0.409/README.md
-drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-08-04 11:09:12.267068 pqinput-0.0.409/pqinput/
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      106 2023-08-04 10:44:06.000000 pqinput-0.0.409/pqinput/__init__.py
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     6695 2023-08-04 10:44:06.000000 pqinput-0.0.409/pqinput/drawPES.py
--rw-rw-r--   0 lubo      (1000) lubo      (1000)    16719 2023-08-04 10:44:06.000000 pqinput-0.0.409/pqinput/inpxml.py
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     4819 2023-08-04 11:07:11.000000 pqinput-0.0.409/pqinput/propagation_dicts.py
-drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-08-04 11:09:12.267068 pqinput-0.0.409/pqinput.egg-info/
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     3887 2023-08-04 11:09:12.000000 pqinput-0.0.409/pqinput.egg-info/PKG-INFO
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      255 2023-08-04 11:09:12.000000 pqinput-0.0.409/pqinput.egg-info/SOURCES.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)        1 2023-08-04 11:09:12.000000 pqinput-0.0.409/pqinput.egg-info/dependency_links.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)        8 2023-08-04 11:09:12.000000 pqinput-0.0.409/pqinput.egg-info/top_level.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      542 2023-08-04 11:07:51.000000 pqinput-0.0.409/pyproject.toml
--rw-rw-r--   0 lubo      (1000) lubo      (1000)       38 2023-08-04 11:09:12.271068 pqinput-0.0.409/setup.cfg
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      653 2023-08-04 11:08:04.000000 pqinput-0.0.409/setup.py
+drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-03 16:40:09.408741 pqinput-0.0.5/
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.5/LICENSE.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     3885 2023-07-03 16:40:09.408741 pqinput-0.0.5/PKG-INFO
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     3314 2023-05-09 09:41:50.000000 pqinput-0.0.5/README.md
+drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-03 16:40:09.408741 pqinput-0.0.5/pqinput/
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      134 2023-05-03 12:56:50.000000 pqinput-0.0.5/pqinput/__init__ (conflicted copy 2023-05-03 145650).py
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      106 2023-05-09 11:00:00.000000 pqinput-0.0.5/pqinput/__init__.py
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     8672 2023-05-11 13:17:09.000000 pqinput-0.0.5/pqinput/drawPES.py
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)    12777 2023-05-03 14:39:36.000000 pqinput-0.0.5/pqinput/inpxml (conflicted copy 2023-05-03 163936).py
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)    15598 2023-07-03 16:30:51.000000 pqinput-0.0.5/pqinput/inpxml.py
+drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-07-03 16:40:09.408741 pqinput-0.0.5/pqinput.egg-info/
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     3885 2023-07-03 16:40:09.000000 pqinput-0.0.5/pqinput.egg-info/PKG-INFO
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      336 2023-07-03 16:40:09.000000 pqinput-0.0.5/pqinput.egg-info/SOURCES.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)        1 2023-07-03 16:40:09.000000 pqinput-0.0.5/pqinput.egg-info/dependency_links.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)        8 2023-07-03 16:40:09.000000 pqinput-0.0.5/pqinput.egg-info/top_level.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      540 2023-07-03 16:39:30.000000 pqinput-0.0.5/pyproject.toml
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)       38 2023-07-03 16:40:09.408741 pqinput-0.0.5/setup.cfg
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      651 2023-07-03 16:39:40.000000 pqinput-0.0.5/setup.py
```

### Comparing `pqinput-0.0.409/LICENSE.txt` & `pqinput-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.409/PKG-INFO` & `pqinput-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.409
+Version: 0.0.5
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
```

### Comparing `pqinput-0.0.409/README.md` & `pqinput-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.409/pqinput/drawPES.py` & `pqinput-0.0.5/pqinput/drawPES.py`

 * *Files 18% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     except:
         c = color
     c = np.array(colorsys.rgb_to_hls(*mc.to_rgb(c)))
     return colorsys.hls_to_rgb(c[0],1-amount * (1-c[1]),c[2])
 
 def plotPES(inxstc, savename=None, SIunits=True, yrange=None, xrange=None, 
 legend=None, showfig=None, showWF=True, offset_overlap=0.5, sizex=12/2.54, sizey=8/2.54,
-title=None, offsetlabel=None, drawpure=True): # inx structure
+title=None, offsetlabel=None): # inx structure
     
     
     fig, ax = plt.subplots(layout='constrained', figsize=(sizex, sizey))
     plt.rcParams.update({'font.size': 10})
     
     cmap = plt.get_cmap("tab10")
     potmin = 0
@@ -93,15 +93,15 @@
                 dim = meta['dim'][0]
                 x = np.linspace(dim.xmin, dim.xmax, dim.size)
                 
             '''PES plotting, if there is a offset (photon energy) the line is dashed'''
             ################# main plot #################
             ax.plot(x, Pot*(HEeV if SIunits else 1), 
                     color=(cmap(j) if not offset else lighter(cmap(j),.5) ), 
-                    linestyle=('-' if not offset else ' ' if not drawpure else '--') ,
+                    linestyle=('-' if not offset else '--') ,
             # label=(re.findall('([\d]+)', element.tag)[0] if not offset else '_nolegend_') )
             label=(element.get('label') if not offset else '_nolegend_') )
     
             '''If the state PES has a photonic contribution'''
             if offset: 
                 homega = float(offset)*HEeV/sec2au*f2En
                 
@@ -160,15 +160,48 @@
     if savename: plt.savefig(savename) 
     [plt.close() if not showfig else plt.show()]
     
     
     return fig, ax
 # %%
 if __name__=='__main__':
-    import inpxml as inx   
-    prop = inx.InpXML()   
-    prop.readInput('2states-wf1.Sig0.1.xml')
+    import pqinput.inpxml as inx
+    home = '/home/lucas/mntcluster/QDng'
+    mass = 12500
+    propapar = {'dt': 4.138276,'steps': 1000,'wcycle': 100,'dir': 'propa_files','nfile': 'norm'}
+    # Kinect energy operators
+    T_CO = {'head':'T', 'name':"GridNablaSq", 'mass':mass, 'key':'T'}
+    Tref = {'head':'T','ref':'T'}
+    # Potential energy surfaces
+    Vg = {'head':'V', 'name':"GridPotential", 'file': home + '/CO/pots/pot_VSp'}
+    Ve = {'head':'V', 'name':"GridPotential", 'file': home + '/CO/pots/pot_VPx'}
+    Vgl = {'head':'V', 'name':"GridPotential", 'file': home + '/CO/pots/pot_VSp', 'offset':0.05}
+    Vgr = {'head':'V', 'name':"GridPotential", 'file': home + '/CO/pots/pot_VPx', 'offset':0.05}
+    # Diagonal terms: pure states
+    G00 = {'head':'m0.0', 'name':'Sum', 'Opes':[T_CO, Vg]}
+    E00 = {'head':'m1.1', 'name':'Sum', 'Opes':[Tref, Ve]}
+    G01 = {'head':'m2.2', 'name':'Sum', 'Opes':[Tref, Vgl]}
+    G10 = {'head':'m3.3', 'name':'Sum', 'Opes':[Tref, Vgr]}
+    # Off diagonal terms: interactions
+    las =  {'head':'m0.1', 'name':'GridDipole', 'file': home + '/CO/mu/mu', 'laser':'Et', 'Opes':[]}
+    dipl = {'head':'m2.1', 'name':'GridPotential', 'file': home + '/CO/mu/mu', 'scale':0.01, 'Opes':[]}    
+    dipr = {'head':'m3.1', 'name':'GridPotential', 'file': home + '/CO/mu/mu', 'scale':0.01, 'Opes':[]}
+    # Hamiltonian dictionary
+    Hparams = {'type':'Multistate', 'Mels':[G00, E00, G01, G10, las, dipl, dipr]} 
+    # Initial state
+    iwf, ef = [1, ], [[0, ],['Sigmap',]]
+    WFpar = {'type':'Multistate', 'states':4, 'label':'$\\psi_0$',
+             'file':[ home + "/CO/efs_{}/ef_{}".format(ef[1][i], ef[0][i]) for i in range(len(ef[0]))], 
+             'index':[iwf[i] for i in range(len(iwf))], 'normalize':True}
+    filteropes = [{'expeconly':{'name':'Multistate', 'states':'4', 'unity':'False', 'header':"mu{}".format(ind)}, 
+                   'm{}'.format(ind):{'name':'GridPotential', 'file':'../CO/mu/mu'}}
+                   for ind in [2.1, 2.3, 3.1] ]
+    
+    prop = inx.InpXML()
+    prop.program('propa', propapar, WFpar)
+    prop.propagation('Cheby', Hparams)
     #%%
-    prop.show
+    
+    # prop.show
     #legend=['G','E','Gl','Gr',],
-    plotPES(prop, yrange=(0,10), xrange=(1.1,4.5), 
+    plotPES(prop, yrange=(0,20), xrange=(1.5,5), 
             offsetlabel=['wx', 'wy'], showfig=True)
```

### Comparing `pqinput-0.0.409/pqinput/inpxml.py` & `pqinput-0.0.5/pqinput/inpxml.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,18 +110,18 @@
         show: prints out the class text in readable xml format
         
         
     * comments from QDng documentation
     """
     # Attributes as properties
     qdng = typed_property('qdng')
-    mainprogram = typed_property('mainprogram')    
-    wavefunction = typed_property('wavefunction')
-    propagator = typed_property('propagator')
-    hamiltonian = typed_property('hamiltonian')
+    prog = typed_property('program')    
+    wavefunc = typed_property('wavefunction')
+    propag = typed_property('propagation')
+    hamilt = typed_property('hamiltonian')
     filterpost = typed_property('filterpost')
     # Defined operations and programs so far
     
     def __init__(self, qdng_params=None): # Initiate the input layout 
         self._qdng = et.Element("qdng") 
         # Root of the XML tree: self._qdng, with the tag-headline 
         if qdng_params: dict2attr(self._qdng, qdng_params)
@@ -133,30 +133,15 @@
         return f'{et.tostring(self._qdng, pretty_print=True).decode()}'    
     
     @property
     def show(self): # printing property
         '''Print out the full text in readable xml format
         Useful for debugging '''
         print(self)    
-        
-    def readInput(self, path):
-        '''Read an input file to generate a InpXML class object'''
-        ' reading an input file will overwrite a InpXML object with the attributes and text'
-        inp = et.parse(path)
-        tags = [element.tag for element in inp.iter()]
-        tree = [element for element in inp.iter()]
-        
-        # Couldnt find a better way to direct the element to the attributes, can use string for variable name...
-        self._qdng = inp.getroot()
-        self._mainprogram = (tree[tags.index('propa')] if 'propa' in tags else None)
-        self._propagator = (tree[tags.index('propagator')] if 'propagator' in tags else None)
-        self._hamiltonian = (tree[tags.index('hamiltonian')] if 'hamiltonian' in tags else None)
-        self._filterpost = (tree[tags.index('filterpost')] if 'filterpost' in tags else None)
-        self._wavefunction = (tree[tags.index('wf')] if 'wf' in tags else None)
-        
+
 # %% 
     ''' METHODS '''
     ######################## Write file ########################
     def writexml(self, file_name='test_file', txt=False):
         """ Write the constructed lxml element to a XML file. """
         tree = et.ElementTree(self._qdng)
         if file_name.endswith('.txt'): 
@@ -206,16 +191,16 @@
             _format: {'dt':num, 'steps':num, 'directory':str,'Nef':num, 'conv':num }
             wf_parameters (dict) wavefunction parameters dictionary:
             _format: {'name':str, 'states':num, 'file':[strs, ], 'normalize':True or None}
             
         """
         '''MAIN PROGRAM'''
         if not ptype in ['propa','eigen']: raise SyntaxError('Program not defined.')  
-        self._mainprogram = subelem(self._qdng, program_parameters, ptype )
-        # Create self._mainprogram as a lxml elem element of qdng
+        self._program = subelem(self._qdng, program_parameters, ptype )
+        # Create self._program as a lxml elem element of qdng
         '''WAVEFUNCTION'''
         self.define_wavefunction(wf_parameters)
         # define wavefunction parameters    
     
     # %% 
     """ Operators """
     def dict2ope(self, d, head=None, text_mode=False):
@@ -252,15 +237,15 @@
                 if 'Multistate' in child.values(): child['states'] = str(self.states)
                 # append a child from an dictionary
                 xml.append(self.dict2ope(child))
                 
         return et.tostring(xml) if text_mode else xml
     
     def def_hamiltonian(self, Hp):    
-        Hel = et.SubElement(self._propagator, 'hamiltonian')
+        Hel = et.SubElement(self._propagation, 'hamiltonian')
         # Create a lxml element to be appended to the self.propag 
         if Hp['type'] == 'Sum': 
             Hel.set('name', Hp['type'])
             [subelem(Hel, elem) for elem in Hp['heir']]
             self.states = 1
             # set hamiltonian of Sum type, creating subelements for each operator
         elif Hp['type'] == 'Multistate':
@@ -281,62 +266,61 @@
                     # if 'heir' in  mel.keys():
                     #     for ind in range(len(mel['heir'])):
                     #         branch.append( self.dict2ope(mel['heir'][ind])) 
         self._hamiltonian = Hel            
         
     # %% 
     ''' Propagator '''
-    def propagation(self, name, hamilt_params, attrib=None):
+    def propagation(self, name, hamilt_params):
         """ Method for the wavefunction propagation. Return a etree.SubElement of previous defined program.
         
         Args:
             name (string) name of the propagation method:
-                *GSPO, Cheby, *SIL, Arnoldi (*not defined yet)
+                *GSPO, Cheby, *SIL, *Arnoldi (*not defined yet)
             hamilt_params (dict) parameters dictionary for the required Cheby hamiltonian
             _format: {'type':hamiltonian type, 'Matrix_elems':[mij, ]} 
             _type in ('Sum', 'Multistate', )
             _matrix elements for multistate, see hamilt_elem() function for format
             
         """
-        # Propagator
-        if name in ['Cheby', 'Arnoldi']:# requires hamiltonian
+        # Chebychev propagator
+        if name == 'Cheby':# requires hamiltonian
             # create the propagator subelement of the program
-            self._propagator = et.SubElement(self._mainprogram, 'propagator', name=name,
-                                              attrib=attrib)
+            self._propagation = et.SubElement(self._program, 'propagator', name=name)
             self.def_hamiltonian(hamilt_params)
             # define hamiltonian 
             self._wavefunction.set('states', str(self.states))
             # change wavefunction states based on hamiltonian matrix
         else:
             raise SyntaxError('Propagator type not defined.')
         # others propagators
         try:
-            self._mainprogram.append( self._wavefunction ) # append wavefunction after the propagation
+            self._program.append( self._wavefunction ) # append wavefunction after the propagation
         except:
             raise SyntaxError('Wavefunction was not properly defined for propa.')    
     
     def filter(self, filter_type, filter_list, options=None):
         # types of filter to add
         def def_filterpost(filter_list):
             # Define the filterpost operation, called after propagation
             filterpost = et.Element('filterpost')
             if not isinstance(filter_list, list): filter_list = [filter_list]
             for dic in filter_list:
                 
                 filterpost.append(self.dict2ope(dic))
             # add operators at the filter list with heir children through dict2ope function
             
-            self._mainprogram.append(filterpost)
+            self._program.append(filterpost)
             return filterpost
         
         # add filter to calculation
         if filter_type == 'filterpost':
             self._filterpost = def_filterpost(filter_list)    
 
-    
+        
 # %% Name == Main 
 if __name__ == "__main__":
     
     Tf = 25 # [fs]
     dt = 0.25 # [fs]
     steps = Tf*41.34/dt
     Nfiles = 5e2
@@ -375,16 +359,15 @@
     #%%
     # Initialize
     prop = InpXML()
     prop.program('propa', propa_params, WF_params)
     prop.propagation('Cheby', Hsum)
     prop.filter('filterpost', filter_elem)
     prop.show
-    prop.readInput('2states-wf1.Sig0.1.xml')
-    prop.show
+
     # Editing
     # prop.hamilt = 'name', 'something'
     # prop.hamilt = 'm0.0/T', 'name', 'something_new'
     # prop.show
     
 
     # prop.plotPES(showfig=True)
```

### Comparing `pqinput-0.0.409/pqinput.egg-info/PKG-INFO` & `pqinput-0.0.5/pqinput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.409
+Version: 0.0.5
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
```

### Comparing `pqinput-0.0.409/pyproject.toml` & `pqinput-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pqinput"
-version = "0.0.409"
+version = "0.0.5"
 authors = [
   { name="Lucas Borges", email="lucas.borges@fysik.su.se" },
 ]
 description = "Create input files for QDng calculations"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pqinput-0.0.409/setup.py` & `pqinput-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setuptools.setup(
     name = "pqinput",
-    version = "0.0.409",
+    version = "0.0.5",
     author = "Lucas Borges",
     author_email = "lucas.borges@fysik.su.se",
     description = ("additional functions for QDng calculations setups."),
     license = "MIT",
     keywords = "qdng",
     url = "https://gitlab.fysik.su.se/lucas.borges/inputxml",
     packages=setuptools.find_packages(),
```

