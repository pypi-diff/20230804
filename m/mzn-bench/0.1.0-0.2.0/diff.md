# Comparing `tmp/mzn-bench-0.1.0.tar.gz` & `tmp/mzn_bench-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mzn-bench-0.1.0.tar", last modified: Mon Feb  8 00:12:34 2021, max compression
+gzip compressed data, was "mzn_bench-0.2.0.tar", max compression
```

## Comparing `mzn-bench-0.1.0.tar` & `mzn_bench-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,14 @@
-drwxr-xr-x   0 dekker1    (501) staff       (20)        0 2021-02-08 00:12:34.852641 mzn-bench-0.1.0/
-drwxr-xr-x   0 dekker1    (501) staff       (20)        0 2021-02-08 00:12:34.841192 mzn-bench-0.1.0/.github/
-drwxr-xr-x   0 dekker1    (501) staff       (20)        0 2021-02-08 00:12:34.843650 mzn-bench-0.1.0/.github/workflows/
--rw-r--r--   0 dekker1    (501) staff       (20)      864 2021-02-08 00:01:53.000000 mzn-bench-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 dekker1    (501) staff       (20)     1457 2021-02-01 03:43:25.000000 mzn-bench-0.1.0/.gitignore
--rw-r--r--   0 dekker1    (501) staff       (20)    11702 2021-02-08 00:12:34.852107 mzn-bench-0.1.0/PKG-INFO
--rw-r--r--   0 dekker1    (501) staff       (20)     9451 2021-02-04 03:10:32.000000 mzn-bench-0.1.0/README.md
--rw-r--r--   0 dekker1    (501) staff       (20)       38 2021-02-08 00:12:34.852819 mzn-bench-0.1.0/setup.cfg
--rw-r--r--   0 dekker1    (501) staff       (20)     1089 2021-02-04 03:10:32.000000 mzn-bench-0.1.0/setup.py
-drwxr-xr-x   0 dekker1    (501) staff       (20)        0 2021-02-08 00:12:34.841613 mzn-bench-0.1.0/src/
-drwxr-xr-x   0 dekker1    (501) staff       (20)        0 2021-02-08 00:12:34.845407 mzn-bench-0.1.0/src/mzn_bench/
--rw-r--r--   0 dekker1    (501) staff       (20)       62 2021-02-04 03:10:32.000000 mzn-bench-0.1.0/src/mzn_bench/__init__.py
-drwxr-xr-x   0 dekker1    (501) staff       (20)        0 2021-02-08 00:12:34.849609 mzn-bench-0.1.0/src/mzn_bench/analysis/
--rw-r--r--   0 dekker1    (501) staff       (20)        0 2021-02-04 03:10:32.000000 mzn-bench-0.1.0/src/mzn_bench/analysis/__init__.py
--rw-r--r--   0 dekker1    (501) staff       (20)     2684 2021-02-04 03:10:32.000000 mzn-bench-0.1.0/src/mzn_bench/analysis/collect.py
--rw-r--r--   0 dekker1    (501) staff       (20)     9666 2021-02-04 03:10:32.000000 mzn-bench-0.1.0/src/mzn_bench/analysis/plot.py
--rw-r--r--   0 dekker1    (501) staff       (20)     1483 2021-02-04 03:10:32.000000 mzn-bench-0.1.0/src/mzn_bench/analysis/report_status.py
--rw-r--r--   0 dekker1    (501) staff       (20)     7191 2021-02-04 03:10:32.000000 mzn-bench-0.1.0/src/mzn_bench/cli.py
--rw-r--r--   0 dekker1    (501) staff       (20)     8517 2021-02-08 00:01:53.000000 mzn-bench-0.1.0/src/mzn_bench/mzn_slurm.py
-drwxr-xr-x   0 dekker1    (501) staff       (20)        0 2021-02-08 00:12:34.851313 mzn-bench-0.1.0/src/mzn_bench/pytest/
--rw-r--r--   0 dekker1    (501) staff       (20)        0 2021-02-04 03:10:32.000000 mzn-bench-0.1.0/src/mzn_bench/pytest/__init__.py
--rw-r--r--   0 dekker1    (501) staff       (20)     5644 2021-02-04 03:10:32.000000 mzn-bench-0.1.0/src/mzn_bench/pytest/check_solutions.py
--rw-r--r--   0 dekker1    (501) staff       (20)     1870 2021-02-04 03:10:32.000000 mzn-bench-0.1.0/src/mzn_bench/pytest/check_statuses.py
-drwxr-xr-x   0 dekker1    (501) staff       (20)        0 2021-02-08 00:12:34.847756 mzn-bench-0.1.0/src/mzn_bench.egg-info/
--rw-r--r--   0 dekker1    (501) staff       (20)    11702 2021-02-08 00:12:34.000000 mzn-bench-0.1.0/src/mzn_bench.egg-info/PKG-INFO
--rw-r--r--   0 dekker1    (501) staff       (20)      616 2021-02-08 00:12:34.000000 mzn-bench-0.1.0/src/mzn_bench.egg-info/SOURCES.txt
--rw-r--r--   0 dekker1    (501) staff       (20)        1 2021-02-08 00:12:34.000000 mzn-bench-0.1.0/src/mzn_bench.egg-info/dependency_links.txt
--rw-r--r--   0 dekker1    (501) staff       (20)       70 2021-02-08 00:12:34.000000 mzn-bench-0.1.0/src/mzn_bench.egg-info/entry_points.txt
--rw-r--r--   0 dekker1    (501) staff       (20)      106 2021-02-08 00:12:34.000000 mzn-bench-0.1.0/src/mzn_bench.egg-info/requires.txt
--rw-r--r--   0 dekker1    (501) staff       (20)       10 2021-02-08 00:12:34.000000 mzn-bench-0.1.0/src/mzn_bench.egg-info/top_level.txt
+-rw-r--r--   0        0        0    10350 2023-07-18 00:15:50.405088 mzn_bench-0.2.0/README.md
+-rw-r--r--   0        0        0      884 2023-08-03 23:47:27.032559 mzn_bench-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      182 2023-07-19 01:10:02.591402 mzn_bench-0.2.0/src/mzn_bench/__init__.py
+-rw-r--r--   0        0        0        0 2021-02-04 03:10:32.000000 mzn_bench-0.2.0/src/mzn_bench/analysis/__init__.py
+-rw-r--r--   0        0        0     9798 2023-07-19 01:10:02.677358 mzn_bench-0.2.0/src/mzn_bench/analysis/analyse_changes.py
+-rw-r--r--   0        0        0     3111 2023-07-18 00:15:50.406004 mzn_bench-0.2.0/src/mzn_bench/analysis/collect.py
+-rw-r--r--   0        0        0     9687 2023-08-03 23:47:27.032998 mzn_bench-0.2.0/src/mzn_bench/analysis/plot.py
+-rw-r--r--   0        0        0     3303 2021-06-15 00:03:55.000000 mzn_bench-0.2.0/src/mzn_bench/analysis/report_status.py
+-rw-r--r--   0        0        0     9444 2023-07-19 01:10:02.675612 mzn_bench-0.2.0/src/mzn_bench/cli.py
+-rw-r--r--   0        0        0    10956 2023-07-19 01:10:02.703121 mzn_bench-0.2.0/src/mzn_bench/mzn_slurm.py
+-rw-r--r--   0        0        0        0 2021-02-04 03:10:32.000000 mzn_bench-0.2.0/src/mzn_bench/pytest/__init__.py
+-rw-r--r--   0        0        0     5635 2023-07-18 00:15:50.406802 mzn_bench-0.2.0/src/mzn_bench/pytest/check_solutions.py
+-rw-r--r--   0        0        0     1977 2023-07-18 00:15:50.407014 mzn_bench-0.2.0/src/mzn_bench/pytest/check_statuses.py
+-rw-r--r--   0        0        0    11262 1970-01-01 00:00:00.000000 mzn_bench-0.2.0/PKG-INFO
```

### Comparing `mzn-bench-0.1.0/PKG-INFO` & `mzn_bench-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,238 +1,263 @@
 Metadata-Version: 2.1
 Name: mzn-bench
