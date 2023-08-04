# Comparing `tmp/gable-0.1.0.tar.gz` & `tmp/gable-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gable-0.1.0.tar", max compression
+gzip compressed data, was "gable-0.2.1.tar", max compression
```

## Comparing `gable-0.1.0.tar` & `gable-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     2581 2023-07-14 21:13:07.778057 gable-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-13 23:27:44.590688 gable-0.1.0/gable/__init__.py
--rw-r--r--   0        0        0     1064 2023-07-14 02:46:30.175869 gable-0.1.0/gable/cli.py
--rw-r--r--   0        0        0     1946 2023-07-12 15:45:20.731121 gable-0.1.0/gable/client.py
--rw-r--r--   0        0        0        0 2023-07-11 21:23:36.262951 gable-0.1.0/gable/commands/__init__.py
--rw-r--r--   0        0        0      448 2023-07-14 02:46:30.175999 gable-0.1.0/gable/commands/auth.py
--rw-r--r--   0        0        0     4549 2023-07-14 21:03:16.563277 gable-0.1.0/gable/commands/contract.py
--rw-r--r--   0        0        0    21700 2023-07-14 21:03:16.563495 gable-0.1.0/gable/commands/data_asset.py
--rw-r--r--   0        0        0      629 2023-07-14 02:46:30.176575 gable-0.1.0/gable/commands/ping.py
--rw-r--r--   0        0        0        0 2023-07-11 21:23:36.263584 gable-0.1.0/gable/helpers/__init__.py
--rw-r--r--   0        0        0     3071 2023-07-14 21:03:16.563951 gable-0.1.0/gable/helpers/check.py
--rw-r--r--   0        0        0     1824 2023-07-14 02:46:30.176848 gable-0.1.0/gable/helpers/contract.py
--rw-r--r--   0        0        0     4260 2023-07-14 21:03:16.564126 gable-0.1.0/gable/helpers/data_asset.py
--rw-r--r--   0        0        0      143 2023-07-12 20:37:22.605800 gable-0.1.0/gable/helpers/emoji.py
--rw-r--r--   0        0        0     1774 2023-07-14 21:03:16.564231 gable-0.1.0/gable/helpers/multi_option.py
--rw-r--r--   0        0        0     1039 2023-07-14 21:03:16.564779 gable-0.1.0/gable/helpers/repo_interactions.py
--rw-r--r--   0        0        0    13598 2023-07-14 02:46:30.177304 gable-0.1.0/gable/openapi.py
--rw-r--r--   0        0        0        0 2023-07-09 17:14:49.025833 gable-0.1.0/gable/readers/__init__.py
--rw-r--r--   0        0        0     4027 2023-07-12 19:04:49.765702 gable-0.1.0/gable/readers/dbapi.py
--rw-r--r--   0        0        0      255 2023-07-14 02:57:36.313991 gable-0.1.0/gable/readers/file.py
--rw-r--r--   0        0        0      638 2023-07-12 19:04:49.766457 gable-0.1.0/gable/readers/mysql.py
--rw-r--r--   0        0        0      668 2023-07-12 19:04:49.766743 gable-0.1.0/gable/readers/postgres.py
--rw-r--r--   0        0        0     1249 2023-07-14 21:13:07.778312 gable-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3487 1970-01-01 00:00:00.000000 gable-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2627 2023-08-01 01:15:13.567843 gable-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 23:48:09.766234 gable-0.2.1/gable/__init__.py
+-rw-r--r--   0        0        0     1165 2023-08-04 15:16:53.040265 gable-0.2.1/gable/cli.py
+-rw-r--r--   0        0        0     2006 2023-08-01 02:47:51.133840 gable-0.2.1/gable/client.py
+-rw-r--r--   0        0        0        0 2023-08-01 01:15:13.568349 gable-0.2.1/gable/commands/__init__.py
+-rw-r--r--   0        0        0      448 2023-08-01 01:15:13.568606 gable-0.2.1/gable/commands/auth.py
+-rw-r--r--   0        0        0     4686 2023-08-04 15:16:53.040416 gable-0.2.1/gable/commands/contract.py
+-rw-r--r--   0        0        0    22739 2023-08-01 01:15:13.568827 gable-0.2.1/gable/commands/data_asset.py
+-rw-r--r--   0        0        0      490 2023-08-01 01:15:13.568913 gable-0.2.1/gable/commands/env.py
+-rw-r--r--   0        0        0      629 2023-08-01 01:15:13.569322 gable-0.2.1/gable/commands/ping.py
+-rw-r--r--   0        0        0        0 2023-08-01 01:15:13.569385 gable-0.2.1/gable/helpers/__init__.py
+-rw-r--r--   0        0        0     3071 2023-08-01 01:15:13.569495 gable-0.2.1/gable/helpers/check.py
+-rw-r--r--   0        0        0     2440 2023-08-04 15:16:53.040830 gable-0.2.1/gable/helpers/contract.py
+-rw-r--r--   0        0        0     4237 2023-08-04 15:16:53.041176 gable-0.2.1/gable/helpers/data_asset.py
+-rw-r--r--   0        0        0      143 2023-08-01 01:15:13.570336 gable-0.2.1/gable/helpers/emoji.py
+-rw-r--r--   0        0        0     1774 2023-08-01 01:15:13.570424 gable-0.2.1/gable/helpers/multi_option.py
+-rw-r--r--   0        0        0     1071 2023-08-04 15:16:53.041597 gable-0.2.1/gable/helpers/repo_interactions.py
+-rw-r--r--   0        0        0      176 2023-08-01 02:47:51.134034 gable-0.2.1/gable/helpers/shell_output.py
+-rw-r--r--   0        0        0    14643 2023-08-04 15:19:12.166896 gable-0.2.1/gable/openapi.py
+-rw-r--r--   0        0        0        0 2023-08-01 01:15:13.571111 gable-0.2.1/gable/readers/__init__.py
+-rw-r--r--   0        0        0     4027 2023-08-01 01:15:13.571395 gable-0.2.1/gable/readers/dbapi.py
+-rw-r--r--   0        0        0      255 2023-08-01 01:15:13.571469 gable-0.2.1/gable/readers/file.py
+-rw-r--r--   0        0        0      638 2023-08-01 01:15:13.571547 gable-0.2.1/gable/readers/mysql.py
+-rw-r--r--   0        0        0      668 2023-08-01 01:15:13.571620 gable-0.2.1/gable/readers/postgres.py
+-rw-r--r--   0        0        0     1317 2023-08-04 15:19:12.167045 gable-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3535 1970-01-01 00:00:00.000000 gable-0.2.1/PKG-INFO
```

### Comparing `gable-0.1.0/README.md` & `gable-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 gable --help
 Usage: gable [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --endpoint TEXT  Customer API endpoint for Gable, in the format
                    https://api.company.gable.ai/
   --api-key TEXT   API Key for Gable
+  --version        Show the version and exit.
   --help           Show this message and exit.
 
 Commands:
   auth        View configured Gable authentication information
   contract    Validate/publish contracts and check data asset compliance
   data-asset  Commands for data assets
   ping        Pings the Gable API to check for connectivity
```

### Comparing `gable-0.1.0/gable/cli.py` & `gable-0.2.1/gable/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 import os
 from typing import Optional
 import click
 from gable.client import GableClient
-from gable.helpers.repo_interactions import GitInfo, get_git_info
+from gable.helpers.repo_interactions import GitInfo, get_git_repo_info
 
 from .commands.auth import auth
+from .commands.env import env
 from .commands.contract import contract
 from .commands.data_asset import data_asset
 from .commands.ping import ping
 
 
 class Context:
     def __init__(self):
         self.client: Optional[GableClient] = None
         self.git_info: Optional[GitInfo] = None
 
 
 @click.group()
 @click.option(
     "--endpoint",
-    default=os.environ.get("GABLE_API_ENDPOINT"),
+    default=lambda: os.environ.get("GABLE_API_ENDPOINT"),
     help="Customer API endpoint for Gable, in the format https://api.company.gable.ai/",
 )
 @click.option(
     "--api-key",
-    default=os.environ.get("GABLE_API_KEY"),
+    default=lambda: os.environ.get("GABLE_API_KEY"),
     help="API Key for Gable",
 )
+@click.version_option()
 @click.pass_context
 def cli(ctx, endpoint, api_key):
     ctx.obj = Context()
     ctx.obj.client = GableClient(endpoint, api_key)
-    ctx.obj.git_info = get_git_info()
+    ctx.obj.git_info = get_git_repo_info()
 
 
 cli.add_command(auth)
+cli.add_command(env)
 cli.add_command(contract)
 cli.add_command(data_asset)
 cli.add_command(ping)
 
 
 if __name__ == "__main__":
     cli()  # type: ignore
```

### Comparing `gable-0.1.0/gable/client.py` & `gable-0.2.1/gable/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     def __init__(self, endpoint: str, api_key: str) -> None:
         self.endpoint = endpoint
         self.api_key = api_key
 
         self.validate_api_key()
         self.validate_endpoint()
 
+        self.ui_endpoint = endpoint.replace("api-", "", 1)
+
     def validate_api_key(self):
         if not self.api_key:
             raise click.ClickException(
                 "API Key is not set. Use the --api-key argument or set GABLE_API_KEY "
                 "environment variable."
             )
```

### Comparing `gable-0.1.0/gable/commands/contract.py` & `gable-0.2.1/gable/commands/contract.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,71 @@
 from typing import List
 import click
 from click.core import Context as ClickContext
 from gable.helpers.data_asset import get_schema_contents
 from gable.helpers.emoji import EMOJI
 from gable.helpers.contract import contract_files_to_post_contract_request
 from gable.helpers.check import post_contract_check_request
+from gable.helpers.shell_output import shell_linkify
 
 
 @click.group()
 def contract():
     """Validate/publish contracts and check data asset compliance"""
     pass
 
 
 @contract.command(
-    name="publish",
     epilog="""Examples:
 
     gable contract publish contract1.yaml
 
     gable contract publish **/*.yaml""",
 )
 @click.argument(
     "contract_files",
     type=click.File(),
     nargs=-1,
 )
 @click.pass_context
-def publish_contract(ctx: ClickContext, contract_files: List[click.File]):
+def publish(ctx: ClickContext, contract_files: List[click.File]):
     """Publishes data contracts to Gable"""
     request = contract_files_to_post_contract_request(contract_files)
     response, success, status_code = ctx.obj.client.post(
         "v0/contract", data=request.json()
     )
     if not success:
         raise click.ClickException(f"Publish failed: {response['message']}")
-    updated_contracts = ", ".join(response["contractIds"])
+    updated_contracts = ", ".join(
+        shell_linkify(
+            f"{ctx.obj.client.ui_endpoint}/contracts/{cid}/schema",
+            cid,
+        )
+        for cid in response["contractIds"]
+    )
     if len(response["contractIds"]) == 0:
         click.echo("\u2705 No contracts published")
     else:
         click.echo(f"\u2705 {len(response['contractIds'])} contract(s) published")
         click.echo(f"\t{updated_contracts}")
 
 
 @contract.command(
-    name="validate",
     epilog="""Examples:
 
     gable contract validate contract1.yaml
 
     gable contract validate **/*.yaml""",
 )
 @click.argument("contract_files", type=click.File(), nargs=-1)
 @click.pass_context
-def validate_contracts(ctx: ClickContext, contract_files: List[click.File]):
+def validate(ctx: ClickContext, contract_files: List[click.File]):
     """Validates the configuration of the data contract files"""
     request = contract_files_to_post_contract_request(contract_files)
-    response, success, status_code = ctx.obj.client.post(
+    response, success, _status_code = ctx.obj.client.post(
         "v0/contract/validate", data=request.json()
     )
     # For each input file, zip up the emoji, file name, and result message into a tuple
     zipped_results = zip(
         [
             # Compute emoji based on whether the contract is valid
             EMOJI.GREEN_CHECK.value if m.strip() == "VALID" else EMOJI.RED_X.value
```

### Comparing `gable-0.1.0/gable/commands/data_asset.py` & `gable-0.2.1/gable/commands/data_asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,33 +35,56 @@
 @click.option(
     "-o",
     "--output",
     type=click.Choice(["table", "json"]),
     default="table",
     help="Format of the output. Options are: table (default) or json",
 )
-def list_data_assets(ctx: ClickContext, output: str) -> None:
+@click.option(
+    "--full",
+    is_flag=True,
+    help="Return full data asset details including namespace and name",
+)
+def list_data_assets(ctx: ClickContext, output: str, full: bool) -> None:
     """List all data assets"""
     # Get the data
     response, success, status_code = ctx.obj.client.get("v0/data-assets")
 
     # Format the output
     if output == "json":
         data_asset_list = []
         for data_asset in response:
-            data_asset_list.append(
-                {"namespace": data_asset["namespace"], "name": data_asset["name"]}
-            )
+            row = {"resourceName": f"{data_asset['namespace']}:{data_asset['name']}"}
+            if full:
+                # Filter out invalid data assets...
+                if "://" in data_asset["namespace"]:
+                    row["type"] = data_asset["namespace"].split("://", 1)[0]
+                    row["dataSource"] = data_asset["namespace"].split("://", 1)[1]
+                    row["name"] = data_asset["name"]
+            data_asset_list.append(row)
         click.echo(json.dumps(data_asset_list))
     else:
         table = Table(show_header=True, title="Data Assets")
-        table.add_column("namespace")
-        table.add_column("name")
+        table.add_column("resourceName")
+        if full:
+            table.add_column("type")
+            table.add_column("dataSource")
+            table.add_column("name")
         for data_asset in response:
-            table.add_row(data_asset["namespace"], data_asset["name"])
+            if not full:
+                table.add_row(f"{data_asset['namespace']}:{data_asset['name']}")
+            else:
+                # Filter out invalid data assets...
+                if "://" in data_asset["namespace"]:
+                    table.add_row(
+                        f"{data_asset['namespace']}:{data_asset['name']}",
+                        data_asset["namespace"].split("://", 1)[0],
+                        data_asset["namespace"].split("://", 1)[1],
+                        data_asset["name"],
+                    )
         console.print(table)
 
 
 @data_asset.command(
     name="register",
     epilog="""Example:
 
@@ -97,31 +120,31 @@
 )
 @optgroup.option(
     "--host",
     "-h",
     type=str,
     help="""The host name of the production database, for example 'service-one.xxxxxxxxxxxx.us-east-1.rds.amazonaws.com'.
     Despite not needing to connect to the production database, the host is still needed to generate the unique resource 
-    name for the data asset. For example, a Postgres resource name is 'postgres://<host>:<port>/<db>/<schema>/<table>'
+    name for the data asset. For example, a Postgres resource name is 'postgres://<host>:<port>:<db>.<schema>.<table>'
     """,
 )
 @optgroup.option(
     "--port",
     "-p",
     type=int,
     help="""The port of the production database. Despite not needing to connect to the production database, the port 
     is still needed to generate the unique resource name for the data asset. For example, a Postgres resource name is 
-    'postgres://<host>:<port>/<db>/<schema>/<table>'""",
+    'postgres://<host>:<port>:<db>.<schema>.<table>'""",
 )
 @optgroup.option(
     "--db",
     type=str,
     help="""The name of the production database. Despite not needing to connect to 
     the production database, the database name is still needed to generate the unique resource name for the data 
-    asset. For example, a Postgres resource name is 'postgres://<host>:<port>/<db>/<schema>/<table>'
+    asset. For example, a Postgres resource name is 'postgres://<host>:<port>:<db>.<schema>.<table>'
     
     Database naming convention frequently includes the environment (production/development/test/staging) in the 
     database name, so this value may not match the name of the database in the proxy database instance. If this is 
     the case, you can set the --proxy-db value to the name of the database in the proxy instance, but we'll use the 
     value of --db to generate the unique resource name for the data asset.
     
     For example, if your production database is 'prod_service_one', but your test database is 'test_service_one', 
@@ -129,15 +152,15 @@
 )
 @optgroup.option(
     "--schema",
     "-s",
     type=str,
     help="""The schema of the production database where the table(s) you want to register are located. Despite not 
     needing to connect to the production database, the schema name is still needed to generate the unique resource 
-    name for the data asset. For example, a Postgres resource name is 'postgres://<host>:<port>/<db>/<schema>/<table>'
+    name for the data asset. For example, a Postgres resource name is 'postgres://<host>:<port>:<db>.<schema>.<table>'
     
     Database naming convention frequently includes the environment (production/development/test/staging) in the 
     schema name, so this value may not match the name of the schema in the proxy database instance. If this is 
     the case, you can set the --proxy-schema value to the name of the schema in the proxy instance, but we'll use the 
     value of --schema to generate the unique resource name for the data asset.
     
     For example, if your production schema is 'production', but your test database is 'test',
```

### Comparing `gable-0.1.0/gable/commands/ping.py` & `gable-0.2.1/gable/commands/ping.py`

 * *Files identical despite different names*

### Comparing `gable-0.1.0/gable/helpers/check.py` & `gable-0.2.1/gable/helpers/check.py`

 * *Files identical despite different names*

### Comparing `gable-0.1.0/gable/helpers/contract.py` & `gable-0.2.1/gable/helpers/contract.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import os
 from typing import Any, Dict, List
 import click
-from gable.helpers.repo_interactions import get_git_info
-from gable.openapi import ContractInput, PostContractRequest
+from gable.helpers.repo_interactions import get_git_repo_info
+from gable.openapi import ContractInput, PostContractRequest, Status
+import git
+from requests import get
 
 
 def load_contract_from_file(file: click.File) -> Dict[str, Any]:
     if file.name.endswith(".yaml") or file.name.endswith(".yml"):
         import yaml
 
         try:
@@ -29,19 +32,29 @@
     contractFiles: List[click.File],
 ) -> PostContractRequest:
     contracts = []
     for contractFile in contractFiles:
         contract = load_contract_from_file(contractFile)
         if "id" not in contract:
             raise click.ClickException(f"{contractFile}:\n\tContract must have an id.")
+        git_info = get_git_repo_info()
+        relative_path = os.path.relpath(contractFile.name, git_info["localRepoRootDir"])
+        if relative_path.startswith(".."):
+            raise click.ClickException(
+                f"{contractFile.name}:\n\tContract must be located within the git repo where gable is being executed ({git_info['localRepoRootDir']})."
+            )
         contractInput = ContractInput(
             id=contract["id"],
             version="0.0.1",  # This should be server calculated
-            status="ACTIVE",
-            **get_git_info(),  # type: ignore
+            status=Status("ACTIVE"),
             reviewers=[],  # This should be info accessible from a github PR integration
+            filePath=relative_path,
             contractSpec=contract,
+            gitHash=git_info["gitHash"],
+            gitRepo=git_info["gitRepo"],  # type: ignore
+            gitUser=git_info["gitUser"],
+            mergedAt=git_info["mergedAt"],
         )
         contracts.append(contractInput)
     return PostContractRequest(
         __root__=contracts,
     )
```

### Comparing `gable-0.1.0/gable/helpers/data_asset.py` & `gable-0.2.1/gable/helpers/data_asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import click
 import json
 from typing import Any, Optional, Union
 from gable.client import GableClient
 from gable.readers.dbapi import DbapiReader
 from gable.readers.file import get_file
-from gable.helpers.repo_interactions import GitInfo, get_git_info, get_git_ssh_file_path
+from gable.helpers.repo_interactions import get_git_ssh_file_path
 
 
 def standardize_source_type(source_type: str) -> str:
     return source_type.lower()
 
 
 def validate_db_input_args(user: str, password: str, db: str) -> None:
```

### Comparing `gable-0.1.0/gable/helpers/multi_option.py` & `gable-0.2.1/gable/helpers/multi_option.py`

 * *Files identical despite different names*

### Comparing `gable-0.1.0/gable/openapi.py` & `gable-0.2.1/gable/openapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,20 @@
     )
     status: Status = Field(..., description="status of the contract")
     gitHash: constr(min_length=40, max_length=40) = Field(
         ...,
         description="full length git hash corresponding to the commit this contract was added/updated",
     )
     gitRepo: AnyUrl = Field(
-        ..., description="full link to the github repo this contract lives in"
+        ..., description="full link to the git repo this contract lives in"
     )
     gitUser: str = Field(..., description="git user who added/updated this contract")
+    fileUri: AnyUrl = Field(
+        ..., description="full link to the file in the repo that contains this contract"
+    )
     reviewers: Optional[List[str]] = Field(
         None,
         description="optional list of users who reviewed the merged PR that this contract added/updated in",
     )
     mergedAt: datetime = Field(
         ...,
         description="date time at which the PR that added/updated this contract was merged",
@@ -68,21 +71,24 @@
     )
     status: Status = Field(..., description="status of the contract")
     gitHash: constr(min_length=40, max_length=40) = Field(
         ...,
         description="full length git hash corresponding to the commit this contract was added/updated",
     )
     gitRepo: AnyUrl = Field(
-        ..., description="full link to the github repo this contract lives in"
+        ..., description="full link to the git repo this contract lives in"
     )
     gitUser: str = Field(..., description="git user who added/updated this contract")
     reviewers: Optional[List[str]] = Field(
         None,
         description="optional list of users who reviewed the merged PR that this contract added/updated in",
     )
+    filePath: constr(regex=r"^([^/]+\/)*[^/]+$") = Field(
+        ..., description="path to the contract file from the root of the git repository"
+    )
     mergedAt: datetime = Field(
         ...,
         description="date time at which the PR that added/updated this contract was merged",
     )
     contractSpec: Any = Field(..., description="contract spec")
 
 
@@ -249,14 +255,23 @@
         ..., description="a boolean indicating if the lineage integration is valid"
     )
     message: Optional[str] = Field(
         None, description="a message indicating why the lineage integration is invalid"
     )
 
 
+class DataAssetId(BaseModel):
+    __root__: constr(
+        regex=r"^(protobuf|avro|json_schema|postgres|mysql|snowflake|bigquery)://(?=.*[a-zA-Z0-9])[a-zA-Z0-9_@\.:/-]+:(?=.*[a-zA-Z0-9])[a-zA-Z0-9_\./-]+$"
+    ) = Field(
+        ...,
+        description="The unique identifier of the data asset. It follows the pattern '{data_asset_type}://{data_asset_namespace}:{data_asset_name}'",
+    )
+
+
 class MarquezId(BaseModel):
     namespace: str = Field(..., description="The namespace of the Marquez dataset.")
     name: str = Field(..., description="The name of the Marquez dataset.")
 
 
 class FieldModel(BaseModel):
     name: str = Field(..., description="The name of the field.")
@@ -264,15 +279,15 @@
     tags: Optional[List[str]] = Field(None, description="List of tags.")
     description: Optional[str] = Field(
         None, description="The description of the field."
     )
 
 
 class DataAsset(BaseModel):
-    id: str = Field(..., description="The unique identifier of the data asset.")
+    id: DataAssetId
     marquezId: MarquezId = Field(..., description="The ID of the dataset.")
     type: str = Field(..., description="The type of the data asset.")
     name: str = Field(..., description="The **logical** name of the data asset.")
     physicalName: Optional[str] = Field(
         None, description="The **physical** name of the data asset."
     )
     createdAt: Optional[datetime] = Field(
@@ -356,28 +371,32 @@
     __root__: ContractOutput
 
 
 class ContractSpec(BaseModel):
     id: UUID = Field(
         ..., description="Unique identifier for the contract in UUID format"
     )
-    dataAssetResourceName: str = Field(
-        ..., description="Resource name of the data asset"
-    )
+    dataAssetResourceName: DataAssetId
     doc: str = Field(..., description="Description of the contract")
-    name: str = Field(..., description="Name of the contract")
-    namespace: str = Field(..., description="Namespace of the contract")
+    name: constr(regex=r"^(?=.*[a-zA-Z0-9])[a-zA-Z0-9_]+$") = Field(
+        ...,
+        description="The name of the contract. When combined with the contract namespace, it represents a unique name in the Gable platform.  Only alphanumeric characters (upper and lowercase) and underscores are allowed",
+    )
+    namespace: constr(regex=r"^(?=.*[a-zA-Z0-9])[a-zA-Z0-9_\.]+$") = Field(
+        ...,
+        description="The namespace of the contract. When combined with the contract name, it represents a unique name in the Gable platform. Only alphanumeric characters (upper and lowercase), underscores, and periods are allowed",
+    )
     owner: str = Field(..., description="Owner of the contract")
     schema_: List[ContractSpecSchemaProperty] = Field(
         ..., alias="schema", description="Schema of the contract"
     )
 
 
 class Type2(Enum):
-    PROTO = "PROTO"
+    PROTOBUF = "PROTOBUF"
     AVRO = "AVRO"
     JSON_SCHEMA = "JSON_SCHEMA"
     POSTGRES = "POSTGRES"
     SNOWFLAKE = "SNOWFLAKE"
 
 
 class CheckContractViolationRequest(BaseModel):
```

### Comparing `gable-0.1.0/gable/readers/dbapi.py` & `gable-0.2.1/gable/readers/dbapi.py`

 * *Files identical despite different names*

### Comparing `gable-0.1.0/gable/readers/mysql.py` & `gable-0.2.1/gable/readers/mysql.py`

 * *Files identical despite different names*

### Comparing `gable-0.1.0/gable/readers/postgres.py` & `gable-0.2.1/gable/readers/postgres.py`

 * *Files identical despite different names*

### Comparing `gable-0.1.0/pyproject.toml` & `gable-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "gable"
-version = "0.1.0"
+version = "0.2.1"
 description = "Command line interface to interact with Gable API"
 authors = ["Gable.ai <engineers@gable.ai>"]
 readme = "README.md"
 packages = [{include = "gable"}]
 
 [tool.poetry.dependencies]
 GitPython = "^3.1.31"
-python = ">=3.10.0,<4.0.0"
+python = ">=3.10,<3.11"
 click = "^8.1.3"
 pydantic = "^1.10.7"
 requests = "^2.31.0"
 pyyaml = "^6.0.0"
 psycopg2-binary = {version = '>=2.7', optional = true}
 mysql-connector-python = {version = "^8.0.33", optional = true}
 click-option-group = "^0.5.6"
@@ -26,18 +26,20 @@
 black = "^23.3.0"
 build = "^0.10.0"
 datamodel-code-generator = "^0.19.0"
 poethepoet = "^0.20.0"
 pytest = "^7.3.1"
 pyright = "^1.1.317"
 twine = "^4.0.2"
+waiting = "^1.4.1"
 
 [tool.poetry.extras]
 postgres = ['psycopg2-binary']
 mysql = ['mysql-connector-python']
+all = ['psycopg2-binary', 'mysql-connector-python']
 
 [tool.poe.tasks.generate_types]
 shell = "bash scripts/generate_types.sh"
 
 [tool.poe.tasks.publish_cli]
 shell = "sh scripts/publish_cli.sh"
```

### Comparing `gable-0.1.0/PKG-INFO` & `gable-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: gable
-Version: 0.1.0
+Version: 0.2.1
 Summary: Command line interface to interact with Gable API
 Author: Gable.ai
 Author-email: engineers@gable.ai
-Requires-Python: >=3.10.0,<4.0.0
+Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
 Provides-Extra: mysql
 Provides-Extra: postgres
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-option-group (>=0.5.6,<0.6.0)
 Requires-Dist: giturlparse (>=0.10.0,<0.11.0)
-Requires-Dist: mysql-connector-python (>=8.0.33,<9.0.0) ; extra == "mysql"
-Requires-Dist: psycopg2-binary (>=2.7) ; extra == "postgres"
+Requires-Dist: mysql-connector-python (>=8.0.33,<9.0.0) ; extra == "mysql" or extra == "all"
+Requires-Dist: psycopg2-binary (>=2.7) ; extra == "postgres" or extra == "all"
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Description-Content-Type: text/markdown
 
 # Gable CLI
@@ -30,14 +30,15 @@
 gable --help
 Usage: gable [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --endpoint TEXT  Customer API endpoint for Gable, in the format
                    https://api.company.gable.ai/
   --api-key TEXT   API Key for Gable
+  --version        Show the version and exit.
   --help           Show this message and exit.
 
 Commands:
   auth        View configured Gable authentication information
   contract    Validate/publish contracts and check data asset compliance
   data-asset  Commands for data assets
   ping        Pings the Gable API to check for connectivity
```

