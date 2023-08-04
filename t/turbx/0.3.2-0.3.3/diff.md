# Comparing `tmp/turbx-0.3.2.tar.gz` & `tmp/turbx-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbx-0.3.2.tar", last modified: Wed Jun 28 20:06:58 2023, max compression
+gzip compressed data, was "turbx-0.3.3.tar", last modified: Fri Aug  4 15:40:14 2023, max compression
```

## Comparing `turbx-0.3.2.tar` & `turbx-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-28 20:06:58.067022 turbx-0.3.2/
--rwxrwxr-x   0 jason     (1000) jason     (1000)     1065 2022-06-30 12:13:09.000000 turbx-0.3.2/LICENSE
--rw-rw-r--   0 jason     (1000) jason     (1000)     2353 2023-06-28 20:06:58.067022 turbx-0.3.2/PKG-INFO
--rwxrwxr-x   0 jason     (1000) jason     (1000)     1072 2023-04-15 18:45:25.000000 turbx-0.3.2/README.md
--rw-rw-r--   0 jason     (1000) jason     (1000)       38 2023-06-28 20:06:58.067022 turbx-0.3.2/setup.cfg
--rwxrwxr-x   0 jason     (1000) jason     (1000)     2295 2023-06-28 20:00:16.000000 turbx-0.3.2/setup.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-28 20:06:58.067022 turbx-0.3.2/turbx/
--rwxrwxr-x   0 jason     (1000) jason     (1000)     3260 2023-06-28 19:59:17.000000 turbx-0.3.2/turbx/__init__.py
--rwxrwxr-x   0 jason     (1000) jason     (1000)  1255673 2023-06-28 19:59:04.000000 turbx-0.3.2/turbx/turbx.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-28 20:06:58.067022 turbx-0.3.2/turbx.egg-info/
--rw-rw-r--   0 jason     (1000) jason     (1000)     2353 2023-06-28 20:06:58.000000 turbx-0.3.2/turbx.egg-info/PKG-INFO
--rw-rw-r--   0 jason     (1000) jason     (1000)      203 2023-06-28 20:06:58.000000 turbx-0.3.2/turbx.egg-info/SOURCES.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)        1 2023-06-28 20:06:58.000000 turbx-0.3.2/turbx.egg-info/dependency_links.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)      143 2023-06-28 20:06:58.000000 turbx-0.3.2/turbx.egg-info/requires.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)        6 2023-06-28 20:06:58.000000 turbx-0.3.2/turbx.egg-info/top_level.txt
+drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-08-04 15:40:14.489992 turbx-0.3.3/
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1065 2022-06-30 12:13:09.000000 turbx-0.3.3/LICENSE
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)     2353 2023-08-04 15:40:14.489992 turbx-0.3.3/PKG-INFO
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1072 2023-04-15 18:45:25.000000 turbx-0.3.3/README.md
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)       38 2023-08-04 15:40:14.489992 turbx-0.3.3/setup.cfg
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     2295 2023-08-04 15:37:59.000000 turbx-0.3.3/setup.py
+drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-08-04 15:40:14.489992 turbx-0.3.3/turbx/
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     3335 2023-08-04 15:37:17.000000 turbx-0.3.3/turbx/__init__.py
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)  1321879 2023-08-04 15:35:23.000000 turbx-0.3.3/turbx/turbx.py
+drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-08-04 15:40:14.489992 turbx-0.3.3/turbx.egg-info/
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)     2353 2023-08-04 15:40:14.000000 turbx-0.3.3/turbx.egg-info/PKG-INFO
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)      203 2023-08-04 15:40:14.000000 turbx-0.3.3/turbx.egg-info/SOURCES.txt
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)        1 2023-08-04 15:40:14.000000 turbx-0.3.3/turbx.egg-info/dependency_links.txt
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)      143 2023-08-04 15:40:14.000000 turbx-0.3.3/turbx.egg-info/requires.txt
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)        6 2023-08-04 15:40:14.000000 turbx-0.3.3/turbx.egg-info/top_level.txt
```

### Comparing `turbx-0.3.2/LICENSE` & `turbx-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `turbx-0.3.2/PKG-INFO` & `turbx-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbx
-Version: 0.3.2
+Version: 0.3.3
 Summary: Extensible toolkit for analyzing turbulent flow datasets
 Home-page: https://github.com/iagappel/turbx
 Author: Jason A
 Maintainer: Jason A
 License: MIT
 Keywords: scientific computing,statistics,simulation,turbulence,turbulent flows,direct numerical simulation,DNS,parallel,visualization
 Platform: any
```

### Comparing `turbx-0.3.2/README.md` & `turbx-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `turbx-0.3.2/setup.py` & `turbx-0.3.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='turbx',
-    version='0.3.2',
+    version='0.3.3',
     description='Extensible toolkit for analyzing turbulent flow datasets',
     
     long_description=long_description,
     long_description_content_type='text/markdown',
     
     url='https://github.com/iagappel/turbx',
     author='Jason A',