-Version: 0.1.0
-Summary: SLURM scheduling functionality and a collection of scripts to process the resulting data.
-Home-page: https://www.minizinc.org/
+Version: 0.2.0
+Summary: SLURM scheduling functionality and a collection of scripts to process the resulting data
+License: MPL-2.0
 Author: Jip J. Dekker
 Author-email: jip.dekker@monash.edu
-License: UNKNOWN
-Project-URL: Source, https://github.com/MiniZinc/mzn-bench
-Description: # MiniZinc Bench
-        
-        This is a small collection of scripts that allow you to run benchmarks on a set
-        of MiniZinc instance using MiniZinc Python. The process is split into several
-        steps to be easily customisable to different kinds of possible benchmarks.
-        
-        > Currently, the only supported way of running benchmarks is through
-        > [SLURM](https://slurm.schedmd.com/). Other methods may become available in the
-        > future.
-        
-        ## Preparation
-        
-        1. Create a CSV file for the MiniZinc instances containing _problem_, _model_,
-           _data_file_. If you store the instances in the MiniZinc benchmarks
-           repository structure, then you can use the `mzn-bench collect-instances`
-           command:
-           ```bash
-           mzn-bench collect-instances <directory> > instances.csv
-           ```
-        2. Instantiate a benchmarking environment. This environment should at least
-           contain a Python virtual environment with _mzn-bench_ and your benchmarking
-           scripts, but you can also set up environmental variables, like `PATH`, and
-           load cluster modules. The following script, `bench_env.sh`,
-           provides an example environment that can be loaded using `source bench_env.sh`:
-        
-           ```bash
-           if [[ "${BASH_SOURCE[0]}" = "${0}" ]]; then
-               >&2 echo "Remember: you need to run me as 'source ${0}', not execute it!"
-               exit
-           fi
-        
-           # Create or activate Python virtual environment
-           if [ -d venv ]; then
-               source venv/bin/activate
-           else
-              python3 -m venv venv
-               source venv/bin/activate
-               python3 -m pip install mzn-bench
-           fi
-        
-           # Set other environment variables and load cluster modules
-           module load MiniZinc/2.4.3
-           ```
-        
-        3. Create a benchmarking script. This script will contain the configuration of
-           where the instance file is located, what MiniZinc/Solver configurations to
-           run for every instance, and how the benchmark runner itself should be
-           configured. The script mainly consists of a call to `schedule` in
-           `mzn_bench`. For example a benchmarking script that runs Gecode and
-           Chuffed for 20 minutes might look like this:
-        
-           ```python
-           from datetime import timedelta
-           from pathlib import Path
-        
-           import minizinc
-        
-           from mzn_bench import Configuration, schedule
-        
-           schedule(
-               instances=Path("./instances.csv"),
-               timeout=timedelta(minutes=20),
-               configurations=[
-                   Configuration(name="Gecode", solver=minizinc.Solver.lookup("gecode")),
-                   Configuration(name="Chuffed", solver=minizinc.Solver.lookup("chuffed")),
-               ],
-               nodelist=["critical001"],
-           )
-           ```
-        
-        These are all the possible arguments to `schedule`:
-        
-        - `instances: Path` - The path to the instances file.
-        - `timeout: timedelta` - The timeout set for the MiniZinc process.
-        - `configurations: Iterable[Configuration]` - MiniZinc solving configurations
-          (see below for details).
-        - `nodelist: Iterable[str]` - A list of nodes on which SLURM is allowed to
-          schedule the tasks.
-        - `output_dir: Path = Path.cwd() / "results"` - The directory in which the raw
-          results will be placed. This directory will be created if it does not yet
-          exist.
-        - `job_name: str = "MiniZinc Benchmark"` - The SLURM job name.
-        - `cpus_per_task: int = 1` - The number of CPU cores required for each task.
-        - `memory: int = 4096` - The maximum memory used for each task.
-        - `debug: bool = False` - Directly capture the output of individual jobs
-          and store them in a `./logs/` directory.
-        - `wait: bool = False` - The scheduling process will wait for all jobs to
-          finish.
-        
-        A `Configuration` object has the following attributes:
-        
-        - `name: str` - Configuration name used in the output.
-        - `solver: minizinc.Solver` - MiniZinc Python solver configuration.
-        - `minizinc: Optional[Path] = None` - Path to a specific MiniZinc executable.
-          If `None` is provided, then the first `minizinc` executable on the `PATH`
-          will be used.
-        - `processes: Optional[int] = None` - Number of processes to be used by the
-          solver.
-        - `random_seed: Optional[int] = None` - Random seed to be used by the solver.
-        - `free_search: bool = False` - Solver can determine its own search heuristic.
-        - `optimisation_level: Optional[int] = None` - MiniZinc compilation
-          optimisation level, e.g., `-O3`.
-        - `other_flags: Dict[str, Any] = field(default_factory=dict)` - A mapping of
-          flag name to value of other flags to be provided to the compiler/solver
-        - `extra_data: Dict[str, Any] = field(default_factory=dict)` - Extra data to be
-          added when using a specific Configuration. Internally this will be used by
-          MiniZinc Python's `__setitem__` method on the generated instances. If data
-          needs the value of an identifier internal to MiniZinc, then please use an
-          `DZNExpression` object (e.g., `{"preferred_encoding": DZNExpression("UNARY")}`).
-        
-        ## Schedule SLURM jobs
-        
-        The job now has to be started on the cluster with the right number of tasks
-        (one for every instance/solver combination). Luckily, the benchmarking script
-        that you've created in the previous step should take care of all of this.
-        So once we ensure that our environment is ready for ou benchmark, we can
-        execute our script and our job will be scheduled.
-        
-        For example, if we had created a script `bench_env.sh` with our benchmarking
-        environment and a script `start_bench.py` with our `schedule` call, then the
-        following code should schedule our job:
-        
-        ```bash
-        source bench_env.sh
-        python start_bench.py
-        ```
-        
-        You can keep track of the status of your job using the `squeue` command.
-        
-        **WARNING:** Once the job has started the CSV file containing the instances and
-        the instance files themselves should not be changed or moved until the full
-        benchmark is finished. This could causes error or, even worse, inconsistent
-        results.
-        
-        **Note:** If you find a mistake after you have scheduled your job, then you
-        should cancel the job as soon as possible. This can be done by using the
-        `scancel` command. This command will take the `job_id`, shown when your job is
-        scheduled, as an argument.
-        
-        ## Collect information
-        
-        Once the job is finished, it is time to get your data wrangling pants on! This
-        repository contains some scripts that might be helpful in locating and
-        formatting the information that you need. Some scripts might be used directly
-        while other might need some customising to fit your purpose. Note that these
-        scripts might require some extra dependencies. For this reason, these scripts
-        are not expected to work unless this package is installed as
-        `pip install mzn-bench[scripts]`.
-        This allows us to install a minimal version on the running cluster and this
-        more complete version locally while processing the data.
-        
-        ### General aggregation
-        
-        The following scripts can help gather the raw `*_stats.yml`/`*_sol.yml` files
-        and combine them for further use:
-        
-        - `mzn-bench collect-objectives <result_dir> <objectives.csv>` -
-          This script gathers all objective value information given by MiniZinc and the
-          used solvers and combines it into a single CSV file.
-        - `mzn-bench collect-statistics <result_dir> <statistics.csv>` -
-          This script gathers all statistical information given by MiniZinc and the used
-          solvers and combines it into a single CSV file.
-        
-        ### Tabulation
-        
-        The following scripts filter and tabulate specific statistics.
-        
-        - `mzn-bench report-status <statistics.csv>` - This script will report the
-          number of occurrences of the various solving status of your MiniZinc tasks.
-          Please consult the `-h` flag to display all options.
-        
-        ### Solution checking
-        
-        The `mzn-bench check-solutions` command takes the solutions output during run
-        and feeds them back into the model to check that the result is satisfiable.
-        It also stores the objective and satisfiability information to be used when
-        checking statuses. The `-c` option can be used to set how many solutions
-        to check (zero to check all solutions).
-        
-        ```bash
-        # Check three solutions from each instance
-        mzn-bench check-solutions -c 3 ./results
-        ```
-        
-        This requires the problem `.mzn` and `.dzn` files from the benchmark run to be
-        available in order to run the checker. The `--base-dir <DIR>` option can be used
-        to specify a root directory relative to which the file names in the
-        `*_sol.yml` files are resolved.
-        
-        ### Status checking
-        
-        The `mzn-bench check-statuses` command takes the results from `check-solutions`
-        command above (which must be run first) and then checks for any solvers which
-        have either
-        
-        - Falsely claimed optimality - where optimality was found by a solver, but a
-          better objective was found elsewhere and verified to be correct.
-        - Falsely claimed unsatisfiability - where unsatisfiability was found by a
-          solver, but another solver has given a correct solution for the instance.
-        
-        ### Graph generation
-        
-        There are a number of plotting helper functions available in
-        `mzn_bench.analysis.plot`. In order to use these, you must enable the
-        plotting features with `pip install mzn-bench[plotting]`. These use the
-        [Bokeh](https://bokeh.org/) visualisation library to provide interactive plots.
-        
-        The `read_csv` function returns a tuple of [pandas](https://pandas.pydata.org/)
-        data frames containing objective and statistics data for plotting or further
-        data analysis.
-        
-        ```py
-        from mzn_bench.analysis.collect import read_csv
-        from mzn_bench.analysis.plot import plot_all_instances
-        from bokeh.plotting import show
-        
-        # Read CSVs generated by mzn-bench collect-result as pandas dataframes
-        objs, stats = read_csv("objectives.csv", "statistics.csv")
-        
-        # Grid plot giving objective values over time, or time to solve
-        # (depending on instance type)
-        show(plot_all_instances(objs, stats))
-        ```
-        
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: plotting
 Provides-Extra: scripts
+Requires-Dist: bokeh (>=3,<4) ; extra == "plotting"
+Requires-Dist: click (>=8.1,<9.0)
+Requires-Dist: minizinc (>=0.9,<0.10)
+Requires-Dist: pandas (>=2.0,<3.0) ; extra == "scripts"
+Requires-Dist: ruamel-yaml (>=0.17,<0.18)
+Requires-Dist: tabulate (>=0.9,<0.10) ; extra == "scripts"
+Description-Content-Type: text/markdown
+
+# MiniZinc Bench
+
+This is a small collection of scripts that allow you to run benchmarks on a set
+of MiniZinc instance using MiniZinc Python. The process is split into several
+steps to be easily customisable to different kinds of possible benchmarks.
+
+> Currently, the only supported way of running benchmarks is through
+> [SLURM](https://slurm.schedmd.com/). Other methods may become available in the
+> future.
+
+## Preparation
+
+1. Create a CSV file for the MiniZinc instances containing _problem_, _model_,
+   _data_file_. If you store the instances in the MiniZinc benchmarks
+   repository structure, then you can use the `mzn-bench collect-instances`
+   command:
+   ```bash
+   mzn-bench collect-instances <directory> > instances.csv
+   ```
+2. Instantiate a benchmarking environment. This environment should at least
+   contain a Python virtual environment with _mzn-bench_ and your benchmarking
+   scripts, but you can also set up environmental variables, like `PATH`, and
+   load cluster modules. The following script, `bench_env.sh`,
+   provides an example environment that can be loaded using `source bench_env.sh`:
+
+   ```bash
+   if [[ "${BASH_SOURCE[0]}" = "${0}" ]]; then
+       >&2 echo "Remember: you need to run me as 'source ${0}', not execute it!"
+       exit
+   fi
+
+   # Create or activate Python virtual environment
+   if [ -d venv ]; then
+       source venv/bin/activate
+   else
+      python3 -m venv venv
+       source venv/bin/activate
+       python3 -m pip install mzn-bench
+   fi
+
+   # Set other environment variables and load cluster modules
+   module load MiniZinc/2.4.3
+   ```
+
+3. Create a benchmarking script. This script will contain the configuration of
+   where the instance file is located, what MiniZinc/Solver configurations to
+   run for every instance, and how the benchmark runner itself should be
+   configured. The script mainly consists of a call to `schedule` in
+   `mzn_bench`. For example a benchmarking script that runs Gecode and
+   Chuffed for 20 minutes might look like this:
+
+   ```python
+   from datetime import timedelta
+   from pathlib import Path
+
+   import minizinc
+
+   from mzn_bench import Configuration, schedule
+
+   schedule(
+       instances=Path("./instances.csv"),
+       timeout=timedelta(minutes=20),
+       configurations=[
+           Configuration(name="Gecode", solver=minizinc.Solver.lookup("gecode")),
+           Configuration(name="Chuffed", solver=minizinc.Solver.lookup("chuffed")),
+       ],
+       nodelist=["critical001"],
+   )
+   ```
+
+These are all the possible arguments to `schedule`:
+
+- `instances: Path` - The path to the instances file.
+- `timeout: timedelta` - The timeout set for the MiniZinc process.
+- `configurations: Iterable[Configuration]` - MiniZinc solving configurations
+  (see below for details).
+- `nodelist: Optional[Iterable[str]]` - A list of nodes on which SLURM is allowed to
+  schedule the tasks. If `None`, `mzn-bench` will sequentially solve the instances locally.
+- `output_dir: Path = Path.cwd() / "results"` - The directory in which the raw
+  results will be placed. This directory will be created if it does not yet
+  exist.
+- `job_name: str = "MiniZinc Benchmark"` - The SLURM job name.
+- `cpus_per_task: int = 1` - The number of CPU cores required for each task.
+- `memory: int = 4096` - The maximum memory used for each task.
+- `debug: bool = False` - Directly capture the output of individual jobs
+  and store them in a `./logs/` directory.
+- `wait: bool = False` - The scheduling process will wait for all jobs to
+  finish.
+
+A `Configuration` object has the following attributes:
+
+- `name: str` - Configuration name used in the output.
+- `solver: minizinc.Solver` - MiniZinc Python solver configuration.
+- `minizinc: Optional[Path] = None` - Path to a specific MiniZinc executable.
+  If `None` is provided, then the first `minizinc` executable on the `PATH`
+  will be used.
+- `processes: Optional[int] = None` - Number of processes to be used by the
+  solver.
+- `random_seed: Optional[int] = None` - Random seed to be used by the solver.
+- `free_search: bool = False` - Solver can determine its own search heuristic.
+- `optimisation_level: Optional[int] = None` - MiniZinc compilation
+  optimisation level, e.g., `-O3`.
+- `other_flags: Dict[str, Any] = field(default_factory=dict)` - A mapping of
+  flag name to value of other flags to be provided to the compiler/solver
+- `extra_data: Dict[str, Any] = field(default_factory=dict)` - Extra data to be
+  added when using a specific Configuration. Internally this will be used by
+  MiniZinc Python's `__setitem__` method on the generated instances. If data
+  needs the value of an identifier internal to MiniZinc, then please use an
+  `DZNExpression` object (e.g., `{"preferred_encoding": DZNExpression("UNARY")}`).
+
+## Schedule SLURM jobs
+
+The job now has to be started on the cluster with the right number of tasks
+(one for every instance/solver combination). Luckily, the benchmarking script
+that you've created in the previous step should take care of all of this.
+So once we ensure that our environment is ready for ou benchmark, we can
+execute our script and our job will be scheduled.
+
+For example, if we had created a script `bench_env.sh` with our benchmarking
+environment and a script `start_bench.py` with our `schedule` call, then the
+following code should schedule our job:
+
+```bash
+source bench_env.sh
+python start_bench.py
+```
+
+You can keep track of the status of your job using the `squeue` command.
+
+**WARNING:** Once the job has started the CSV file containing the instances and
+the instance files themselves should not be changed or moved until the full
+benchmark is finished. This could causes error or, even worse, inconsistent
+results.
+
+**Note:** If you find a mistake after you have scheduled your job, then you
+should cancel the job as soon as possible. This can be done by using the
+`scancel` command. This command will take the `job_id`, shown when your job is
+scheduled, as an argument.
+
+## Collect information
+
+Once the job is finished, it is time to get your data wrangling pants on! This
+repository contains some scripts that might be helpful in locating and
+formatting the information that you need. Some scripts might be used directly
+while other might need some customising to fit your purpose. Note that these
+scripts might require some extra dependencies. For this reason, these scripts
+are not expected to work unless this package is installed as
+`pip install mzn-bench[scripts]`.
+This allows us to install a minimal version on the running cluster and this
+more complete version locally while processing the data.
+
+### General aggregation
+
+The following scripts can help gather the raw `*_stats.yml`/`*_sol.yml` files
+and combine them for further use:
+
+- `mzn-bench collect-objectives <result_dir> <objectives.csv>` -
+  This script gathers all objective value information given by MiniZinc and the
+  used solvers and combines it into a single CSV file.
+- `mzn-bench collect-statistics <result_dir> <statistics.csv>` -
+  This script gathers all statistical information given by MiniZinc and the used
+  solvers and combines it into a single CSV file.
+
+### Tabulation
+
+The following scripts filter and tabulate specific statistics.
+
+- `mzn-bench report-status <statistics.csv>` - This command will report the
+  number of occurrences of the various solving status of your MiniZinc tasks.
+  Note that the number of satisfied instances is reported as `A + B`, where `A`
+  is the number of optimisation instances that reach a solution not proven
+  optimal and `B` is the number of satisfaction instance finding a solution.
+  Please consult the `-h` flag to display all options.
+- `mzn-bench compare-configurations <statistics.csv> <before_conf> <after_conf>` - This command reports on the differences of the achieved
+  results between two configurations (differences in status, runtime, and
+  objective). You can adjust the changes deemed significant with the
+  `--time-delta` and `--objective-delta` flag. You can use the `--output-mode json` option to ensure the output can be easily parsed by other programs.
+
+### Solution checking
+
+The `mzn-bench check-solutions` command takes the solutions output during run
+and feeds them back into the model to check that the result is satisfiable.
+It also stores the objective and satisfiability information to be used when
+checking statuses. The `-c` option can be used to set how many solutions
+to check (zero to check all solutions).
+
+```bash
+# Check three solutions from each instance
+mzn-bench check-solutions -c 3 ./results
+```
+
+This requires the problem `.mzn` and `.dzn` files from the benchmark run to be
+available in order to run the checker. The `--base-dir <DIR>` option can be used
+to specify a root directory relative to which the file names in the
+`*_sol.yml` files are resolved.
+
+### Status checking
+
+The `mzn-bench check-statuses` command takes the results from `check-solutions`
+command above (which must be run first) and then checks for any solvers which
+have either
+
+- Falsely claimed optimality - where optimality was found by a solver, but a
+  better objective was found elsewhere and verified to be correct.
+- Falsely claimed unsatisfiability - where unsatisfiability was found by a
+  solver, but another solver has given a correct solution for the instance.
+
+### Graph generation
+
+There are a number of plotting helper functions available in
+`mzn_bench.analysis.plot`. In order to use these, you must enable the
+plotting features with `pip install mzn-bench[plotting]`. These use the
+[Bokeh](https://bokeh.org/) visualisation library to provide interactive plots.
+
+The `read_csv` function returns a tuple of [pandas](https://pandas.pydata.org/)
+data frames containing objective and statistics data for plotting or further
+data analysis.
+
+```py
+from mzn_bench.analysis.collect import read_csv
+from mzn_bench.analysis.plot import plot_all_instances
+from bokeh.plotting import show
+
+# Read CSVs generated by mzn-bench collect-result as pandas dataframes
+objs, stats = read_csv("objectives.csv", "statistics.csv")
+
+# Grid plot giving objective values over time, or time to solve
+# (depending on instance type)
+show(plot_all_instances(objs, stats))
+```
+
+
+### Testing
+Currently, this library is tested using a single end-to-end test which runs most of the pipeline locally (without SLURM).
+
+```
+pytest
+```
+
```

### Comparing `mzn-bench-0.1.0/README.md` & `mzn_bench-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -70,16 +70,16 @@
 
 These are all the possible arguments to `schedule`:
 
 - `instances: Path` - The path to the instances file.
 - `timeout: timedelta` - The timeout set for the MiniZinc process.
 - `configurations: Iterable[Configuration]` - MiniZinc solving configurations
   (see below for details).
-- `nodelist: Iterable[str]` - A list of nodes on which SLURM is allowed to
-  schedule the tasks.
+- `nodelist: Optional[Iterable[str]]` - A list of nodes on which SLURM is allowed to
+  schedule the tasks. If `None`, `mzn-bench` will sequentially solve the instances locally.
 - `output_dir: Path = Path.cwd() / "results"` - The directory in which the raw
   results will be placed. This directory will be created if it does not yet
   exist.
 - `job_name: str = "MiniZinc Benchmark"` - The SLURM job name.
 - `cpus_per_task: int = 1` - The number of CPU cores required for each task.
 - `memory: int = 4096` - The maximum memory used for each task.
 - `debug: bool = False` - Directly capture the output of individual jobs
@@ -161,17 +161,24 @@
   This script gathers all statistical information given by MiniZinc and the used
   solvers and combines it into a single CSV file.
 
 ### Tabulation
 
 The following scripts filter and tabulate specific statistics.
 
-- `mzn-bench report-status <statistics.csv>` - This script will report the
+- `mzn-bench report-status <statistics.csv>` - This command will report the
   number of occurrences of the various solving status of your MiniZinc tasks.
+  Note that the number of satisfied instances is reported as `A + B`, where `A`
+  is the number of optimisation instances that reach a solution not proven
+  optimal and `B` is the number of satisfaction instance finding a solution.
   Please consult the `-h` flag to display all options.
+- `mzn-bench compare-configurations <statistics.csv> <before_conf> <after_conf>` - This command reports on the differences of the achieved
+  results between two configurations (differences in status, runtime, and
+  objective). You can adjust the changes deemed significant with the
+  `--time-delta` and `--objective-delta` flag. You can use the `--output-mode json` option to ensure the output can be easily parsed by other programs.
 
 ### Solution checking
 
 The `mzn-bench check-solutions` command takes the solutions output during run
 and feeds them back into the model to check that the result is satisfiable.
 It also stores the objective and satisfiability information to be used when
 checking statuses. The `-c` option can be used to set how many solutions
@@ -217,7 +224,15 @@
 # Read CSVs generated by mzn-bench collect-result as pandas dataframes
 objs, stats = read_csv("objectives.csv", "statistics.csv")
 
 # Grid plot giving objective values over time, or time to solve
 # (depending on instance type)
 show(plot_all_instances(objs, stats))
 ```
+
+
+### Testing
+Currently, this library is tested using a single end-to-end test which runs most of the pipeline locally (without SLURM).
+
+```
+pytest
+```
```

### Comparing `mzn-bench-0.1.0/src/mzn_bench/analysis/collect.py` & `mzn_bench-0.2.0/src/mzn_bench/analysis/collect.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,79 @@
 import os
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Union
+import minizinc
+from mzn_bench import yaml
 
-import ruamel.yaml
+STANDARD_KEYS = [
+    "configuration",
+    "problem",
+    "model",
+    "data_file",
+    "status",
+    "time",
+]
 
 
-def collect_instances(benchmarks_location: str):
+def collect_instances(benchmarks_location: str, shared_data: Optional[str]):
+    shared = Path(shared_data) if shared_data is not None else None
     for root, _, files in os.walk(benchmarks_location):
         for name in files:
             if name.endswith(".mzn"):
                 problem = root.split(os.sep)[-1]
                 datafiles = 0
                 for nroot, _, nfiles in os.walk(root):
                     for nname in nfiles:
-                        if nname.endswith(".dzn") or nname.endswith(".json"):
+                        data = Path(nroot) / nname
+                        if (
+                            data.suffix == ".dzn" or data.suffix == ".json"
+                        ) and data != shared:
                             datafiles += 1
                             yield {
                                 "problem": problem,
                                 "model": Path(root) / name,
-                                "data_file": Path(nroot) / nname,
+                                "data_file": str(data)
+                                + (":" + str(shared) if shared is not None else ""),
                             }
 
                 if datafiles == 0:
                     yield {
                         "problem": problem,
                         "model": Path(root) / name,
-                        "data_file": None,
+                        "data_file": str(shared) if shared is not None else "",
                     }
 
 
 def collect_objectives(dirs: Iterable[Union[str, Path]]) -> List[Dict[str, Any]]:
-    base_keys = ["configuration", "problem", "model", "data_file", "time"]
+    base_keys = STANDARD_KEYS.copy()
+    base_keys.remove("status")  # No need to output SAT every time
     for dir in dirs:
         path = (dir if isinstance(dir, Path) else Path(dir)).resolve()
         for file in path.rglob("*_sol.yml"):
             with file.open() as fp:
-                sols = ruamel.yaml.safe_load(fp)
+                sols = yaml.load(fp)
                 for sol in sols or []:
                     if "solution" not in sol:
                         continue
                     obj = sol["solution"].get("objective", None)
                     item = {k: sol[k] for k in base_keys}
                     item["objective"] = obj
                     item["run"] = path.name
                     yield item
 
 
 def collect_statistics(
     dirs: Iterable[Union[str, Path]], filter_stats: Optional[List[str]] = None
 ) -> List[Dict[str, Any]]:
-    base_keys = ["configuration", "problem", "model", "data_file", "time"]
+    base_keys = STANDARD_KEYS
     for dir in dirs:
         path = (dir if isinstance(dir, Path) else Path(dir)).resolve()
         for file in path.rglob("*_stats.yml"):
             with file.open() as fp:
-                stats = ruamel.yaml.safe_load(fp)
+                stats = yaml.load(fp)
                 if filter_stats is not None:
                     stats = {k: stats[k] for k in base_keys + filter_stats}
                 stats["run"] = path.name
                 yield stats
 
 
 def read_csv(sols: str, stats: str):
```

### Comparing `mzn-bench-0.1.0/src/mzn_bench/analysis/plot.py` & `mzn_bench-0.2.0/src/mzn_bench/analysis/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,39 +3,40 @@
 
 import pandas as pd
 from bokeh.models import CDSView, ColumnDataSource, GroupFilter
 from bokeh.models.annotations import Span
 from bokeh.models.ranges import FactorRange
 from bokeh.models.tools import HoverTool
 from bokeh.palettes import Palette, Spectral5
-from bokeh.plotting import Figure, figure, gridplot
+from bokeh.plotting import figure, gridplot
 from bokeh.transform import factor_cmap
 
 
 def plot_all_instances(
     sols: pd.DataFrame, stats: pd.DataFrame, palette: Palette = Spectral5
-) -> Figure:
+) -> figure:
     """Plot all instances in a grid
 
     Args:
         sols (pd.DataFrame): The solution data frame
         stats (pd.DataFrame): The statistics data frame
         palette (Palette, optional): The colour palette to use. Defaults to Spectral5.
 
     Returns:
-        Figure: The plotting figure
+        figure: The plotting figure
     """
     return gridplot(
         [
             [
                 plot_instance(
                     sols,
                     stats,
                     model,
                     data,
+                    palette,
                 )
                 for model in stats[stats.problem.eq(problem)].model.unique()
                 for data in stats[stats.problem.eq(problem)].data_file.unique()
             ]
             for problem in stats.problem.unique()
         ]
     )
@@ -43,27 +44,27 @@
 
 def plot_instance(
     sols: pd.DataFrame,
     stats: pd.DataFrame,
     model: str,
     data: str = "",
     palette: Palette = Spectral5,
-) -> Figure:
+) -> figure:
     """Plots objective data for an optimisation problem instance, and run time
        data for a satisfaction problem instance.
 
     Args:
         sols (pd.DataFrame): The solution data frame
         stats (pd.DataFrame): The statistics data frame
         model (str): The model file path or problem name of the instance
         data (str, optional): The data file path or name. Defaults to "".
         palette (Palette, optional): The colour palette to use. Defaults to Spectral5.
 
     Returns:
-        Figure: The plotting figure
+        figure.Figure: The plotting figure
     """
     df_stats = stats[
         (stats.model.eq(model) | stats.problem.eq(model)) & stats.data_file.eq(data)
     ]
     df_sols = sols[
         (sols.model.eq(model) | sols.problem.eq(model)) & sols.data_file.eq(data)
     ]
@@ -228,24 +229,24 @@
         p.x_range.end = df_stats.time.max()
         p.xaxis.axis_label = "Time (s)"
         p.yaxis.axis_label = "Objective"
         p.legend.click_policy = "hide"
         return p
 
 
-def plot_total_time(stats: pd.DataFrame, palette: Palette = Spectral5) -> Figure:
+def plot_total_time(stats: pd.DataFrame, palette: Palette = Spectral5) -> figure:
     """Plots a summary bar graph giving total run time for each configuration
         and run.
 
     Args:
         stats (pd.DataFrame): Data frame containing the statistics output
         palette (Palette, optional): Colour palette. Defaults to Spectral5.
 
     Returns:
-        figure.Figure: The plotting figure
+        figure: The plotting figure
     """
 
     if stats.configuration.nunique() == 1:
         # Group by run only
         y = stats.run.unique()
         by = ["run"]
     elif stats.run.nunique() == 1:
```

### Comparing `mzn-bench-0.1.0/src/mzn_bench/cli.py` & `mzn_bench-0.2.0/src/mzn_bench/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 #!/usr/bin/env python3
 
 import csv
 import sys
 from pathlib import Path
-from typing import Iterable
+from typing import Iterable, Optional
 
 import click
 
 from mzn_bench.analysis.collect import collect_instances as collect_insts
 from mzn_bench.analysis.collect import collect_objectives as collect_objs
 from mzn_bench.analysis.collect import collect_statistics as collect_stats
+from mzn_bench.analysis.collect import STANDARD_KEYS
 
-STANDARD_KEYS = [
-    "problem",
-    "model",
-    "data_file",
-    "configuration",
-    "status",
-    "time",
-    "run",
-]
 IMPORT_ERROR = """This feature is not supported in minimal minizinc-slurm environments.
 
 Please install using `pip install mzn-bench[scripts]`
 """
 
 # Import the tabulate formats if the package is available
 tabulate_options = []
@@ -38,16 +30,22 @@
 @click.group()
 def main():
     """Command-line tool for minizinc-slurm."""
     pass
 
 
 @main.command()
+@click.option(
+    "--shared-data",
+    default=None,
+    help="Additional data to be shared by all instances",
+    type=click.Path(exists=True, dir_okay=False),
+)
 @click.argument("benchmarks_location", type=click.Path(exists=True, file_okay=True))
-def collect_instances(benchmarks_location: str):
+def collect_instances(shared_data: Optional[str], benchmarks_location: str):
     """This script collect MiniZinc instances and outputs them in a csv format
 
     The MiniZinc instances are expected to be organised according to the MiniZinc
     benchmarks structure:
         - Each problem is contained in its own folder
         - Problems contain one or more MiniZinc Model (.mzn) file
         - Each model is combined with all the data (.dzn / .json) in the same problem folder (and its subfolders)
@@ -61,15 +59,15 @@
     instances = 0
     writer = csv.DictWriter(
         sys.stdout,
         ["problem", "model", "data_file"],
         dialect="unix",
     )
     writer.writeheader()
-    for instance in collect_insts(benchmarks_location):
+    for instance in collect_insts(benchmarks_location, shared_data):
         writer.writerow(instance)
         instances += 1
     click.echo(f"Nr. Instances = {instances}", err=True)
 
 
 @main.command()
 @click.argument("dirs", nargs=-1, type=click.Path(exists=True, dir_okay=True))
@@ -78,49 +76,68 @@
     """Collects objective values and combines them into a single CSV file.
 
     \b
     DIRS are directories containing the result YAML files
     OUT_FILE is the output CSV file containing objective data
     """
 
+    collect_objectives_(dirs, out_file)
+
+
+def collect_objectives_(dirs: Iterable[str], out_file: str):
     count = 0
     with Path(out_file).open(mode="w") as file:
         writer = csv.DictWriter(
-            file, STANDARD_KEYS + ["objective"], dialect="unix", extrasaction="ignore"
+            file,
+            STANDARD_KEYS + ["run", "objective"],
+            dialect="unix",
+            extrasaction="ignore",
         )
         writer.writeheader()
+        last_keys = ("", "", "", "")
         for objective in collect_objs(dirs):
+            keys = (
+                objective["configuration"],
+                objective["problem"],
+                objective["model"],
+                objective["data_file"],
+            )
             writer.writerow(objective)
-            count += 1
+            if last_keys != keys:
+                count += 1
+                last_keys = keys
 
-    click.echo(f"Processed {count} files.", err=True)
+    click.echo(f"Processed objectives from {count} files.", err=True)
 
 
 @main.command()
 @click.argument("dirs", nargs=-1, type=click.Path(exists=True, dir_okay=True))
 @click.argument("out_file", nargs=1, type=click.Path(file_okay=True))
 def collect_statistics(dirs: Iterable[str], out_file: str):
     """Collects statistics values and combines them into a single CSV file.
 
     \b
     DIRS are directories containing the result YAML files
     OUT_FILE is the CSV file containing aggregated statistics data
     """
+    collect_statistics_(dirs, out_file)
 
+
+def collect_statistics_(dirs: Iterable[str], out_file: str):
     statistics = list(collect_stats(dirs))
     keys = {key for obj in statistics for key in obj.keys()}
     keys = keys.difference(STANDARD_KEYS)
     with Path(out_file).open(mode="w") as file:
         writer = csv.DictWriter(
             file, STANDARD_KEYS + list(keys), dialect="unix", extrasaction="ignore"
         )
         writer.writeheader()
         for stat in statistics:
             writer.writerow(stat)
-    click.echo(f"Processed {len(statistics)} files.", err=True)
+    click.echo(f"Processed statistics from {len(statistics)} files.", err=True)
 
 
 @main.command()
 @click.option(
     "-c",
     "--check",
     default=1,
@@ -144,14 +161,18 @@
     This is done by feeding the solution produced back into the model and checking
     that is is still satisfiable.
 
     \b
     DIR is the directory containing YAML output from minizinc-slurm
     PYTEST_ARGS are passed to the underlying PyTest command
     """
+    check_solutions_(check, base_dir, dir, pytest_args)
+
+
+def check_solutions_(check: int, base_dir: str, dir: str, pytest_args: Iterable[str]):
     try:
         import pytest
 
         args = [
             "-p",
             "mzn_bench.pytest.check_solutions",
             "--check",
@@ -175,15 +196,18 @@
 
     This can only be run after the check-solutions command has been run.
 
     \b
     DIR is the directory containing YAML output from minizinc-slurm
     PYTEST_ARGS are passed to the underlying PyTest command
     """
+    check_statuses_(dir, pytest_args)
 
+
+def check_statuses_(dir: str, pytest_args: Iterable[str]):
     try:
         import pytest
 
         args = ["-p", "mzn_bench.pytest.check_statuses", dir]
         args.extend(pytest_args)
         exit(pytest.main(args))
     except ImportError:
@@ -199,46 +223,96 @@
 )
 @click.option(
     "--per-problem",
     is_flag=True,
     help="Create a row for every problem",
 )
 @click.option(
-    "--avg-time",
-    is_flag=True,
-    help="Show average runtime in the table",
+    "--avg",
+    type=click.Choice(["time", "solveTime", "flatTime"]),
+    help="Show average of the given stat in the table",
 )
 @click.option(
     "--output-mode",
     type=click.Choice(tabulate_options, case_sensitive=False),
     default="pretty",
     help="The table format used in the output. All valid tablefmt values are allow, try `latex` for example.",
 )
 @click.argument(
     "statistics", metavar="stats_file", type=click.Path(exists=True, file_okay=True)
 )
 def report_status(
     per_model: bool,
     per_problem: bool,
     statistics: str,
-    avg_time: bool,
+    avg: str,
     output_mode: str,
 ):
     """Aggregate status of MiniZinc instance runs into a table
 
     STATS_FILE is the CSV file containing aggregated statistics data
     """
     try:
         from .analysis.report_status import report_status as report_status_fn
 
         print(
-            report_status_fn(
-                per_model, per_problem, Path(statistics), avg_time, output_mode
-            )
+            report_status_fn(per_model, per_problem, Path(statistics), avg, output_mode)
         )
     except ImportError:
         click.echo(IMPORT_ERROR, err=True)
         exit(1)
 
 
+@main.command()
+@click.argument(
+    "statistics", metavar="stats_file", type=click.Path(exists=True, file_okay=True)
+)
+@click.argument(
+    "from_conf",
+    metavar="from_conf",
+)
+@click.argument(
+    "to_conf",
+    metavar="to_conf",
+)
+@click.option(
+    "--time-delta",
+    default=0.1,
+    type=float,
+    help="Fraction of time change considered to be significant",
+)
+@click.option(
+    "--obj-delta",
+    default=0.1,
+    type=float,
+    help="Fraction of objective value change considered to be significant",
+)
+@click.option(
+    "--output-mode",
+    type=click.Choice(["human", "json"], case_sensitive=False),
+    default="human",
+    help="The format used in the output.",
+)
+def compare_configurations(
+    statistics: str,
+    from_conf: str,
+    to_conf: str,
+    time_delta: float,
+    obj_delta: float,
+    output_mode: str,
+):
+    """Show all significant performance changes between two configurations"""
+    try:
+        from .analysis.analyse_changes import compare_configurations as fn
+
+        result = fn(Path(statistics), from_conf, to_conf, time_delta, obj_delta)
+        if output_mode != "human":
+            result = result.serialise(output_mode)
+
+        print(result)
+    except ImportError:
+        click.echo(IMPORT_ERROR, err=True)
+        exit(1)
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `mzn-bench-0.1.0/src/mzn_bench/mzn_slurm.py` & `mzn_bench-0.2.0/src/mzn_bench/mzn_slurm.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,23 +6,27 @@
 import sys
 import time
 import traceback
 from dataclasses import asdict, dataclass, field, fields
 from datetime import timedelta
 from pathlib import Path
 from typing import Any, Dict, Iterable, NoReturn, Optional
+import minizinc
+from ruamel.yaml import YAML
+
+yaml = YAML(typ="safe")
+yaml.register_class(minizinc.types.ConstrEnum)
+yaml.register_class(minizinc.types.AnonEnum)
+yaml.default_flow_style = False
 
 if os.environ.get("MZN_DEBUG", "OFF") == "ON":
     import logging
 
     logging.basicConfig(stream=sys.stderr, level=logging.DEBUG)
 
-import minizinc
-import ruamel.yaml
-
 
 @dataclass
 class Configuration:
     name: str
     solver: minizinc.Solver
     minizinc: Optional[Path] = None
     processes: Optional[int] = None
@@ -30,27 +34,50 @@
     free_search: bool = False
     optimisation_level: Optional[int] = None
     other_flags: Dict[str, Any] = field(default_factory=dict)
     extra_data: Dict[str, Any] = field(default_factory=dict)
 
     def to_dict(self):
         obj = asdict(self)
-        obj["solver"] = self.solver.output_configuration()
-        obj["sol_ident"] = self.solver._identifier
+        if self.solver._identifier is not None:
+            obj["solver"] = ""
+            obj["sol_ident"] = self.solver._identifier
+        else:
+            obj["solver"] = self.solver.output_configuration()
+            obj["sol_ident"] = ""
         if self.minizinc is not None:
             obj["minizinc"] = str(self.minizinc)
         return obj
 
     @classmethod
     def from_dict(cls, obj):
         field_names = set(f.name for f in fields(minizinc.Solver))
-        obj["solver"] = minizinc.Solver(
-            **{k: v for k, v in json.loads(obj["solver"]).items() if k in field_names}
-        )
-        obj["solver"]._identifier = obj.pop("sol_ident")
+        identifier = obj.pop("sol_ident")
+        if identifier == "":
+            obj["solver"] = minizinc.Solver(
+                **{
+                    k: v
+                    for k, v in json.loads(obj["solver"]).items()
+                    if k in field_names
+                }
+            )
+        elif identifier.endswith(".msc"):
+            obj["solver"] = minizinc.Solver.load(identifier)
+        else:
+            # TODO: version tags should be handled correctly by MiniZinc Python
+            version = None
+            if "@" in identifier:
+                split = identifier.split("@")
+                assert len(split) == 2
+                identifier = split[0]
+                version = split[1]
+            obj["solver"] = minizinc.Solver.lookup(identifier)
+            if version is not None:
+                assert obj["solver"].version == version
+
         if obj["minizinc"] is not None:
             obj["minizinc"] = Path(obj["minizinc"])
         return cls(**obj)
 
 
 @dataclass
 class DZNExpression:
@@ -75,24 +102,23 @@
 
 
 # Schedule SLURM tasks
 def schedule(
     instances: Path,
     timeout: timedelta,
     configurations: Iterable[Configuration],
-    nodelist: Iterable[str],
+    nodelist: Optional[Iterable[str]] = None,
     output_dir: Path = Path.cwd() / "results",
     job_name: str = "MiniZinc Benchmark",
     cpus_per_task: int = 1,
     memory: int = 4096,
     debug: bool = False,
     nice: Optional[int] = None,
     wait: bool = False,
 ) -> NoReturn:
-
     # Count number of instances
     assert instances.exists()
     num_instances = sum(1 for line in instances.open()) - 1
 
     # Create output_dir if it does not exist
     output_dir.mkdir(parents=True, exist_ok=True)
 
@@ -107,33 +133,43 @@
     env["MZN_SLURM_TIMEOUT"] = str(int(timeout / timedelta(milliseconds=1)))
 
     slurm_output = "/dev/null"
     if debug:
         slurm_output = f"{output_dir.resolve()}/minizinc_slurm-%A_%a.out"
         env["MZN_DEBUG"] = "ON"
 
+    n_tasks = num_instances * len(configurations)
+    instances = str(instances.resolve())
+    output_dir = str(output_dir.resolve())
+
+    if nodelist is None:
+        os.environ.update(env)
+        for i in range(n_tasks):  # simulate environment like SLURM
+            os.environ["SLURM_ARRAY_TASK_ID"] = str(i + 1)
+            main(Path(instances), Path(output_dir))
+        return
     cmd = [
         "sbatch",
         f"--output={slurm_output}",
         f'--job-name="{job_name}"',
         f"--cpus-per-task={cpus_per_task}",
         f"--mem={memory}",
         f"--nodelist={','.join(nodelist)}",
-        f"--array=1-{num_instances*len(configurations)}",
+        f"--array=1-{n_tasks}",
         f"--time={timeout + timedelta(minutes=1)}",  # Set hard timeout as failsafe
     ]
     if nice is not None:
         cmd.append(f"--nice={nice}")
     if wait:
         cmd.append(f"--wait")
     cmd.extend(
         [
             str(this_script.resolve()),
-            str(instances.resolve()),
-            str(output_dir.resolve()),
+            str(instances),
+            str(output_dir),
         ]
     )
 
     # Replace current process with the correct sbatch call
     os.execvpe(
         "sbatch",
         cmd,
@@ -144,18 +180,21 @@
 async def run_instance(
     problem, model, data, config, timeout, stat_base, sol_file, stats_file
 ):
     statistics = stat_base.copy()
     try:
         driver = minizinc.default_driver
         if config.minizinc is not None:
-            driver = minizinc.CLI.CLIDriver(config.minizinc)
-        instance = minizinc.Instance(config.solver, minizinc.Model(model), driver)
-        if data is not None:
-            instance.add_file(data, parse_data=False)
+            assert config.minizinc.exists()
+            driver = minizinc.Driver(config.minizinc)
+        model = minizinc.Model(model)
+        model.output_type = dict
+        instance = minizinc.Instance(config.solver, model, driver)
+        for path in data:
+            instance.add_file(path, parse_data=False)
         is_satisfaction = instance.method == minizinc.Method.SATISFY
 
         for key, value in config.extra_data.items():
             instance[key] = value
 
         start = time.perf_counter()
         with sol_file.open(mode="w") as file:
@@ -167,80 +206,93 @@
                 free_search=config.free_search,
                 optimisation_level=config.optimisation_level,
                 **config.other_flags,
             ):
                 solution = stat_base.copy()
                 solution["status"] = str(result.status)
                 if "time" in result.statistics:
-                    solution["time"] = result.statistics.pop("time").total_seconds()
+                    statistics_time = result.statistics.pop("time")
+                    if type(statistics_time) is timedelta:
+                        solution[
+                            "time"
+                        ] = (
+                            statistics_time.total_seconds()
+                        )  # convert timedelta to seconds (float), since we cannot register and serialize it to YAML
+                    else:
+                        raise TypeError(
+                            f"Time statistic was not `datetime.timedelta` type, but was {type(statistics_time)}. Perhaps you are using an older version of minizinc-python"
+                        )
                 if result.solution is not None:
-                    solution["solution"] = asdict(result.solution)
+                    solution["solution"] = result.solution
                     solution["solution"].pop("_output_item", None)
                     solution["solution"].pop("_checker", None)
-                file.write(ruamel.yaml.dump([solution]))
+                yaml.dump([solution], file)
 
                 statistics.update(result.statistics)
                 statistics["status"] = str(result.status)
                 if result.solution is not None and not is_satisfaction:
-                    statistics["objective"] = result.solution.objective
-
-        total_time = time.perf_counter() - start
-        statistics["time"] = total_time
+                    statistics["objective"] = result.solution["objective"]
     except minizinc.MiniZincError as err:
         statistics["status"] = str(minizinc.result.Status.ERROR)
         statistics["error"] = str(err)
 
+    total_time = time.perf_counter() - start
+    statistics["time"] = time.perf_counter() - start
+
     for key, val in statistics.items():
         if isinstance(val, timedelta):
             statistics[key] = val.total_seconds()
-    ruamel.yaml.dump(
-        statistics,
-        stats_file.open(mode="w"),
-        default_flow_style=False,
-    )
 
+    with open(stats_file, "w") as file:
+        yaml.dump(statistics, file)
 
-if __name__ == "__main__":
+
+def main(instances, output_dir):
     filename = "minizinc_slurm"
-    output_dir = Path.home()
     try:
-        instances = Path(sys.argv[1])
-        output_dir = Path(sys.argv[2])
         task_id = int(os.environ["SLURM_ARRAY_TASK_ID"]) - 1
         timeout = timedelta(milliseconds=int(os.environ["MZN_SLURM_TIMEOUT"]))
-        configurations = [
-            Configuration.from_dict(conf)
-            for conf in json.loads(os.environ["MZN_SLURM_CONFIGS"], cls=_JSONDec)
-        ]
+        configurations = json.loads(os.environ["MZN_SLURM_CONFIGS"], cls=_JSONDec)
 
         # Select instance and configuration based on SLURM_ARRAY_TASK_ID
         with open(instances) as instances_file:
             reader = csv.reader(instances_file, dialect="unix")
             next(reader)  # Skip the header line
             row = 1
             while task_id >= len(configurations):
                 next(reader)  # Skip non-selected instances
                 task_id = task_id - len(configurations)
                 row = row + 1
             selected_instance = next(reader)
-            config = configurations[task_id]
-            filename = f"{row}_{config.name}"
+
+        # Deserialise Configuration
+        config = configurations[task_id]
+        # TODO: workaround because we might not know the solver in the system MiniZinc
+        if config["minizinc"] is not None:
+            mzn_path = Path(config["minizinc"])
+            assert mzn_path.exists()
+            minizinc.Driver(mzn_path).make_default()
+        config = Configuration.from_dict(config)
+
+        filename = f"{row}_{config.name}"
 
         # Process instance
         problem = selected_instance[0]
 
         model = Path(selected_instance[1])
         if not model.is_absolute():
             model = instances.parent / model
 
-        data = None
-        if selected_instance[2] != "":
-            data = Path(selected_instance[2])
-            if not data.is_absolute():
-                data = instances.parent / data
+        data = []
+        for file in selected_instance[2].split(":"):
+            if file != "":
+                path = Path(selected_instance[2])
+                if not path.is_absolute():
+                    path = instances.parent / file
+                data.append(path)
 
         stat_base = {
             "problem": selected_instance[0],
             "model": selected_instance[1],
             "data_file": selected_instance[2],
             "configuration": config.name,
             "status": str(minizinc.result.Status.UNKNOWN),
@@ -256,9 +308,17 @@
                 timeout,
                 stat_base,
                 output_dir / f"{filename}_sol.yml",
                 output_dir / f"{filename}_stats.yml",
             )
         )
     except Exception:
+        if "SLURM_JOB_NODELIST" not in os.environ:
+            raise
         file = output_dir / f"{filename}_err.txt"
         file.write_text(f"ERROR: {traceback.format_exc()}")
+
+
+if __name__ == "__main__":
+    instances = Path(sys.argv[1])
+    output_dir = Path(sys.argv[2]) if len(sys.argv) == 3 else Path.home()
+    main(instances, output_dir)
```

### Comparing `mzn-bench-0.1.0/src/mzn_bench/pytest/check_solutions.py` & `mzn_bench-0.2.0/src/mzn_bench/pytest/check_solutions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 import pytest
 from _pytest.config import Config
 from minizinc import Model, Solver, Status
 from minizinc.helpers import check_solution
-from ruamel.yaml import YAML
-
-yaml = YAML(typ="unsafe")
+import minizinc
+from mzn_bench import yaml
 
 
 class SolFile(pytest.File):
     checker: Solver
     num_check: int
     base_dir: Path
 
@@ -135,15 +134,15 @@
             help="Base directory for model/data file resolution.",
         )
 
     def pytest_collect_file(self, parent, path):
         if path.basename.endswith("_sol.yml"):
             return SolFile.from_parent(
                 parent,
-                fspath=path,
+                path=Path(path),
                 checker=self.checker,
                 num_check=self.num_check,
                 base_dir=Path(self.base_dir),
             )
 
     def pytest_runtest_logreport(self, report):
         # Record satisfiability and objective bounds for check_statuses
```

### Comparing `mzn-bench-0.1.0/src/mzn_bench/pytest/check_statuses.py` & `mzn_bench-0.2.0/src/mzn_bench/pytest/check_statuses.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Any, Dict
 
 import pytest
 from minizinc import Method, Status
-from ruamel.yaml import YAML
-
-yaml = YAML(typ="unsafe")
+from pathlib import Path
+from mzn_bench import yaml
 
 
 class StatsFile(pytest.File):
     def collect(self):
         with self.fspath.open() as fp:
             stats = yaml.load(fp)
             name = ":".join(
@@ -26,19 +25,22 @@
     stats: Dict[str, Any]
 
     def __init__(self, stats: Dict[str, any], *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.stats = stats
 
     def runtest(self):
-        method = Method[self.stats["method"].upper()]
         status = Status[self.stats["status"]]
         key = "{}_{}_{}".format(
             self.stats["problem"], self.stats["model"], self.stats["data_file"]
         )
+        if status is Status.ERROR:
+            pytest.skip("skipping {} as status was ERROR".format(key))
+
+        method = Method[self.stats["method"].upper()]
         if status is Status.UNSATISFIABLE:
             is_satisfiable = self.config.cache.get("sat/" + key, False)
             assert not is_satisfiable, "Incorrect UNSAT status"
         if status is Status.OPTIMAL_SOLUTION:
             min_obj, max_obj = self.config.cache.get("obj/" + key, (None, None))
             assert (
                 method is Method.MAXIMIZE
@@ -50,8 +52,8 @@
 
     def reportinfo(self):
         return self.fspath, 0, "usecase: {}".format(self.name)
 
 
 def pytest_collect_file(parent, path):
     if path.basename.endswith("_stats.yml"):
-        return StatsFile.from_parent(parent, fspath=path)
+        return StatsFile.from_parent(parent, path=Path(path))
```