```

### Comparing `turbx-0.3.2/turbx/__init__.py` & `turbx-0.3.3/turbx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 turbx
 
 Extensible toolkit for analyzing turbulent flow datasets
 '''
 
-__version__ = '0.3.2'
+__version__ = '0.3.3'
 __author__ = 'Jason A'
 
 from .turbx import cgd
 from .turbx import rgd
 from .turbx import eas4
 from .turbx import ztmd
 from .turbx import lpd
@@ -61,14 +61,15 @@
 from .turbx import get_Lch_colors
 from .turbx import hex2rgb
 from .turbx import hsv_adjust_hex
 from .turbx import analytical_u_plus_y_plus
 from .turbx import nice_log_labels
 from .turbx import fig_trim_y
 from .turbx import fig_trim_x
+from .turbx import axs_grid_initializer
 from .turbx import axs_grid_compress
 from .turbx import tight_layout_helper_ax_with_cbar
 from .turbx import cmap_convert_mpl_to_pview
 
 __all__ = ['cgd',
            'rgd',
            'eas4',
@@ -112,10 +113,11 @@
            'get_Lch_colors',
            'hex2rgb',
            'hsv_adjust_hex',
            'analytical_u_plus_y_plus',
            'nice_log_labels',
            'fig_trim_y',
            'fig_trim_x',
+           'axs_grid_initializer',
            'axs_grid_compress',
            'tight_layout_helper_ax_with_cbar',
            'cmap_convert_mpl_to_pview' ]
```

### Comparing `turbx-0.3.2/turbx/turbx.py` & `turbx-0.3.3/turbx/turbx.py`

 * *Files 2% similar despite different names*

```diff
@@ -10441,14 +10441,15 @@
                         
                         chunk_kb_ = np.prod(dset.chunks)*float_bytes / 1024. ## actual
                         if verbose:
                             even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
                             even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
                 
                 if favre:
+                    
                     if (scalar in scalars_fv):
                         if ('data/%s_fv'%scalar in hf_mean):
                             del hf_mean['data/%s_fv'%scalar]
                         if verbose:
                             even_print( f'initializing data/{scalar}_fv' , f'{data_gb_mean:0.3f} [GB]' )
                         dset = hf_mean.create_dataset(f'data/{scalar}_fv',
                                                       shape=shape,
@@ -11605,14 +11606,20 @@
                                 pass
                                 
                                 if verbose: progress_bar.update()
                         
                         if self.usingmpi: self.comm.Barrier()
                         if hf_prime.usingmpi: comm_rgd_prime.Barrier()
                         if hf_mean.usingmpi: comm_rgd_mean.Barrier()
+                    
+                    ## report mem free
+                    mem_avail_gb = psutil.virtual_memory().available/1024**3
+                    mem_free_gb  = psutil.virtual_memory().free/1024**3
+                    if verbose:
+                        tqdm.write(even_print('mem free', '%0.1f [GB]'%mem_free_gb, s=True))
                 
                 if verbose:
                     progress_bar.close()
             
             # === replace dims/t array in prime file (if ti_min was given)
             if (ti_min is not None):
                 t = np.copy( self.t[ti_min:] )
@@ -19088,14 +19095,20 @@
         if ('dz' in self.attrs.keys()):
             self.dz = self.attrs['dz']
         
         if ('dims/stang' in self):
             self.stang = np.copy( self['dims/stang'][()] )
         if ('dims/snorm' in self):
             self.snorm = np.copy( self['dims/snorm'][()] )
+        
+        if ('csys/vtang' in self):
+            self.vtang = np.copy( self['csys/vtang'][()] )
+        if ('csys/vnorm' in self):
+            self.vnorm = np.copy( self['csys/vnorm'][()] )
+        
         if ('dims/crv_R' in self):
             self.crv_R = np.copy( self['dims/crv_R'][()] )
         if ('dims/R_min' in self):
             self.R_min = self['dims/R_min'][()]
         
         if verbose: print(72*'-')
         if verbose and hasattr(self,'duration_avg'): even_print('duration_avg', '%0.5f'%self.duration_avg)
@@ -19367,28 +19380,31 @@
                 w   = np.copy( data_mean['w']   ) * U_inf
                 rho = np.copy( data_mean['rho'] ) * rho_inf
                 p   = np.copy( data_mean['p']   ) * (rho_inf * U_inf**2)
                 T   = np.copy( data_mean['T']   ) * T_inf
                 mu  = np.copy( data_mean['mu']  ) * mu_inf
                 data_mean = None; del data_mean
                 
+                
+                ## derived values from base scalars
                 a     = np.sqrt( kappa * R * T )
                 nu    = mu / rho
                 umag  = np.sqrt( u**2 + v**2 + w**2 )
                 M     = umag / np.sqrt(kappa * R * T)
                 mflux = umag * rho
                 
                 ## base scalars [u,v,w,ρ,p,T]
                 dset = self.create_dataset('data/u'   , data=u.T   , chunks=None)
                 dset = self.create_dataset('data/v'   , data=v.T   , chunks=None)
                 dset = self.create_dataset('data/w'   , data=w.T   , chunks=None)
                 dset = self.create_dataset('data/rho' , data=rho.T , chunks=None)
                 dset = self.create_dataset('data/p'   , data=p.T   , chunks=None)
                 dset = self.create_dataset('data/T'   , data=T.T   , chunks=None)
-                ##
+                
+                ## derived fields
                 dset = self.create_dataset('data/a'     , data=a.T     , chunks=None) #; dset.attrs['dimensional'] = True  ; dset.attrs['unit'] = '[m/s]'
                 dset = self.create_dataset('data/mu'    , data=mu.T    , chunks=None) #; dset.attrs['dimensional'] = True  ; dset.attrs['unit'] = '[kg/(m·s)]'
                 dset = self.create_dataset('data/nu'    , data=nu.T    , chunks=None) #; dset.attrs['dimensional'] = True  ; dset.attrs['unit'] = '[m²/s]'
                 dset = self.create_dataset('data/umag'  , data=umag.T  , chunks=None) #; dset.attrs['dimensional'] = True  ; dset.attrs['unit'] = '[m/s]'
                 dset = self.create_dataset('data/M'     , data=M.T     , chunks=None) #; dset.attrs['dimensional'] = False
                 dset = self.create_dataset('data/mflux' , data=mflux.T , chunks=None) #; dset.attrs['dimensional'] = True  ; dset.attrs['unit'] = '[kg/(m²·s)]'
         
@@ -20824,72 +20840,1462 @@
         self.get_header(verbose=False)
         if verbose: print(72*'-')
         if verbose: print('total time : ztmd.calc_vel_tangnorm_mean_removed() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
-    # === post-processing: mass, momentum, energy balance
+    # === post-processing: mass & momentum balance
+    
+    @staticmethod
+    def mass_balance_kernel(x,y, u,v,rho, transformation_matrix=None, acc=8, edge_stencil='half'):
+        '''
+        get Cartesian mass balance terms in 2D plane
+        '''
+        
+        ## stack 2D arrays, each with shape (nx,ny) along third axis --> shape=(nx,ny,2)
+        uv2d = np.copy(np.stack((u,v), axis=-1))
+        
+        ## rotate & translate [x,y]
+        if (transformation_matrix is not None):
+            
+            ## rotate & translate [x,y]
+            xy2d_tmp = np.copy( np.stack( ( x, y, np.ones_like(x) ), axis=-1) )
+            xy2d_tmp = np.copy( np.einsum( 'ij,xyj->xyi', transformation_matrix , xy2d_tmp ) )
+            xy2d     = np.copy( xy2d_tmp[:,:,:2] )
+            xy2d_tmp = None; del xy2d_tmp
+            
+            ## overwrite
+            x = np.squeeze(np.copy(xy2d[:,:,0]))
+            y = np.squeeze(np.copy(xy2d[:,:,1]))
+            
+            ## make a copy of the [2x2] matrix
+            rotation_matrix_2x2 = np.copy(transformation_matrix[:2,:2])
+            
+            ## rotate [u,v]
+            uv2d = np.copy( np.einsum( 'ij,xyj->xyi' , rotation_matrix_2x2 , uv2d ) )
+            
+            ## overwrite
+            u = np.squeeze(np.copy(uv2d[:,:,0]))
+            v = np.squeeze(np.copy(uv2d[:,:,1]))
+        
+        else:
+            
+            ## stack 2D arrays, each with shape (nx,ny) along third axis --> shape=(nx,ny,2)
+            xy2d = np.copy(np.stack((x,y), axis=-1))
+        
+        ## get metric tensor
+        M = get_metric_tensor_2d(x, y, acc=acc, edge_stencil=edge_stencil, verbose=False)
+        ddx1_q1 = np.copy( M[:,:,0,0] ) ## ∂q1/∂x1 --> ∂q1/∂x or ∂q1/∂r
+        ddx1_q2 = np.copy( M[:,:,1,0] ) ## ∂q2/∂x1 --> ∂q2/∂x or ∂q2/∂r
+        ddx2_q1 = np.copy( M[:,:,0,1] ) ## ∂q1/∂x2 --> ∂q1/∂y or ∂q1/∂θ
+        ddx2_q2 = np.copy( M[:,:,1,1] ) ## ∂q2/∂x2 --> ∂q2/∂y or ∂q2/∂θ
+        M = None ; del M
+        
+        # ===
+        
+        A = np.copy( rho * u )
+        ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+        ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+        ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+        ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+        
+        ddx_r_u = np.copy(ddx_A)
+        ddy_r_u = np.copy(ddy_A)
+        
+        ddx_A = None; del ddx_A
+        ddy_A = None; del ddy_A
+        
+        
+        A = np.copy( rho * v )
+        ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+        ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+        ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+        ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+        
+        ddx_r_v = np.copy(ddx_A)
+        ddy_r_v = np.copy(ddy_A)
+        
+        ddx_A = None; del ddx_A
+        ddy_A = None; del ddy_A
+        
+        # ===
+        
+        data = {'t1':ddx_r_u,
+                't2':ddy_r_v,
+               }
+        
+        return data
     
     def calc_mass_balance_terms(self, **kwargs):
         '''
         calculate terms of time-averaged mass conservation equation
         '''
         
-        verbose = kwargs.get('verbose',True)
+        verbose      = kwargs.get('verbose',True)
+        local_csys   = kwargs.get('local_csys',False)
+        gn           = kwargs.get('gn','data_mass') ## group name
+        acc          = kwargs.get('acc',8)
+        edge_stencil = kwargs.get('edge_stencil','half')
+        xis          = kwargs.get('xis',None)
+        
+        csys_type = 'cartesian' ## dummy for now... mass balance in cylindrical not yet implemented
+        
         if verbose: print('\n'+'ztmd.calc_mass_balance_terms()'+'\n'+72*'-')
         t_start_func = timeit.default_timer()
         
-        pass
-        pass
-        raise NotImplementedError
+        if verbose: even_print('local_csys',str(local_csys))
+        if verbose: even_print('csys_type',csys_type)
+        if verbose: even_print('group name',f'{gn}/')
+        
+        if local_csys:
+            if self.rectilinear:
+                print('>>> WARNING: this grid is rectilinear. Using local csys is not needed.')
+            if not ('csys/vtang' in self):
+                raise ValueError('csys/vtang not in hdf5')
+            if not ('csys/vnorm' in self):
+                raise ValueError('csys/vnorm not in hdf5')
+            
+            ## read unit vectors (wall tangent, wall norm) from HDF5
+            vtang = np.copy( self['csys/vtang'][()] )
+            vnorm = np.copy( self['csys/vnorm'][()] )
+            if verbose: even_print('vtang',str(vtang.shape))
+            if verbose: even_print('vnorm',str(vnorm.shape))
+        
+        ## if group already exists, delete it entirely
+        if (gn in self):
+            del self[gn]
+            if verbose: even_print('deleted group',f'/{gn}/')
+        
+        ## create group
+        grp = self.create_group(gn)
+        if verbose: even_print('created group',f'{grp.name}/')
+        
+        ## set group attributes
+        grp.attrs['local_csys'] = local_csys
+        if verbose: even_print(f'{gn}.local_csys',str(grp.attrs['local_csys']))
+        
+        if verbose: print(72*'-')
+        
+        terms = {'t1':r'$\partial_x [\bar{\rho} \tilde{u}]$',
+                 't2':r'$\partial_y [\bar{\rho} \tilde{v}]$',
+                 }
+        
+        ## initialize dsets
+        for dsn, tag in terms.items():
+            shape = (self.ny,self.nx)
+            if (f'{gn}/{dsn}' in self): del self[f'{gn}/{dsn}']
+            dset = self.create_dataset(f'{gn}/{dsn}', 
+                                       shape=shape, 
+                                       dtype=np.float32,
+                                       chunks=None)
+            if verbose: even_print(f'{gn}/{dsn}',str(shape))
+            dset.attrs['latex'] = tag
+            if verbose: even_print(f'{dsn}.latex',str(dset.attrs['latex']))
+        
+        if verbose: print(72*'-')
+        
+        ## copy data
+        u   = np.copy( self['data/u'][()].T   )
+        v   = np.copy( self['data/v'][()].T   )
+        #w   = np.copy( self['data/w'][()].T   )
+        rho = np.copy( self['data/rho'][()].T )
+        #p   = np.copy( self['data/p'][()].T   )
+        #T   = np.copy( self['data/T'][()].T   )
+        #mu  = np.copy( self['data/mu'][()].T  )
+        if verbose: even_print('u',str(u.shape))
+        if verbose: even_print('v',str(v.shape))
+        if verbose: even_print('ρ',str(rho.shape))
+        
+        u_Fv = np.copy( self['data/u_Fv'][()].T )
+        v_Fv = np.copy( self['data/v_Fv'][()].T )
+        if verbose: even_print('u_Fv',str(u_Fv.shape))
+        if verbose: even_print('v_Fv',str(v_Fv.shape))
+        
+        x = np.copy(self.x)
+        y = np.copy(self.y)
+        
+        if (x.ndim==1) and (y.ndim==1):
+            x,y = np.meshgrid(x,y, indexing='ij')
+        if verbose: even_print('x',str(x.shape))
+        if verbose: even_print('y',str(y.shape))
+        
+        if local_csys:
+            
+            # ## calculate grid points for specific postions in char. lengths
+            # s_vert_locs = [-100,-50,-25,0,+25,+50,+100]
+            # svert  = (self.stang-250*self.lchar)/self.lchar
+            # xis    = [ np.abs(s-svert).argmin() for s in s_vert_locs ]
+            
+            if (xis is None):
+                xis = np.arange(self.nx)
+                n_prog = self.nx
+            else:
+                n_prog = len(xis)
+            
+            if verbose: progress_bar = tqdm(total=n_prog, ncols=100, desc='mass balance', leave=False, file=sys.stdout)
+            
+            ## iterate through axis=0 indices
+            for xi in xis:
+                
+                rotation_angle_z = np.arcsin(vnorm[xi,0,0])
+                #rotation_angle_z = np.arcsin(-vtang[xi,0,1])
+                #if verbose: tqdm.write( even_print('rotation_angle_z', f'{np.degrees(rotation_angle_z):0.14f} [deg]', s=True) )
+                
+                rotation_matrix_1 = np.array( [[ np.cos(rotation_angle_z) , -np.sin(rotation_angle_z) , 0 ],
+                                               [ np.sin(rotation_angle_z) ,  np.cos(rotation_angle_z) , 0 ],
+                                               [ 0                        ,  0                        , 1 ]], dtype=np.float64 )
+                
+                rotation_matrix_2 = np.array( [[ vtang[xi,0,0] ,  vtang[xi,0,1] , 0 ],
+                                               [ vnorm[xi,0,0] ,  vnorm[xi,0,1] , 0 ],
+                                               [ 0             ,  0             , 1 ]], dtype=np.float64 )
+                
+                ## just showing that these are the same
+                np.testing.assert_allclose( rotation_matrix_1 , rotation_matrix_2 , rtol=1e-14 , atol=1e-14 )
+                rotation_matrix = np.copy(rotation_matrix_1)
+                
+                ## translate to [cx,cy]
+                cx = x[xi,0]
+                cy = y[xi,0]
+                translation_matrix_A = np.array( [[ 1 , 0 , -cx ],
+                                                  [ 0 , 1 , -cy ],
+                                                  [ 0 , 0 , 1   ]], dtype=np.float64 )
+                
+                ## translate in [y] by -R (the local curvature radius)
+                if (csys_type=='cylindrical'):
+                    cx = 0.
+                    cy = crv_R[xi]
+                    translation_matrix_B = np.array( [[ 1 , 0 , 0.  ],
+                                                      [ 0 , 1 , -cy ],
+                                                      [ 0 , 0 , 1   ]], dtype=np.float64 )
+                else:
+                    translation_matrix_B = np.identity(3, dtype=np.float64)
+                
+                ## form the full [3x3] matrix by multiplying together --> order matters!
+                transformation_matrix = np.einsum( 'ij,jk,kl->il', translation_matrix_B , rotation_matrix, translation_matrix_A )
+                
+                # ===
+                
+                ## send to kernel
+                data = ztmd.mass_balance_kernel(x=x,y=y,
+                                                u=u_Fv, v=v_Fv, rho=rho,
+                                                transformation_matrix=transformation_matrix,
+                                                acc=acc,edge_stencil=edge_stencil,
+                                                )
+                
+                ## write to HDF5 (only data from single axis=0 index)
+                for dsn, arr in data.items():
+                    dset = self[f'{gn}/{dsn}']
+                    dset[:,xi] = arr[xi,:] ## arrays in HDF5 are transposed
+                
+                if verbose: progress_bar.update()
+            if verbose: progress_bar.close()
+        
+        else:
+            
+            ## send to kernel
+            data = ztmd.mass_balance_kernel(x=x,y=y,
+                                            u=u_Fv, v=v_Fv, rho=rho,
+                                            transformation_matrix=None,
+                                            acc=acc,edge_stencil=edge_stencil,
+                                            )
+            
+            ## write to HDF5 (only data from single axis=0 index)
+            for dsn, arr in data.items():
+                dset = self[f'{gn}/{dsn}']
+                dset[:,:] = arr.T ## arrays in HDF5 are transposed
         
         self.get_header(verbose=False)
         if verbose: print(72*'-')
         if verbose: print('total time : ztmd.calc_mass_balance_terms() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
-    def calc_momentum_balance_x_terms(self, **kwargs):
+    @staticmethod
+    def momentum_balance_kernel_cartesian(x,y, u,v, u_Fv,v_Fv, p,rho,mu, r_uII_uII,r_uII_vII,r_vII_vII, transformation_matrix=None, acc=8, edge_stencil='half'):
         '''
-        calculate terms of time-averaged momentum [x] conservation equation
+        get Cartesian [x] momentum balance terms in 2D plane
         '''
         
-        verbose = kwargs.get('verbose',True)
-        if verbose: print('\n'+'ztmd.calc_momentum_balance_x_terms()'+'\n'+72*'-')
-        t_start_func = timeit.default_timer()
+        nx,ny = x.shape
         
-        pass
-        pass
-        raise NotImplementedError
+        ## stack 2D arrays, each with shape (nx,ny) along third axis --> shape=(nx,ny,2)
+        uv2d    = np.copy(np.stack((u,v),       axis=-1))
+        uv2d_Fv = np.copy(np.stack((u_Fv,v_Fv), axis=-1))
         
-        self.get_header(verbose=False)
-        if verbose: print(72*'-')
-        if verbose: print('total time : ztmd.calc_momentum_balance_x_terms() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
-        if verbose: print(72*'-')
+        ## rotate & translate [x,y]
+        if (transformation_matrix is not None):
+            
+            ## rotate & translate [x,y]
+            xy2d_tmp = np.copy( np.stack( ( x, y, np.ones_like(x) ), axis=-1) )
+            xy2d_tmp = np.copy( np.einsum( 'ij,xyj->xyi', transformation_matrix , xy2d_tmp ) )
+            xy2d     = np.copy( xy2d_tmp[:,:,:2] )
+            xy2d_tmp = None; del xy2d_tmp
+            
+            ## overwrite
+            x = np.squeeze(np.copy(xy2d[:,:,0]))
+            y = np.squeeze(np.copy(xy2d[:,:,1]))
+            
+            ## make a copy of the [2x2] matrix
+            rotation_matrix_2x2 = np.copy(transformation_matrix[:2,:2])
+            
+            ## rotate [u,v]
+            uv2d = np.copy( np.einsum( 'ij,xyj->xyi' , rotation_matrix_2x2 , uv2d ) )
+            
+            ## overwrite
+            u = np.squeeze(np.copy(uv2d[:,:,0]))
+            v = np.squeeze(np.copy(uv2d[:,:,1]))
+            
+            ## rotate [u_Fv,v_Fv]
+            uv2d_Fv = np.copy( np.einsum( 'ij,xyj->xyi' , rotation_matrix_2x2 , uv2d_Fv ) )
+            
+            ## overwrite
+            u_Fv = np.squeeze(np.copy(uv2d_Fv[:,:,0]))
+            v_Fv = np.squeeze(np.copy(uv2d_Fv[:,:,1]))
+            
+            if True: ## Re-Stress tensor: global Cartesian rotate
+                
+                r_uiIIujII = np.zeros((nx,ny,2,2), dtype=np.float64)
+                r_uiIIujII[:,:,0,0] = np.copy( r_uII_uII )
+                r_uiIIujII[:,:,0,1] = np.copy( r_uII_vII )
+                r_uiIIujII[:,:,1,0] = np.copy( r_uII_vII )
+                r_uiIIujII[:,:,1,1] = np.copy( r_vII_vII )
+                
+                ## assert symmetric
+                np.testing.assert_allclose(r_uiIIujII, np.transpose(r_uiIIujII, (0,1,3,2)), atol=1e-14, rtol=1e-14)
+                
+                ## do tensor rotation : [A'] = [R][A][R]^T
+                r_uiIIujII = np.copy( np.einsum( 'ij,xyjk,kl->xyil' , rotation_matrix_2x2 , r_uiIIujII , rotation_matrix_2x2.T ) )
+                
+                r_uII_uII = np.copy(r_uiIIujII[:,:,0,0])
+                r_uII_vII = np.copy(r_uiIIujII[:,:,0,1])
+                r_vII_uII = np.copy(r_uiIIujII[:,:,1,0])
+                r_vII_vII = np.copy(r_uiIIujII[:,:,1,1])
+                
+                r_uiIIujII = None ; del r_uiIIujII
+                
+                np.testing.assert_allclose(r_uII_vII, r_vII_uII, atol=1e-7, rtol=1e-7)
         
-        return
+        else:
+            
+            ## stack 2D arrays, each with shape (nx,ny) along third axis --> shape=(nx,ny,2)
+            xy2d = np.copy(np.stack((x,y), axis=-1))
+        
+        # ===
+        
+        ## get metric tensor M = δ[q1,q2]/δ[x1,x2] : δ[q1,q2]/δ[x,y] or δ[q1,q2]/δ[r,θ]
+        M = get_metric_tensor_2d(x, y, acc=acc, edge_stencil=edge_stencil, verbose=False)
+        ddx1_q1 = np.copy( M[:,:,0,0] ) ## ∂q1/∂x1 --> ∂q1/∂x or ∂q1/∂r
+        ddx1_q2 = np.copy( M[:,:,1,0] ) ## ∂q2/∂x1 --> ∂q2/∂x or ∂q2/∂r
+        ddx2_q1 = np.copy( M[:,:,0,1] ) ## ∂q1/∂x2 --> ∂q1/∂y or ∂q1/∂θ
+        ddx2_q2 = np.copy( M[:,:,1,1] ) ## ∂q2/∂x2 --> ∂q2/∂y or ∂q2/∂θ
+        M = None ; del M
+        
+        # ===
+        
+        if True: ## calculate gradients : Cartesian [x,y]
+            
+            ## [x1,x2] = [x,y]
+            ## ∂(A)/∂x1 = ∂(A)/∂(q1)·∂(q1)/∂(x1) + ∂(A)/∂(q2)·∂(q2)/∂(x1)
+            ## ∂(A)/∂x2 = ∂(A)/∂(q1)·∂(q1)/∂(x2) + ∂(A)/∂(q2)·∂(q2)/∂(x2)
+            
+            A = np.copy( u )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddx_u = np.copy(ddx_A)
+            ddy_u = np.copy(ddy_A)
+            
+            ddx_A = None; del ddx_A
+            ddy_A = None; del ddy_A
+            
+            
+            A = np.copy( v )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddx_v = np.copy(ddx_A)
+            ddy_v = np.copy(ddy_A)
+            
+            ddx_A = None; del ddx_A
+            ddy_A = None; del ddy_A
+            
+            
+            A = np.copy( rho )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddx_rho = np.copy(ddx_A)
+            ddy_rho = np.copy(ddy_A)
+            
+            ddx_A = None; del ddx_A
+            ddy_A = None; del ddy_A
+            
+            
+            A = np.copy( p )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddx_p = np.copy(ddx_A)
+            ddy_p = np.copy(ddy_A)
+            
+            ddx_A = None; del ddx_A
+            ddy_A = None; del ddy_A
+            
+            
+            A = np.copy( u_Fv )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddx_u_Fv = np.copy(ddx_A)
+            ddy_u_Fv = np.copy(ddy_A)
+            
+            ddx_A = None; del ddx_A
+            ddy_A = None; del ddy_A
+            
+            
+            A = np.copy( v_Fv )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddx_v_Fv = np.copy(ddx_A)
+            ddy_v_Fv = np.copy(ddy_A)
+            
+            ddx_A = None; del ddx_A
+            ddy_A = None; del ddy_A
+        
+        if True: ## construct momentum balance : Cartesian [x,y]
+            
+            tau_xx = np.copy( +(4/3)*mu*ddx_u - (2/3)*mu*ddy_v )
+            tau_yy = np.copy( -(2/3)*mu*ddx_u + (4/3)*mu*ddy_v )
+            
+            tau_xy = np.copy( mu*(ddx_v + ddy_u) )
+            #tau_yx = np.copy( tau_xy )
+            
+            # === δx[ρ·u·u]
+            
+            A = np.copy( rho * u_Fv * u_Fv )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddx_r_uFv_uFv = np.copy(ddx_A)
+            t1x = np.copy( ddx_r_uFv_uFv )
+            t1x_lbl = r'$\partial_{x}[\bar{\rho} \tilde{u} \tilde{u}]$'
+            
+            ddx_A = None; del ddx_A
+            ddy_A = None; del ddy_A
+            
+            # === δx[ρ·u·v] & δy[ρ·u·v]
+            
+            A = np.copy( rho * u_Fv * v_Fv )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddx_r_uFv_vFv = np.copy(ddx_A)
+            ddy_r_uFv_vFv = np.copy(ddy_A)
+            
+            t1y = np.copy( ddx_r_uFv_vFv )
+            t1y_lbl = r'$\partial_{x}[\bar{\rho} \tilde{u} \tilde{v}]$'
+            
+            t2x = np.copy( ddy_r_uFv_vFv )
+            t2x_lbl = r'$\partial_{y}[\bar{\rho} \tilde{u} \tilde{v}]$'
+            
+            ddx_A = None; del ddx_A
+            ddy_A = None; del ddy_A
+            
+            # === δy[ρ·v·v]
+            
+            A = np.copy( rho * v_Fv * v_Fv )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddy_r_vFv_vFv = np.copy(ddy_A)
+            t2y = np.copy( ddy_r_vFv_vFv )
+            t2y_lbl = r'$\partial_{y}[\bar{\rho} \tilde{v} \tilde{v}]$'
+            
+            ddx_A = None; del ddx_A
+            ddy_A = None; del ddy_A
+            
+            # === δx[ρ·u''·u'']
+            
+            A = np.copy(r_uII_uII)
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddx_r_uII_uII = np.copy(ddx_A)
+            t5x = np.copy( ddx_r_uII_uII )
+            t5x_lbl = r'$\partial_{x}[ \overline{ \rho u^{\prime\prime} u^{\prime\prime}} ]$'
+            
+            ddx_A = None; del ddx_A
+            ddy_A = None; del ddy_A
+            
+            # === δx[ρ·u''·v''] & δy[ρ·u''·v'']
+            
+            A = np.copy(r_uII_vII)
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddx_r_uII_vII = np.copy(ddx_A)
+            ddy_r_uII_vII = np.copy(ddy_A)
+            
+            t5y = np.copy( ddx_r_uII_vII )
+            t5y_lbl = r'$\partial_{x}[ \overline{ \rho u^{\prime\prime} v^{\prime\prime}} ]$'
+            t7x = np.copy( ddy_r_uII_vII )
+            t7x_lbl = r'$\partial_{y}[ \overline{ \rho u^{\prime\prime} v^{\prime\prime}} ]$'
+            
+            ddx_A = None; del ddx_A
+            ddy_A = None; del ddy_A
+            
+            # === δy[ρ·v''·v'']
+            
+            A = np.copy(r_vII_vII)
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddy_r_vII_vII = np.copy(ddy_A)
+            t7y = np.copy( ddy_r_vII_vII )
+            t7y_lbl = r'$\partial_{y}[ \overline{\rho v^{\prime\prime} v^{\prime\prime}} ]$'
+            
+            ddx_A = None; del ddx_A
+            ddy_A = None; del ddy_A
+            
+            # === δx[p] & δy[p]
+            
+            t3x = np.copy( ddx_p )
+            t3x_lbl = r'$\partial_{x}[p]$'
+            
+            t3y = np.copy( ddy_p )
+            t3y_lbl = r'$\partial_{y}[p]$'
+            
+            # === δx[τxx]
+            
+            ddq1_A = gradient(tau_xx, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(tau_xx, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddx_tau_xx = np.copy(ddx_A)
+            t4x = np.copy( -1 * ddx_tau_xx )
+            t4x_lbl = r'$-\partial_{x}[\overline{\tau_{xx}}]$'
+            
+            ddx_A = None; del ddx_A
+            ddy_A = None; del ddy_A
+            
+            # === δx[τxy] & δy[τxy]
+            
+            ddq1_A = gradient(tau_xy, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(tau_xy, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddx_tau_xy = np.copy(ddx_A)
+            ddy_tau_xy = np.copy(ddy_A)
+            
+            t4y = np.copy( -1 * ddx_tau_xy )
+            t4y_lbl = r'$-\partial_{x}[\overline{\tau_{xy}}]$'
+            
+            t6x = np.copy( -1 * ddy_tau_xy )
+            t6x_lbl = r'$-\partial_{y}[\overline{\tau_{xy}}]$'
+            
+            ddx_A = None; del ddx_A
+            ddy_A = None; del ddy_A
+            
+            # === δy[τyy]
+            
+            ddq1_A = gradient(tau_yy, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(tau_yy, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx_A  = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddy_A  = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddy_tau_yy = np.copy(ddy_A)
+            t6y = np.copy( -1 * ddy_tau_yy )
+            t6y_lbl = r'$-\partial_{y}[\overline{\tau_{yy}}]$'
+            
+            ddx_A = None; del ddx_A
+            ddy_A = None; del ddy_A
+        
+        # ===
+        
+        data_x = {'t1':np.copy(t1x),
+                  't2':np.copy(t2x),
+                  't3':np.copy(t3x),
+                  't4':np.copy(t4x),
+                  't5':np.copy(t5x),
+                  't6':np.copy(t6x),
+                  't7':np.copy(t7x),
+                  }
+        
+        data_y = {'t1':np.copy(t1y),
+                  't2':np.copy(t2y),
+                  't3':np.copy(t3y),
+                  't4':np.copy(t4y),
+                  't5':np.copy(t5y),
+                  't6':np.copy(t6y),
+                  't7':np.copy(t7y),
+                  }
+        
+        return data_x, data_y
     
-    def calc_momentum_balance_y_terms(self, **kwargs):
+    @staticmethod
+    def momentum_balance_kernel_cylindrical(x,y, u,v, u_Fv,v_Fv, p,rho,mu, r_uII_uII,r_uII_vII,r_vII_vII, transformation_matrix=None, acc=8, edge_stencil='half'):
         '''
-        calculate terms of time-averaged momentum [y] conservation equation
+        get cylindrical [r,θ] momentum balance terms in 2D plane
         '''
         
-        verbose = kwargs.get('verbose',True)
-        if verbose: print('\n'+'ztmd.calc_momentum_balance_y_terms()'+'\n'+72*'-')
+        nx,ny = x.shape
+        
+        ## stack 2D arrays, each with shape (nx,ny) along third axis --> shape=(nx,ny,2)
+        uv2d    = np.copy(np.stack((u,v),       axis=-1))
+        uv2d_Fv = np.copy(np.stack((u_Fv,v_Fv), axis=-1))
+        
+        ## rotate & translate [x,y]
+        if (transformation_matrix is not None):
+            
+            ## rotate & translate [x,y]
+            xy2d_tmp = np.copy( np.stack( ( x, y, np.ones_like(x) ), axis=-1) )
+            xy2d_tmp = np.copy( np.einsum( 'ij,xyj->xyi', transformation_matrix , xy2d_tmp ) )
+            xy2d     = np.copy( xy2d_tmp[:,:,:2] )
+            xy2d_tmp = None; del xy2d_tmp
+            
+            ## overwrite
+            x = np.squeeze(np.copy(xy2d[:,:,0]))
+            y = np.squeeze(np.copy(xy2d[:,:,1]))
+            
+            ## make a copy of the [2x2] matrix
+            rotation_matrix_2x2 = np.copy(transformation_matrix[:2,:2])
+            
+            ## rotate [u,v]
+            uv2d = np.copy( np.einsum( 'ij,xyj->xyi' , rotation_matrix_2x2 , uv2d ) )
+            
+            ## overwrite
+            u = np.squeeze(np.copy(uv2d[:,:,0]))
+            v = np.squeeze(np.copy(uv2d[:,:,1]))
+            
+            ## rotate [u_Fv,v_Fv]
+            uv2d_Fv = np.copy( np.einsum( 'ij,xyj->xyi' , rotation_matrix_2x2 , uv2d_Fv ) )
+            
+            ## overwrite
+            u_Fv = np.squeeze(np.copy(uv2d_Fv[:,:,0]))
+            v_Fv = np.squeeze(np.copy(uv2d_Fv[:,:,1]))
+            
+            if True: ## Re-Stress tensor: global Cartesian rotate
+                
+                r_uiIIujII = np.zeros((nx,ny,2,2), dtype=np.float64)
+                r_uiIIujII[:,:,0,0] = np.copy( r_uII_uII )
+                r_uiIIujII[:,:,0,1] = np.copy( r_uII_vII )
+                r_uiIIujII[:,:,1,0] = np.copy( r_uII_vII )
+                r_uiIIujII[:,:,1,1] = np.copy( r_vII_vII )
+                
+                ## assert symmetric
+                np.testing.assert_allclose(r_uiIIujII, np.transpose(r_uiIIujII, (0,1,3,2)), atol=1e-14, rtol=1e-14)
+                
+                ## do tensor rotation : [A'] = [R][A][R]^T
+                r_uiIIujII = np.copy( np.einsum( 'ij,xyjk,kl->xyil' , rotation_matrix_2x2 , r_uiIIujII , rotation_matrix_2x2.T ) )
+                
+                r_uII_uII = np.copy(r_uiIIujII[:,:,0,0])
+                r_uII_vII = np.copy(r_uiIIujII[:,:,0,1])
+                r_vII_uII = np.copy(r_uiIIujII[:,:,1,0])
+                r_vII_vII = np.copy(r_uiIIujII[:,:,1,1])
+                
+                r_uiIIujII = None ; del r_uiIIujII
+                
+                np.testing.assert_allclose(r_uII_vII, r_vII_uII, atol=1e-7, rtol=1e-7)
+        
+        else:
+            
+            ## stack 2D arrays, each with shape (nx,ny) along third axis --> shape=(nx,ny,2)
+            xy2d = np.copy(np.stack((x,y), axis=-1))
+        
+        # ===
+        
+        ## calculate coordinate arrays [r,θ] from [x,y]
+        r     = np.copy( np.sqrt(x**2 + y**2) )
+        theta = np.copy( np.arctan2(y,x) )
+        
+        ## calculate [ur,uθ] from [u,v]
+        vel_cart2cyl_trans_mat = np.zeros((nx,ny,2,2), dtype=np.float64)
+        for i in range(nx):
+            for j in range(ny):
+                vel_cart2cyl_trans_mat[i,j,:,:] = np.array( [[  np.cos(theta[i,j]) , np.sin(theta[i,j]) ],
+                                                             [ -np.sin(theta[i,j]) , np.cos(theta[i,j]) ]], dtype=np.float64 )
+        
+        ## ur, uθ
+        urut2d = np.einsum( 'xyji,xyi->xyj', vel_cart2cyl_trans_mat, uv2d )
+        ur = np.squeeze(np.copy(urut2d[:,:,0]))
+        ut = np.squeeze(np.copy(urut2d[:,:,1]))
+        
+        ## ur_Fv, uθ_Fv
+        urut2d_Fv = np.einsum( 'xyji,xyi->xyj', vel_cart2cyl_trans_mat, uv2d_Fv )
+        ur_Fv = np.squeeze(np.copy(urut2d_Fv[:,:,0]))
+        ut_Fv = np.squeeze(np.copy(urut2d_Fv[:,:,1]))
+        
+        ## Re-Stress tensor : convert from Cartesian (rotated) to cylindrical components
+        r_uiIIujII = np.zeros((nx,ny,2,2), dtype=np.float64)
+        r_uiIIujII[:,:,0,0] = np.copy( r_uII_uII )
+        r_uiIIujII[:,:,0,1] = np.copy( r_uII_vII )
+        r_uiIIujII[:,:,1,0] = np.copy( r_uII_vII )
+        r_uiIIujII[:,:,1,1] = np.copy( r_vII_vII )
+        
+        r_uII_uII = None; del r_uII_uII
+        r_uII_vII = None; del r_uII_vII
+        r_vII_uII = None; del r_vII_uII
+        r_vII_vII = None; del r_vII_vII
+        
+        ## assert symmetric
+        np.testing.assert_allclose(r_uiIIujII, np.transpose(r_uiIIujII, (0,1,3,2)), atol=1e-14, rtol=1e-14)
+        
+        ## csys conversion : Cartesian --> cylindrical
+        r_uiIIujII = np.copy( np.einsum( 'xyij,xyjk,xykl->xyil' , vel_cart2cyl_trans_mat , r_uiIIujII , np.transpose(vel_cart2cyl_trans_mat,(0,1,3,2)) ) )
+        
+        r_urII_urII = np.copy(r_uiIIujII[:,:,0,0])
+        r_urII_utII = np.copy(r_uiIIujII[:,:,0,1])
+        r_utII_urII = np.copy(r_uiIIujII[:,:,1,0])
+        r_utII_utII = np.copy(r_uiIIujII[:,:,1,1])
+        
+        r_uiIIujII = None ; del r_uiIIujII
+        
+        ## assert symmetric again
+        np.testing.assert_allclose(r_urII_utII, r_utII_urII, atol=1e-7, rtol=1e-7)
+        
+        # ===
+        
+        ## get metric tensor M = δ[q1,q2]/δ[x1,x2] : δ[q1,q2]/δ[x,y] or δ[q1,q2]/δ[r,θ]
+        M = get_metric_tensor_2d(r, theta, acc=acc, edge_stencil=edge_stencil, verbose=False)
+        ddx1_q1 = np.copy( M[:,:,0,0] ) ## ∂q1/∂x1 --> ∂q1/∂x or ∂q1/∂r
+        ddx1_q2 = np.copy( M[:,:,1,0] ) ## ∂q2/∂x1 --> ∂q2/∂x or ∂q2/∂r
+        ddx2_q1 = np.copy( M[:,:,0,1] ) ## ∂q1/∂x2 --> ∂q1/∂y or ∂q1/∂θ
+        ddx2_q2 = np.copy( M[:,:,1,1] ) ## ∂q2/∂x2 --> ∂q2/∂y or ∂q2/∂θ
+        M = None ; del M
+        
+        # ===
+        
+        if True: ## calculate gradients : cylindrical [r,θ]
+            
+            ## [x1,x2] = [r,θ]
+            ## ∂(A)/∂x1 = ∂(A)/∂(q1)·∂(q1)/∂(x1) + ∂(A)/∂(q2)·∂(q2)/∂(x1)
+            ## ∂(A)/∂x2 = ∂(A)/∂(q1)·∂(q1)/∂(x2) + ∂(A)/∂(q2)·∂(q2)/∂(x2)
+            
+            A = np.copy( ur )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddr_ur = np.copy(ddx1_A)
+            ddt_ur = np.copy(ddx2_A)
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+            
+            
+            A = np.copy( ut )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddr_ut = np.copy(ddx1_A)
+            ddt_ut = np.copy(ddx2_A)
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+            
+            
+            A = np.copy( rho )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddr_rho = np.copy(ddx1_A)
+            ddt_rho = np.copy(ddx2_A)
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+            
+            
+            A = np.copy( p )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddr_p = np.copy(ddx1_A)
+            ddt_p = np.copy(ddx2_A)
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+            
+            
+            A = np.copy( ur_Fv )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddr_ur_Fv = np.copy(ddx1_A)
+            ddt_ur_Fv = np.copy(ddx2_A)
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+            
+            
+            A = np.copy( ut_Fv )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddr_ut_Fv = np.copy(ddx1_A)
+            ddt_ut_Fv = np.copy(ddx2_A)
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+        
+        if True: ## construct momentum balance : cylindrical [r,θ]
+            
+            ## τ_rr, τ_θθ, τ_rθ
+            tau_rr = np.copy( +(4/3)*mu*ddr_ur - (2/3)*(1/r)*mu*ddt_ut - (2/3)*mu*(ur/r) )
+            tau_tt = np.copy( -(2/3)*mu*ddr_ur + (4/3)*(1/r)*mu*ddt_ut + (4/3)*mu*(ur/r) )
+            tau_rt = np.copy( mu*( (1/r)*ddt_ur + ddr_ut - (ut/r) ) )
+            
+            # === δr[ρ·ur·ur]
+            
+            A = np.copy( rho * ur_Fv * ur_Fv )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddr_rho_urFv_urFv = np.copy(ddx1_A)
+            t1x1 = np.copy( ddr_rho_urFv_urFv )
+            t1x1_lbl = r'$\partial_{r}[ \bar{\rho} \tilde{u}_r \tilde{u}_r ]$'
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+            
+            # === (1/r)·δθ[ρ·ur·uθ]
+            
+            A = np.copy( rho * ur_Fv * ut_Fv )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddt_rho_urFv_utFv = np.copy(ddx2_A)
+            t2x1 = np.copy( (1/r)*ddt_rho_urFv_utFv )
+            t2x1_lbl = r'$\frac{1}{r} \partial_{\theta}[ \bar{\rho} \tilde{u}_r \tilde{u}_\theta ]$'
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+            
+            # === δr[ρ·ur·uθ]
+            
+            A = np.copy( rho * ur_Fv * ut_Fv )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddr_rho_urFv_utFv = np.copy(ddx1_A)
+            t1x2 = np.copy( ddr_rho_urFv_utFv )
+            t1x2_lbl = r'$\partial_{r}[ \bar{\rho} \tilde{u}_r \tilde{u}_\theta ]$'
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+            
+            # === δθ[ρ·uθ·uθ]
+            
+            A = np.copy( rho * ut_Fv * ut_Fv )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddt_rho_utFv_utFv = np.copy(ddx2_A)
+            t2x2 = np.copy( (1/r)*ddt_rho_utFv_utFv )
+            t2x2_lbl = r'$\frac{1}{r} \partial_{\theta}[ \bar{\rho} \tilde{u}_\theta \tilde{u}_\theta ]$'
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+            
+            # === δr[p] & δθ[p]
+            
+            t3x1 = np.copy( ddr_p )
+            t3x1_lbl = r'$\partial_{r}[\bar{p}]$'
+            
+            t3x2 = np.copy( (1/r)*ddt_p )
+            t3x2_lbl = r'$\frac{1}{r} \partial_{\theta}[\bar{p}]$'
+            
+            # === δr[τ_rr]
+            
+            A = np.copy( tau_rr )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddr_tau_rr = np.copy( ddx1_A )
+            t4x1 = np.copy( -ddr_tau_rr )
+            t4x1_lbl = r'$-\partial_{r}[ \overline{\tau}_{r r} ]$'
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+            
+            # === -(1/r)·δθ[τ_θθ]
+            
+            A = np.copy( tau_tt )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddt_tau_tt = np.copy( ddx2_A )
+            t6x2 = np.copy( -(1/r)*ddt_tau_tt )
+            t6x2_lbl = r'$-\frac{1}{r} \partial_{\theta}[ \overline{\tau}_{\theta \theta} ]$'
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+            
+            # === δr[ρ·ur''·ur'']
+            
+            A = np.copy( r_urII_urII )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddr_r_urII_urII = np.copy( ddx1_A )
+            t5x1 = np.copy( ddr_r_urII_urII )
+            t5x1_lbl = r'$\partial_{r}[ \overline{ \rho u^{\prime \prime}_r  u^{\prime \prime}_r } ]$'
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+            
+            # === -(1/r)·δθ[τ_rθ]  &  -δr[τ_rθ]
+            
+            A = np.copy( tau_rt )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddr_tau_rt = np.copy( ddx1_A )
+            t4x2 = np.copy( -ddr_tau_rt )
+            t4x2_lbl = r'$-\partial_{r}[ \overline{\tau}_{r \theta} ]$'
+            
+            ddt_tau_rt = np.copy( ddx2_A )
+            t6x1 = np.copy( -(1/r)*ddt_tau_rt )
+            t6x1_lbl = r'$-\frac{1}{r} \partial_{\theta}[ \overline{\tau}_{r \theta} ]$'
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+            
+            # === (1/r)·δθ[ρ·ur''·uθ''] & δr[ρ·ur''·uθ'']
+            
+            A = np.copy( r_urII_utII )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddt_r_urII_utII = np.copy( ddx2_A )
+            t7x1 = np.copy( (1/r)*ddt_r_urII_utII )
+            t7x1_lbl = r'$\frac{1}{r} \partial_{\theta}[ \overline{\rho u^{\prime \prime}_r  u^{\prime \prime}_\theta } ]$'
+            
+            ddr_r_urII_utII = np.copy( ddx1_A )
+            t5x2 = np.copy( ddr_r_urII_utII )
+            t5x2_lbl = r'$\partial_{r}[ \overline{\rho u^{\prime \prime}_r  u^{\prime \prime}_\theta } ]$'
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+            
+            # === (1/r)·δθ[ρ·uθ''·uθ'']
+            
+            A = np.copy( r_utII_utII )
+            ddq1_A = gradient(A, 1., axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddq2_A = gradient(A, 1., axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+            ddx1_A = ddq1_A*ddx1_q1 + ddq2_A*ddx1_q2
+            ddx2_A = ddq1_A*ddx2_q1 + ddq2_A*ddx2_q2
+            
+            ddt_r_utII_utII = np.copy( ddx2_A )
+            t7x2 = np.copy( (1/r)*ddt_r_utII_utII )
+            t7x2_lbl = r'$\frac{1}{r} \partial_{\theta}[ \overline{\rho u^{\prime \prime}_\theta  u^{\prime \prime}_\theta } ]$'
+            
+            ddx1_A = None; del ddx1_A
+            ddx2_A = None; del ddx2_A
+            
+            # ===
+            
+            ## +(1/r)·ρ·ur·ur
+            t8x1 = np.copy( (1/r) * rho * ur_Fv * ur_Fv )
+            t8x1_lbl = r'$\frac{1}{r} \bar{\rho} \tilde{u}_{r} \tilde{u}_{r}$'
+            
+            ## +(1/r)·ρ·ur''·ur''
+            t9x1 = np.copy( (1/r) * r_urII_urII )
+            t9x1_lbl = r'$\frac{1}{r} \overline{ \rho u^{\prime \prime}_r u^{\prime \prime}_r }$'
+            
+            ## -(1/r)·ρ·uθ·uθ
+            t10x1 = np.copy( -1 * (1/r) * rho * ut_Fv * ut_Fv )
+            t10x1_lbl = r'$-\frac{1}{r} \bar{\rho} \tilde{u}_{\theta} \tilde{u}_{\theta}$'
+            
+            ## -(1/r)·ρ·uθ''·uθ''
+            t11x1 = np.copy( -1 * (1/r) * r_utII_utII )
+            t11x1_lbl = r'$-\frac{1}{r} \overline{ \rho u^{\prime \prime}_\theta u^{\prime \prime}_\theta }$'
+            
+            ## -(1/r)·τ_rr
+            t12x1 = np.copy( -1 * (1/r) * tau_rr )
+            t12x1_lbl = r'$-\frac{1}{r} \overline{\tau}_{r r}$'
+            
+            ## +(1/r)·τ_θθ
+            t13x1 = np.copy( (1/r) * tau_tt )
+            t13x1_lbl = r'$\frac{1}{r} \overline{\tau}_{\theta \theta}$'
+            
+            # ===
+            
+            ## +(2/r)·ρ·ur·uθ
+            t8x2 = np.copy( (2/r) * rho * ur_Fv * ut_Fv )
+            t8x2_lbl = r'$\frac{2}{r} \bar{\rho} \tilde{u}_{r} \tilde{u}_{\theta}$'
+            
+            ## +(2/r)·ρ·ur·uθ
+            t9x2 = np.copy( (2/r) * r_urII_utII  )
+            t9x2_lbl = r'$\frac{2}{r} \overline{ \rho u^{\prime \prime}_r u^{\prime \prime}_\theta }$'
+            
+            ## -(2/r)·τ_rθ
+            t10x2 = np.copy( -(2/r) * tau_rt )
+            t10x2_lbl = r'$-\frac{2}{r} \overline{\tau}_{r \theta}$'
+        
+        # ===
+        
+        data_r = {'t1':np.copy(t1x1),
+                  't2':np.copy(t2x1),
+                  't3':np.copy(t3x1),
+                  't4':np.copy(t4x1),
+                  't5':np.copy(t5x1),
+                  't6':np.copy(t6x1),
+                  't7':np.copy(t7x1),
+                  't8':np.copy(t8x1),
+                  't9':np.copy(t9x1),
+                  't10':np.copy(t10x1),
+                  't11':np.copy(t11x1),
+                  't12':np.copy(t12x1),
+                  't13':np.copy(t13x1),
+                  }
+        
+        data_t = {'t1':np.copy(t1x2),
+                  't2':np.copy(t2x2),
+                  't3':np.copy(t3x2),
+                  't4':np.copy(t4x2),
+                  't5':np.copy(t5x2),
+                  't6':np.copy(t6x2),
+                  't7':np.copy(t7x2),
+                  't8':np.copy(t8x2),
+                  't9':np.copy(t9x2),
+                  't10':np.copy(t10x2),
+                  }
+        
+        return data_r, data_t
+    
+    def calc_momentum_balance_terms(self, **kwargs):
+        '''
+        calculate terms of the 2D time-averaged momentum conservation equation in Cartesian coords
+        '''
+        
+        verbose      = kwargs.get('verbose',True)
+        local_csys   = kwargs.get('local_csys',False)
+        acc          = kwargs.get('acc',8)
+        edge_stencil = kwargs.get('edge_stencil','half')
+        xis          = kwargs.get('xis',None)
+        csys_type    = kwargs.get('csys_type','cartesian')
+        
+        if verbose: print('\n'+'ztmd.calc_momentum_balance_terms()'+'\n'+72*'-')
         t_start_func = timeit.default_timer()
         
-        pass
-        pass
-        raise NotImplementedError
+        if not (self.open_mode=='a') or (self.open_mode=='w') or (self.open_mode=='r+'):
+            raise ValueError('not able to write to hdf5 file')
+        
+        if verbose: even_print('local_csys',str(local_csys))
+        if verbose: even_print('csys_type',csys_type)
+        
+        if local_csys:
+            if self.rectilinear:
+                print('>>> WARNING: this grid is rectilinear. Using local csys is not needed.')
+            if not ('csys/vtang' in self):
+                raise ValueError('csys/vtang not in hdf5')
+            if not ('csys/vnorm' in self):
+                raise ValueError('csys/vnorm not in hdf5')
+            
+            ## read unit vectors (wall tangent, wall norm) from HDF5
+            vtang = np.copy( self['csys/vtang'][()] )
+            vnorm = np.copy( self['csys/vnorm'][()] )
+            if verbose: even_print('vtang',str(vtang.shape))
+            if verbose: even_print('vnorm',str(vnorm.shape))
+        
+        if (csys_type=='cartesian'):
+            gnx = 'data_momentum_x'
+            gny = 'data_momentum_y'
+            gns = [gnx,gny]
+        elif (csys_type=='cylindrical'):
+            gnr = 'data_momentum_r'
+            gnt = 'data_momentum_theta'
+            gns = [gnr,gnt]
+        else:
+            raise NotImplementedError
+        
+        terms_x = {'t1':r'$\partial_{x}[\bar{\rho} \tilde{u} \tilde{u}]$',
+                   't2':r'$\partial_{y}[\bar{\rho} \tilde{u} \tilde{v}]$',
+                   't3':r'$\partial_{x}[\bar{p}]$',
+                   't4':r'$-\partial_{x}[\overline{\tau}_xx}]$',
+                   't5':r'$\partial_{x}[\overline{\rho u^{\prime\prime} u^{\prime\prime}}]$',
+                   't6':r'$-\partial_{y}[\overline{\tau_{xy}}]$',
+                   't7':r'$\partial_{y}[\overline{\rho u^{\prime\prime} v^{\prime\prime}}]$',
+                   }
+        
+        terms_y = {'t1':r'$\partial_{x}[\bar{\rho} \tilde{u} \tilde{v}]$',
+                   't2':r'$\partial_{y}[\bar{\rho} \tilde{v} \tilde{v}]$',
+                   't3':r'$\partial_{y}[\bar{p}]$',
+                   't4':r'$-\partial_{x}[\overline{\tau_{xy}}]$',
+                   't5':r'$\partial_{x}[\overline{\rho u^{\prime\prime} v^{\prime\prime}}]$',
+                   't6':r'$-\partial_{y}[\overline{\tau_{yy}}]$',
+                   't7':r'$\partial_{y}[\overline{\rho v^{\prime\prime} v^{\prime\prime}}]$',
+                   }
+        
+        terms_r = {'t1':r'$\partial_{r}[ \bar{\rho} \tilde{u}_r \tilde{u}_r ]$',
+                   't2':r'$\frac{1}{r} \partial_{\theta}[ \bar{\rho} \tilde{u}_r \tilde{u}_\theta ]$',
+                   't3':r'$\partial_{r}[\bar{p}]$',
+                   't4':r'$-\partial_{r}[ \overline{\tau}_{r r} ]$',
+                   't5':r'$\partial_{r}[ \overline{ \rho u^{\prime \prime}_r  u^{\prime \prime}_r } ]$',
+                   't6':r'$-\frac{1}{r} \partial_{\theta}[ \overline{\tau}_{r \theta} ]$',
+                   't7':r'$\frac{1}{r} \partial_{\theta}[ \overline{\rho u^{\prime \prime}_r  u^{\prime \prime}_\theta } ]$',
+                   't8':r'$\frac{1}{r} \bar{\rho} \tilde{u}_{r} \tilde{u}_{r}$',
+                   't9':r'$\frac{1}{r} \overline{ \rho u^{\prime \prime}_r u^{\prime \prime}_r }$',
+                   't10':r'$-\frac{1}{r} \bar{\rho} \tilde{u}_{\theta} \tilde{u}_{\theta}$',
+                   't11':r'$-\frac{1}{r} \overline{ \rho u^{\prime \prime}_\theta u^{\prime \prime}_\theta }$',
+                   't12':r'$-\frac{1}{r} \overline{\tau}_{r r}$',
+                   't13':r'$\frac{1}{r} \overline{\tau}_{\theta \theta}$',
+                   }
+        
+        terms_theta = {'t1':r'$\partial_{r}[ \bar{\rho} \tilde{u}_r \tilde{u}_\theta ]$',
+                       't2':r'$\frac{1}{r} \partial_{\theta}[ \bar{\rho} \tilde{u}_\theta \tilde{u}_\theta ]$',
+                       't3':r'$\frac{1}{r} \partial_{\theta}[\bar{p}]$',
+                       't4':r'$-\partial_{r}[ \overline{\tau}_{r \theta} ]$',
+                       't5':r'$\partial_{r}[ \overline{\rho u^{\prime \prime}_r  u^{\prime \prime}_\theta } ]$',
+                       't6':r'$-\frac{1}{r} \partial_{\theta}[ \overline{\tau}_{\theta \theta} ]$',
+                       't7':r'$\frac{1}{r} \partial_{\theta}[ \overline{\rho u^{\prime \prime}_\theta  u^{\prime \prime}_\theta } ]$',
+                       't8':r'$\frac{2}{r} \bar{\rho} \tilde{u}_{r} \tilde{u}_{\theta}$',
+                       't9':r'$\frac{2}{r} \overline{ \rho u^{\prime \prime}_r u^{\prime \prime}_\theta }$',
+                       't10':r'$-\frac{2}{r} \overline{\tau}_{r \theta}$',
+                       }
+        
+        ## create groups
+        for gn in gns:
+            
+            if verbose: print(72*'-')
+            
+            if (gn in self):
+                del self[gn]
+                if verbose: even_print('deleted group',f'/{gn}/')
+            
+            grp = self.create_group(gn)
+            if verbose: even_print('created group',f'{grp.name}/')
+            
+            ## set group attributes
+            grp.attrs['local_csys'] = local_csys
+            if verbose: even_print(f'{gn}.local_csys',str(grp.attrs['local_csys']))
+        
+        gn=None; del gn
+        
+        if verbose: print(72*'-')
+        
+        ## initialize dsets for [x] terms
+        if (csys_type=='cartesian'):
+            for dsn, tag in terms_x.items():
+                shape = (self.ny,self.nx)
+                if (f'{gnx}/{dsn}' in self): del self[f'{gnx}/{dsn}']
+                dset = self.create_dataset(f'{gnx}/{dsn}', 
+                                           shape=shape, 
+                                           dtype=np.float32,
+                                           chunks=None)
+                if verbose: even_print(f'{gnx}/{dsn}',str(shape))
+                dset.attrs['latex'] = tag
+                if verbose: even_print(f'{dsn}.latex',str(dset.attrs['latex']))
+            if verbose: print(72*'-')
+        
+        ## initialize dsets for [y] terms
+        if (csys_type=='cartesian'):
+            for dsn, tag in terms_y.items():
+                shape = (self.ny,self.nx)
+                if (f'{gny}/{dsn}' in self): del self[f'{gny}/{dsn}']
+                dset = self.create_dataset(f'{gny}/{dsn}', 
+                                           shape=shape, 
+                                           dtype=np.float32,
+                                           chunks=None)
+                if verbose: even_print(f'{gny}/{dsn}',str(shape))
+                dset.attrs['latex'] = tag
+                if verbose: even_print(f'{dsn}.latex',str(dset.attrs['latex']))
+            if verbose: print(72*'-')
+        
+        ## initialize dsets for [r] terms
+        if (csys_type=='cylindrical'):
+            for dsn, tag in terms_r.items():
+                shape = (self.ny,self.nx)
+                if (f'{gnr}/{dsn}' in self): del self[f'{gnr}/{dsn}']
+                dset = self.create_dataset(f'{gnr}/{dsn}', 
+                                           shape=shape, 
+                                           dtype=np.float32,
+                                           chunks=None)
+                if verbose: even_print(f'{gnr}/{dsn}',str(shape))
+                dset.attrs['latex'] = tag
+                if verbose: even_print(f'{dsn}.latex',str(dset.attrs['latex']))
+            if verbose: print(72*'-')
+        
+        ## initialize dsets for [θ] terms
+        if (csys_type=='cylindrical'):
+            for dsn, tag in terms_theta.items():
+                shape = (self.ny,self.nx)
+                if (f'{gnt}/{dsn}' in self): del self[f'{gnt}/{dsn}']
+                dset = self.create_dataset(f'{gnt}/{dsn}', 
+                                           shape=shape, 
+                                           dtype=np.float32,
+                                           chunks=None)
+                if verbose: even_print(f'{gnt}/{dsn}',str(shape))
+                dset.attrs['latex'] = tag
+                if verbose: even_print(f'{dsn}.latex',str(dset.attrs['latex']))
+            if verbose: print(72*'-')
+        
+        ## copy data
+        
+        if (csys_type=='cylindrical') and hasattr(self,'crv_R'):
+            crv_R = np.copy(self.crv_R)
+            if verbose: even_print('crv_R',str(crv_R.shape))
+        
+        u   = np.copy( self['data/u'][()].T   )
+        v   = np.copy( self['data/v'][()].T   )
+        #w   = np.copy( self['data/w'][()].T   )
+        rho = np.copy( self['data/rho'][()].T )
+        p   = np.copy( self['data/p'][()].T   )
+        #T   = np.copy( self['data/T'][()].T   )
+        mu  = np.copy( self['data/mu'][()].T  )
+        
+        if verbose: even_print('u',str(u.shape))
+        if verbose: even_print('v',str(v.shape))
+        if verbose: even_print('ρ',str(rho.shape))
+        if verbose: even_print('p',str(p.shape))
+        if verbose: even_print('μ',str(mu.shape))
+        
+        u_Fv = np.copy( self['data/u_Fv'][()].T )
+        v_Fv = np.copy( self['data/v_Fv'][()].T )
+        if verbose: even_print('u_Fv',str(u_Fv.shape))
+        if verbose: even_print('v_Fv',str(v_Fv.shape))
+        
+        r_uII_uII = np.copy( self['data/r_uII_uII'][()].T )
+        r_vII_vII = np.copy( self['data/r_vII_vII'][()].T )
+        #r_wII_wII = np.copy( self['data/r_wII_wII'][()].T )
+        r_uII_vII = np.copy( self['data/r_uII_vII'][()].T )
+        #r_uII_wII = np.copy( self['data/r_uII_wII'][()].T )
+        #r_vII_wII = np.copy( self['data/r_vII_wII'][()].T )
+        if verbose: even_print('ρu′′u′′',str(r_uII_uII.shape))
+        if verbose: even_print('ρu′′v′′',str(r_uII_vII.shape))
+        if verbose: even_print('ρv′′v′′',str(r_vII_vII.shape))
+        
+        x = np.copy(self.x)
+        y = np.copy(self.y)
+        
+        if (x.ndim==1) and (y.ndim==1):
+            x,y = np.meshgrid(x,y, indexing='ij')
+        if verbose: even_print('x',str(x.shape))
+        if verbose: even_print('y',str(y.shape))
+        
+        nx,ny = x.shape
+        
+        if local_csys:
+            
+            # ## calculate grid points for specific postions in char. lengths
+            # s_vert_locs = [-100,-50,-25,0,+25,+50,+100]
+            # svert  = (self.stang-250*self.lchar)/self.lchar
+            # xis    = [ np.abs(s-svert).argmin() for s in s_vert_locs ]
+            
+            if (xis is None):
+                xis = np.arange(self.nx)
+                n_prog = self.nx
+            else:
+                n_prog = len(xis)
+            
+            if (csys_type=='cartesian'):
+                desc='momentum balance [x,y]'
+            elif (csys_type=='cylindrical'):
+                desc='momentum balance [r,θ]'
+            else:
+                raise ValueError
+            
+            if verbose: progress_bar = tqdm(total=n_prog, ncols=100, desc=desc, leave=False, file=sys.stdout)
+            
+            ## iterate through axis=0 indices
+            for xi in xis:
+                
+                rotation_angle_z = np.arcsin(vnorm[xi,0,0])
+                #rotation_angle_z = np.arcsin(-vtang[xi,0,1])
+                #if verbose: tqdm.write( even_print('rotation_angle_z', f'{np.degrees(rotation_angle_z):0.14f} [deg]', s=True) )
+                
+                rotation_matrix_1 = np.array( [[ np.cos(rotation_angle_z) , -np.sin(rotation_angle_z) , 0 ],
+                                               [ np.sin(rotation_angle_z) ,  np.cos(rotation_angle_z) , 0 ],
+                                               [ 0                        ,  0                        , 1 ]], dtype=np.float64 )
+                
+                ## rotation_matrix_2 = np.array( [[ vtang[xi,0,0] ,  vtang[xi,0,1] , 0 ],
+                ##                                [ vnorm[xi,0,0] ,  vnorm[xi,0,1] , 0 ],
+                ##                                [ 0             ,  0             , 1 ]], dtype=np.float64 )
+                ## 
+                ## ## just showing that these are the same
+                ## np.testing.assert_allclose( rotation_matrix_1 , rotation_matrix_2 , rtol=1e-14 , atol=1e-14 )
+                
+                rotation_matrix = np.copy(rotation_matrix_1)
+                
+                ## translate to [cx,cy]
+                cx = x[xi,0]
+                cy = y[xi,0]
+                translation_matrix_A = np.array( [[ 1 , 0 , -cx ],
+                                                  [ 0 , 1 , -cy ],
+                                                  [ 0 , 0 ,  1  ]], dtype=np.float64 )
+                
+                ## translate in [y] by -R (the local curvature radius)
+                if (csys_type=='cylindrical'):
+                    cx = 0.
+                    cy = crv_R[xi]
+                    translation_matrix_B = np.array( [[ 1 , 0 ,  0  ],
+                                                      [ 0 , 1 , -cy ],
+                                                      [ 0 , 0 ,  1  ]], dtype=np.float64 )
+                else:
+                    translation_matrix_B = np.identity(3, dtype=np.float64)
+                
+                ## form the full [3x3] matrix by multiplying together --> order matters!
+                transformation_matrix = np.einsum( 'ij,jk,kl->il', translation_matrix_B , rotation_matrix, translation_matrix_A )
+                
+                # ===
+                
+                ## send to kernel
+                if (csys_type=='cartesian'):
+                    
+                    data_x, data_y = ztmd.momentum_balance_kernel_cartesian(x=x,y=y,
+                                                                            u=u,v=v,
+                                                                            u_Fv=u_Fv,v_Fv=v_Fv,
+                                                                            p=p, rho=rho, mu=mu,
+                                                                            r_uII_uII=r_uII_uII,
+                                                                            r_uII_vII=r_uII_vII,
+                                                                            r_vII_vII=r_vII_vII,
+                                                                            transformation_matrix=transformation_matrix,
+                                                                            acc=acc,edge_stencil=edge_stencil )
+                    
+                    ## write to HDF5 (only data from single axis=0 index)
+                    for dsn, arr in data_x.items():
+                        dset = self[f'{gnx}/{dsn}']
+                        dset[:,xi] = arr[xi,:] ## arrays in HDF5 are transposed
+                    for dsn, arr in data_y.items():
+                        dset = self[f'{gny}/{dsn}']
+                        dset[:,xi] = arr[xi,:]
+                
+                elif (csys_type=='cylindrical'):
+                    
+                    data_r, data_t = ztmd.momentum_balance_kernel_cylindrical(x=x,y=y,
+                                                                              u=u,v=v,
+                                                                              u_Fv=u_Fv,v_Fv=v_Fv,
+                                                                              p=p, rho=rho, mu=mu,
+                                                                              r_uII_uII=r_uII_uII,
+                                                                              r_uII_vII=r_uII_vII,
+                                                                              r_vII_vII=r_vII_vII,
+                                                                              transformation_matrix=transformation_matrix,
+                                                                              acc=acc,edge_stencil=edge_stencil )
+                    
+                    ## write to HDF5 (only data from single axis=0 index)
+                    for dsn, arr in data_r.items():
+                        dset = self[f'{gnr}/{dsn}']
+                        dset[:,xi] = arr[xi,:] ## arrays in HDF5 are transposed
+                    for dsn, arr in data_t.items():
+                        dset = self[f'{gnt}/{dsn}']
+                        dset[:,xi] = arr[xi,:]
+                
+                else:
+                    raise ValueError
+                
+                if verbose: progress_bar.update()
+            if verbose: progress_bar.close()
+        
+        else:
+            
+            ## send to kernel
+            if (csys_type=='cartesian'):
+                
+                data_x, data_y = ztmd.momentum_balance_kernel_cartesian(x=x,y=y,
+                                                                        u=u,v=v,
+                                                                        u_Fv=u_Fv,v_Fv=v_Fv,
+                                                                        p=p, rho=rho, mu=mu,
+                                                                        r_uII_uII=r_uII_uII,
+                                                                        r_uII_vII=r_uII_vII,
+                                                                        r_vII_vII=r_vII_vII,
+                                                                        #transformation_matrix=transformation_matrix,
+                                                                        acc=acc,edge_stencil=edge_stencil )
+                
+                ## write to HDF5 (only data from single axis=0 index)
+                for dsn, arr in data_x.items():
+                    dset = self[f'{gnx}/{dsn}']
+                    dset[:,:] = arr.T ## arrays in HDF5 are transposed
+                for dsn, arr in data_y.items():
+                    dset = self[f'{gny}/{dsn}']
+                    dset[:,:] = arr.T ## arrays in HDF5 are transposed
+            
+            elif (csys_type=='cylindrical'):
+                
+                data_r, data_t = ztmd.momentum_balance_kernel_cylindrical(x=x,y=y,
+                                                                          u=u,v=v,
+                                                                          u_Fv=u_Fv,v_Fv=v_Fv,
+                                                                          p=p, rho=rho, mu=mu,
+                                                                          r_uII_uII=r_uII_uII,
+                                                                          r_uII_vII=r_uII_vII,
+                                                                          r_vII_vII=r_vII_vII,
+                                                                          #transformation_matrix=transformation_matrix,
+                                                                          acc=acc,edge_stencil=edge_stencil )
+                
+                ## write to HDF5 (only data from single axis=0 index)
+                for dsn, arr in data_r.items():
+                    dset = self[f'{gnr}/{dsn}']
+                    dset[:,xi] = arr[xi,:] ## arrays in HDF5 are transposed
+                for dsn, arr in data_t.items():
+                    dset = self[f'{gnt}/{dsn}']
+                    dset[:,xi] = arr[xi,:]
+            
+            else:
+                raise ValueError
         
         self.get_header(verbose=False)
         if verbose: print(72*'-')
-        if verbose: print('total time : ztmd.calc_momentum_balance_y_terms() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print('total time : ztmd.calc_momentum_balance_terms() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
     # === post-processing: 1D profiles
     
     def calc_bl_edge(self, **kwargs):
@@ -21298,27 +22704,32 @@
         rho_edge = np.copy( data_edge['rho_edge'] )
         
         if self.curvilinear:
             utang_edge = np.copy( data_edge['utang_edge'] )
         
         if self.rectilinear:
             
-            cf_1   = np.copy( 2. * (u_tau/u_edge)**2 * (rho_wall/rho_edge) )
-            cf_2   = np.copy( 2. * tau_wall / (rho_edge*u_edge**2) )
+            # cf_1   = np.copy( 2. * (u_tau/u_edge)**2 * (rho_wall/rho_edge) )
+            # cf_2   = np.copy( 2. * tau_wall / (rho_edge*u_edge**2) )
+            # np.testing.assert_allclose(cf_1, cf_2, rtol=1e-6, atol=1e-8)
+            # cf = np.copy(cf_2)
+            
             cf_inf = np.copy( 2. * tau_wall / ( self.rho_inf * self.U_inf**2 ) )
-            np.testing.assert_allclose(cf_1,   cf_2, rtol=1e-6, atol=1e-8)
-            #np.testing.assert_allclose(cf_inf, cf_2, rtol=1e-6, atol=1e-8) ## fails --> Max relative difference: 0.067
-            #cf = np.copy(cf_2)
             cf = np.copy(cf_inf)
         
         elif self.curvilinear:
-            cf_1 = 2. * (u_tau/utang_edge)**2 * (rho_wall/rho_edge)
-            cf_2 = 2. * tau_wall / (rho_edge*utang_edge**2)
-            np.testing.assert_allclose(cf_1, cf_2, rtol=1e-6, atol=1e-8)
-            cf = np.copy(cf_2)
+            
+            # cf_1 = 2. * (u_tau/utang_edge)**2 * (rho_wall/rho_edge)
+            # cf_2 = 2. * tau_wall / (rho_edge*utang_edge**2)
+            # np.testing.assert_allclose(cf_1, cf_2, rtol=1e-6, atol=1e-8)
+            # cf = np.copy(cf_2)
+            
+            cf_inf = np.copy( 2. * tau_wall / ( self.rho_inf * self.U_inf**2 ) )
+            cf = np.copy(cf_inf)
+        
         else:
             raise ValueError
         
         if ('data_1Dx/cf' in self): del self['data_1Dx/cf']
         self.create_dataset('data_1Dx/cf', data=cf, chunks=None)
         if verbose: even_print('data_1Dx/cf', '%s'%str(cf.shape))
         
@@ -24532,15 +25943,18 @@
     if isinstance(obj,h5py._hl.dataset.Dataset):
         print(shift + item_name + ' --> shape=%s, dtype=%s'%( str(obj.shape), str(obj.dtype) ) )
     else:
         print(shift + item_name)
     
     ## print attributes
     for key, val in obj.attrs.items():
-        print(shift + 2*' ' + f'{key} = {str(val)} --> dtype={str(val.dtype)}')
+        try:
+            print(shift + 2*' ' + f'{key} = {str(val)} --> dtype={str(val.dtype)}')
+        except:
+            print(shift + 2*' ' + f'{key} = {str(val)} --> type={str(type(val).__name__)}')
 
 class h5_visit_container:
     '''
     callable for input to h5py.Group.visit() which stores dataset/group names
     '''
     def __init__(self):
         self.names = []
@@ -24985,15 +26399,15 @@
         elif (curveType=='power_plus_const'):
             '''
             power law (plus a constant) y = a + b·(x^c)
             no longer a straight line on log-log but allows non-zero y-intercept
             '''
             def curve(x, a, b, c):
                 return a + b*np.power(x,c)
-
+        
         elif (curveType=='power_asymp'):
             '''
             power asymptotic
             '''
             def curve(x, a, b, c, d):
                 return a/(b + c*np.power(x,d))
         
@@ -27174,29 +28588,14 @@
         $> rm ~/.cache/matplotlib/fontlist-v330.json
         $> rm -rf ~/.cache/matplotlib/tex.cache
     
     Windows
     -------
     --> download, install, then delete : C:/Users/%USERNAME%/.matplotlib/fontlist-v330.json
     --> this JSON file will get regenerated with newly installed fonts
-    
-    MikTeX .sty files --> global (sometimes needed for journals)
-    -----------------
-    - https://miktex.org/faq/local-additions
-    - in C:/Users/%USERNAME%/AppData/Local  : make : mytextmf\tex\latex\mystuff
-    - register as root directory in MikTeX
-    - put .sty files in there
-    
-    Dimension Presets: Springer 'svjour3' Template
-    ----------------------------------------------
-    ltx_textwidth  = 6.85066
-    ltx_hsize      = 3.30719 # \linewidth
-    ltx_textheight = 9.2144 * 0.90 ### error if fig is actually this tall, so effective max *= 0.90
-    ltx_vsize      = 9.2144 * 0.90
-    
     '''
     
     useTex   = kwargs.get('useTex',False) ## use LaTeX text rendering
     darkMode = kwargs.get('darkMode',True)
     font     = kwargs.get('font',None)
     
     ## mpl.rcParams.update(mpl.rcParamsDefault) ## reset rcparams to defaults
@@ -27208,24 +28607,26 @@
     
     if useTex:
         
         ## 'Text rendering with LaTeX'
         ## https://matplotlib.org/stable/tutorials/text/usetex.html
         
         mpl.rcParams['text.usetex'] = True
-        #mpl.rcParams['pgf.texsystem'] = 'xelatex' ## 'xelatex', 'lualatex', 'pdflatex' --> xelatex seems to be fastest
+        mpl.rcParams['pgf.texsystem'] = 'pdflatex' ## 'xelatex', 'lualatex', 'pdflatex' --> xelatex seems to be fastest
         
-        preamble_opts = [ r'\usepackage[T1]{fontenc}',
-                          #r'\usepackage[utf8]{inputenc}',
+        preamble_opts = [ r'\usepackage[utf8]{inputenc}',
+                          r'\usepackage[T1]{fontenc}',
                           r'\usepackage{amsmath}', 
                           r'\usepackage{amsfonts}',
                           #r'\usepackage{amssymb}',
                           r'\usepackage{gensymb}', ## Generic symbols 
-                          r'\usepackage{xfrac}',
+                          #r'\usepackage{xfrac}',
                           #r'\usepackage{nicefrac}',
+                          ##r'\usepackage{newtxtext}',
+                          #r'\usepackage{newtxmath}',
                           ]
         
         if (font==None): ## default
             mpl.rcParams['font.family']= 'serif'
             mpl.rcParams['font.serif'] = 'Computer Modern Roman'
         
         elif (font=='IBM Plex Sans') or (font=='IBM Plex') or (font=='IBM') or (font=='ibm'):
@@ -27407,15 +28808,15 @@
     
     ## ## list all options
     ## print(mpl.rcParams.keys())
     
     fontsize = 10
     axesAndTickWidth = 0.5
     
-    mpl.rcParams['figure.figsize'] = 3*2, 3
+    mpl.rcParams['figure.figsize'] = 3*(16/9), 3
     mpl.rcParams['figure.dpi']     = 300
     #mpl.rcParams['figure.facecolor'] = 'k'
     #mpl.rcParams['figure.autolayout'] = True ### tight_layout() --> just use instead : fig1.tight_layout(pad=0.20)
     
     #mpl.rcParams['figure.constrained_layout.use'] = True
     #mpl.rcParams['figure.constrained_layout.h_pad']  = 0.0 ## Padding around axes objects. Float representing
     #mpl.rcParams['figure.constrained_layout.w_pad']  = 0.0 ## inches. Default is 3/72 inches (3 points)
@@ -27450,38 +28851,38 @@
     #mpl.rcParams['ytick.color'] = 'k' ## set with mpl.style.use()
     mpl.rcParams['ytick.direction'] = 'in'
     
     mpl.rcParams['xtick.labelsize'] = fontsize
     mpl.rcParams['ytick.labelsize'] = fontsize
     
     mpl.rcParams['xtick.major.pad'] = 3.0
-    mpl.rcParams['ytick.major.pad'] = 1.0
+    mpl.rcParams['ytick.major.pad'] = 2.0
     
-    mpl.rcParams['lines.linewidth']  = 0.8
+    mpl.rcParams['lines.linewidth']  = 1.0
     mpl.rcParams['lines.linestyle']  = 'solid'
     mpl.rcParams['lines.marker']     = 'None' #'o'
     mpl.rcParams['lines.markersize'] = 1.2
     mpl.rcParams['lines.markeredgewidth'] = 0.
     
     #mpl.rcParams['axes.facecolor'] = 'k' ## set with mpl.style.use()
     mpl.rcParams['axes.linewidth'] = axesAndTickWidth
     mpl.rcParams['axes.labelpad']  = 3.0
     mpl.rcParams['axes.titlesize'] = fontsize
     mpl.rcParams['axes.labelsize'] = fontsize
     mpl.rcParams['axes.formatter.use_mathtext'] = True
     mpl.rcParams['axes.axisbelow'] = False ## dont allow axes, ticks to be under lines --> doesn't work for artist objects with zorder >2.5
     
-    mpl.rcParams['legend.fontsize'] = fontsize*0.8
+    mpl.rcParams['legend.fontsize'] = fontsize
     mpl.rcParams['legend.shadow']   = False
-    mpl.rcParams['legend.borderpad'] = 0.5
+    mpl.rcParams['legend.borderpad'] = 0.3
     mpl.rcParams['legend.framealpha'] = 1.0
     mpl.rcParams['legend.edgecolor']  = 'inherit'
     mpl.rcParams['legend.handlelength'] = 1.0
     mpl.rcParams['legend.handletextpad'] = 0.4
-    mpl.rcParams['legend.borderaxespad'] = 0.7
+    mpl.rcParams['legend.borderaxespad'] = 0.6
     mpl.rcParams['legend.columnspacing'] = 0.5
     mpl.rcParams['legend.fancybox'] = False
     
     return
 
 def colors_table():
     '''
@@ -27793,14 +29194,66 @@
     ## do shift
     for ai, axis in enumerate(list_of_axes):
         x0n, y0n, dxn, dyn = ax_tb_pct[ai,:]
         axis.set_position( [ x0n*(w/w_adj) , y0n , dxn*(w/w_adj) , dyn ] )
     
     return
 
+def axs_grid_initializer(**kwargs):
+    '''
+    initialize several axes in a grid
+    '''
+    
+    w_prop    = kwargs.get('w_prop',True) ## peg to width vals
+    figsize_x = kwargs.get('figsize_x',6)
+    figsize_y = kwargs.get('figsize_y',4) ## figsizes in 
+    mrg_l     = kwargs.get('mrg_l',0.05)
+    mrg_r     = kwargs.get('mrg_r',0.05)
+    mrg_w     = kwargs.get('mrg_w',0.05)
+    mrg_t     = kwargs.get('mrg_t',0.05)
+    mrg_b     = kwargs.get('mrg_b',0.05)
+    mrg_h     = kwargs.get('mrg_h',0.05)
+    
+    cols = kwargs.get('cols',2)
+    rows = kwargs.get('rows',1)
+    
+    dpi_fig = kwargs.get('dpi_fig',110)
+    
+    
+    fig = plt.figure(figsize=(figsize_x,figsize_y), dpi=dpi_fig)
+    aspect = figsize_x/figsize_y
+    if w_prop:
+        mrg_t *= aspect
+        mrg_b *= aspect
+        mrg_h *= aspect
+    
+    ax_width  = (1.0 - (cols-1)*mrg_w - mrg_l - mrg_r)/cols
+    ax_height = (1.0 - (rows-1)*mrg_h - mrg_t - mrg_b)/rows
+    axs          = np.zeros(shape=(cols,rows),   dtype=object)
+    ax_grid_dims = np.zeros(shape=(cols,rows,4), dtype=np.float64) ## the original axis positions
+    for j in range(rows):
+        for i in range(cols):
+            ii = i ## left to right
+            jj = (rows-1) - j ## top to bottom
+            x0 = mrg_l + ii*mrg_w + ii*ax_width
+            dx = ax_width
+            y0 = mrg_b + jj*mrg_h + jj*ax_height
+            dy = ax_height
+            ax = fig.add_axes([x0,y0,dx,dy])
+            
+            ax_grid_dims[i,j,:] = x0,y0,dx,dy
+            axs[i,j] = ax
+    
+    ## axs          = np.asarray(axs)
+    ## ax_grid_dims = np.asarray(ax_grid_dims, dtype=object)
+    ## axs          = np.reshape(axs,          (cols, rows),    order='F')
+    ## ax_grid_dims = np.reshape(ax_grid_dims, (cols, rows, 4), order='F') ; print(ax_grid_dims.shape)
+    
+    return fig, axs, ax_grid_dims
+
 def axs_grid_compress(fig,axs,**kwargs):
     '''
     compress ax grid
     '''
     dim = kwargs.get('dim',1)
     offset_px = kwargs.get('offset_px',5)
     transFigInv = fig.transFigure.inverted()
```

### Comparing `turbx-0.3.2/turbx.egg-info/PKG-INFO` & `turbx-0.3.3/turbx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbx
-Version: 0.3.2
+Version: 0.3.3
 Summary: Extensible toolkit for analyzing turbulent flow datasets
 Home-page: https://github.com/iagappel/turbx
 Author: Jason A
 Maintainer: Jason A
 License: MIT
 Keywords: scientific computing,statistics,simulation,turbulence,turbulent flows,direct numerical simulation,DNS,parallel,visualization
 Platform: any
```

