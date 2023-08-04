# Comparing `tmp/gamium-2.0.2.tar.gz` & `tmp/gamium-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamium-2.0.2.tar", max compression
+gzip compressed data, was "gamium-2.0.3.tar", max compression
```

## Comparing `gamium-2.0.2.tar` & `gamium-2.0.3.tar`

### file list

```diff
@@ -1,106 +1,109 @@
--rw-r--r--   0        0        0     1007 2023-06-14 11:50:40.607475 gamium-2.0.2/README.md
--rw-r--r--   0        0        0      626 2023-06-14 11:50:40.613159 gamium-2.0.2/gamium/__init__.py
--rw-r--r--   0        0        0      500 2023-06-14 11:50:40.613219 gamium-2.0.2/gamium/__main__.py
--rw-r--r--   0        0        0    11229 2023-06-14 11:50:40.613344 gamium-2.0.2/gamium/actions/action_chain.py
--rw-r--r--   0        0        0     1449 2023-06-14 11:50:40.613418 gamium-2.0.2/gamium/actions/key_by.py
--rw-r--r--   0        0        0      471 2023-06-14 11:50:40.613535 gamium-2.0.2/gamium/condition/condition.py
--rw-r--r--   0        0        0     2138 2023-06-14 11:50:40.613608 gamium-2.0.2/gamium/condition/until.py
--rw-r--r--   0        0        0      245 2023-06-14 11:50:40.613675 gamium-2.0.2/gamium/condition/wait_condition.py
--rw-r--r--   0        0        0      269 2023-06-14 11:50:40.613784 gamium-2.0.2/gamium/errors/gamium_error.py
--rw-r--r--   0        0        0     6303 2023-06-14 11:50:40.613864 gamium-2.0.2/gamium/gamium_client.py
--rw-r--r--   0        0        0     8498 2023-06-14 11:50:40.613955 gamium-2.0.2/gamium/gamium_service.py
--rw-r--r--   0        0        0     1248 2023-06-14 11:50:40.614021 gamium-2.0.2/gamium/igamium_client.py
--rw-r--r--   0        0        0       62 2023-06-14 11:50:40.614114 gamium-2.0.2/gamium/internal/__init__.py
--rw-r--r--   0        0        0     1147 2023-06-14 11:50:40.614187 gamium-2.0.2/gamium/internal/logger.py
--rw-r--r--   0        0        0      672 2023-06-14 11:50:40.614244 gamium-2.0.2/gamium/internal/size_prefixed_recv_queue.py
--rw-r--r--   0        0        0      349 2023-06-14 11:50:40.614339 gamium-2.0.2/gamium/locator/by.py
--rw-r--r--   0        0        0       59 2023-06-14 11:50:40.614392 gamium-2.0.2/gamium/locator/locator.py
--rw-r--r--   0        0        0      906 2023-06-14 11:50:40.614465 gamium-2.0.2/gamium/locator/rpc_by.py
--rw-r--r--   0        0        0       47 2023-06-14 11:50:40.614515 gamium-2.0.2/gamium/locator/rpc_locator.py
--rw-r--r--   0        0        0     1996 2023-06-14 11:50:40.614611 gamium-2.0.2/gamium/object/player.py
--rw-r--r--   0        0        0     3925 2023-06-14 11:50:40.614688 gamium-2.0.2/gamium/object/ui_element.py
--rw-r--r--   0        0        0      390 2023-06-14 11:50:40.614806 gamium-2.0.2/gamium/options/__init__.py
--rw-r--r--   0        0        0      142 2023-06-14 11:50:40.614872 gamium-2.0.2/gamium/options/action_click_options.py
--rw-r--r--   0        0        0      204 2023-06-14 11:50:40.614933 gamium-2.0.2/gamium/options/action_drag_options.py
--rw-r--r--   0        0        0       92 2023-06-14 11:50:40.614988 gamium-2.0.2/gamium/options/action_move_options.py
--rw-r--r--   0        0        0      144 2023-06-14 11:50:40.615054 gamium-2.0.2/gamium/options/action_scroll_options.py
--rw-r--r--   0        0        0      171 2023-06-14 11:50:40.615119 gamium-2.0.2/gamium/options/execute_rpc_options.py
--rw-r--r--   0        0        0      132 2023-06-14 11:50:40.615176 gamium-2.0.2/gamium/options/find_objects_options.py
--rw-r--r--   0        0        0      374 2023-06-14 11:50:40.615231 gamium-2.0.2/gamium/options/move_player_options.py
--rw-r--r--   0        0        0      262 2023-06-14 11:50:40.615305 gamium-2.0.2/gamium/options/query_object_interactable_options.py
--rw-r--r--   0        0        0      139 2023-06-14 11:50:40.615367 gamium-2.0.2/gamium/options/send_key_options.py
--rw-r--r--   0        0        0       89 2023-06-14 11:50:40.615419 gamium-2.0.2/gamium/options/set_text_options.py
--rw-r--r--   0        0        0      362 2023-06-14 11:50:40.615480 gamium-2.0.2/gamium/options/wait_options.py
--rw-r--r--   0        0        0        0 2023-06-15 11:26:24.105569 gamium-2.0.2/gamium/protocol/__init__.py
--rw-r--r--   0        0        0      597 2023-06-15 11:30:59.400220 gamium-2.0.2/gamium/protocol/functions.py
--rw-r--r--   0        0        0     1988 2023-06-15 11:26:24.096767 gamium-2.0.2/gamium/protocol/generated/Packets/ActionParam.py
--rw-r--r--   0        0        0     4353 2023-06-15 11:26:24.095939 gamium-2.0.2/gamium/protocol/generated/Packets/ActionParamSingle.py
--rw-r--r--   0        0        0     2917 2023-06-15 11:26:24.103605 gamium-2.0.2/gamium/protocol/generated/Packets/ActionResult.py
--rw-r--r--   0        0        0     2909 2023-06-15 11:26:24.098368 gamium-2.0.2/gamium/protocol/generated/Packets/Actions/AppQuitParam.py
--rw-r--r--   0        0        0     4175 2023-06-15 11:26:24.099176 gamium-2.0.2/gamium/protocol/generated/Packets/Actions/InputKeyParam.py
--rw-r--r--   0        0        0     5031 2023-06-15 11:26:24.098694 gamium-2.0.2/gamium/protocol/generated/Packets/Actions/InputMouseParam.py
--rw-r--r--   0        0        0     3357 2023-06-15 11:26:24.099348 gamium-2.0.2/gamium/protocol/generated/Packets/Actions/InputSetTextParam.py
--rw-r--r--   0        0        0      156 2023-06-15 11:26:24.099989 gamium-2.0.2/gamium/protocol/generated/Packets/Actions/MovePlayerBy.py
--rw-r--r--   0        0        0     6404 2023-06-15 11:26:24.099518 gamium-2.0.2/gamium/protocol/generated/Packets/Actions/MovePlayerParam.py
--rw-r--r--   0        0        0     2213 2023-06-15 11:26:24.099726 gamium-2.0.2/gamium/protocol/generated/Packets/Actions/SleepParam.py
--rw-r--r--   0        0        0        0 2023-06-15 11:26:24.099011 gamium-2.0.2/gamium/protocol/generated/Packets/Actions/__init__.py
--rw-r--r--   0        0        0     3665 2023-06-15 11:26:24.094786 gamium-2.0.2/gamium/protocol/generated/Packets/ActionsParam.py
--rw-r--r--   0        0        0     4251 2023-06-15 11:26:24.089711 gamium-2.0.2/gamium/protocol/generated/Packets/ActionsResult.py
--rw-r--r--   0        0        0     3323 2023-06-15 11:26:24.102407 gamium-2.0.2/gamium/protocol/generated/Packets/ChangeConfigurationParam.py
--rw-r--r--   0        0        0     2116 2023-06-15 11:26:24.086680 gamium-2.0.2/gamium/protocol/generated/Packets/ChangeConfigurationResult.py
--rw-r--r--   0        0        0     3503 2023-06-15 11:26:24.100216 gamium-2.0.2/gamium/protocol/generated/Packets/DumpObjectsHierarchyParam.py
--rw-r--r--   0        0        0     4913 2023-06-15 11:26:24.100866 gamium-2.0.2/gamium/protocol/generated/Packets/DumpObjectsHierarchyResult.py
--rw-r--r--   0        0        0     2799 2023-06-15 11:26:24.090396 gamium-2.0.2/gamium/protocol/generated/Packets/Env.py
--rw-r--r--   0        0        0     6064 2023-06-15 11:26:24.095273 gamium-2.0.2/gamium/protocol/generated/Packets/ExecuteRpcParam.py
--rw-r--r--   0        0        0     2634 2023-06-15 11:26:24.089056 gamium-2.0.2/gamium/protocol/generated/Packets/ExecuteRpcResult.py
--rw-r--r--   0        0        0     3093 2023-06-15 11:26:24.093511 gamium-2.0.2/gamium/protocol/generated/Packets/FindObjectsParam.py
--rw-r--r--   0        0        0     4307 2023-06-15 11:26:24.093972 gamium-2.0.2/gamium/protocol/generated/Packets/FindObjectsResult.py
--rw-r--r--   0        0        0     1941 2023-06-15 11:26:24.091053 gamium-2.0.2/gamium/protocol/generated/Packets/GetPageSourceParam.py
--rw-r--r--   0        0        0     2758 2023-06-15 11:26:24.092906 gamium-2.0.2/gamium/protocol/generated/Packets/GetPageSourceResult.py
--rw-r--r--   0        0        0     2437 2023-06-15 11:26:24.100388 gamium-2.0.2/gamium/protocol/generated/Packets/HelloParam.py
--rw-r--r--   0        0        0     8271 2023-06-15 11:26:24.101353 gamium-2.0.2/gamium/protocol/generated/Packets/HelloResult.py
--rw-r--r--   0        0        0     4330 2023-06-15 11:26:24.097724 gamium-2.0.2/gamium/protocol/generated/Packets/InspectObjectOnScreenParam.py
--rw-r--r--   0        0        0     5826 2023-06-15 11:26:24.095600 gamium-2.0.2/gamium/protocol/generated/Packets/InspectObjectOnScreenResult.py
--rw-r--r--   0        0        0     2874 2023-06-15 11:26:24.092195 gamium-2.0.2/gamium/protocol/generated/Packets/InspectObjectWithIdParam.py
--rw-r--r--   0        0        0     3294 2023-06-15 11:26:24.090095 gamium-2.0.2/gamium/protocol/generated/Packets/InspectObjectWithIdResult.py
--rw-r--r--   0        0        0     4413 2023-06-15 11:26:24.097098 gamium-2.0.2/gamium/protocol/generated/Packets/QueryObjectInteractableParam.py
--rw-r--r--   0        0        0     2950 2023-06-15 11:26:24.100590 gamium-2.0.2/gamium/protocol/generated/Packets/QueryObjectInteractableResult.py
--rw-r--r--   0        0        0     1916 2023-06-15 11:26:24.091450 gamium-2.0.2/gamium/protocol/generated/Packets/QueryProfileParam.py
--rw-r--r--   0        0        0     2466 2023-06-15 11:26:24.090746 gamium-2.0.2/gamium/protocol/generated/Packets/QueryProfileResult.py
--rw-r--r--   0        0        0     1891 2023-06-15 11:26:24.096444 gamium-2.0.2/gamium/protocol/generated/Packets/QueryScreenParam.py
--rw-r--r--   0        0        0     3030 2023-06-15 11:26:24.102985 gamium-2.0.2/gamium/protocol/generated/Packets/QueryScreenResult.py
--rw-r--r--   0        0        0        0 2023-06-15 11:26:24.094347 gamium-2.0.2/gamium/protocol/generated/Packets/__init__.py
--rw-r--r--   0        0        0     3752 2023-06-15 11:26:24.083611 gamium-2.0.2/gamium/protocol/generated/Param.py
--rw-r--r--   0        0        0     5254 2023-06-15 11:26:24.082821 gamium-2.0.2/gamium/protocol/generated/Request.py
--rw-r--r--   0        0        0     6436 2023-06-15 11:26:24.084104 gamium-2.0.2/gamium/protocol/generated/Response.py
--rw-r--r--   0        0        0     3826 2023-06-15 11:26:24.084580 gamium-2.0.2/gamium/protocol/generated/Result.py
--rw-r--r--   0        0        0     3222 2023-06-15 11:26:24.076068 gamium-2.0.2/gamium/protocol/generated/Types/Configuration.py
--rw-r--r--   0        0        0     1146 2023-06-15 11:26:24.081707 gamium-2.0.2/gamium/protocol/generated/Types/ErrorCode.py
--rw-r--r--   0        0        0     2962 2023-06-15 11:26:24.076466 gamium-2.0.2/gamium/protocol/generated/Types/ErrorResult.py
--rw-r--r--   0        0        0      164 2023-06-15 11:26:24.082235 gamium-2.0.2/gamium/protocol/generated/Types/ExecuteRpcBy.py
--rw-r--r--   0        0        0      161 2023-06-15 11:26:24.079125 gamium-2.0.2/gamium/protocol/generated/Types/InputKeyBy.py
--rw-r--r--   0        0        0      147 2023-06-15 11:26:24.080951 gamium-2.0.2/gamium/protocol/generated/Types/InputKeyPressType.py
--rw-r--r--   0        0        0      168 2023-06-15 11:26:24.078700 gamium-2.0.2/gamium/protocol/generated/Types/InputMouseButtonCode.py
--rw-r--r--   0        0        0      177 2023-06-15 11:26:24.077804 gamium-2.0.2/gamium/protocol/generated/Types/InputMousePressType.py
--rw-r--r--   0        0        0     5920 2023-06-15 11:26:24.080483 gamium-2.0.2/gamium/protocol/generated/Types/ObjectHierarchyNode.py
--rw-r--r--   0        0        0    10803 2023-06-15 11:26:24.078418 gamium-2.0.2/gamium/protocol/generated/Types/ObjectInfo.py
--rw-r--r--   0        0        0     2955 2023-06-15 11:26:24.078924 gamium-2.0.2/gamium/protocol/generated/Types/ObjectLocator.py
--rw-r--r--   0        0        0      146 2023-06-15 11:26:24.081299 gamium-2.0.2/gamium/protocol/generated/Types/ObjectLocatorBy.py
--rw-r--r--   0        0        0      158 2023-06-15 11:26:24.076250 gamium-2.0.2/gamium/protocol/generated/Types/ObjectType.py
--rw-r--r--   0        0        0     5147 2023-06-15 11:26:24.075832 gamium-2.0.2/gamium/protocol/generated/Types/ObjectsHierarchy.py
--rw-r--r--   0        0        0     7471 2023-06-15 11:26:24.074991 gamium-2.0.2/gamium/protocol/generated/Types/Unity/UnityKeyCode.py
--rw-r--r--   0        0        0     1944 2023-06-15 11:26:24.075558 gamium-2.0.2/gamium/protocol/generated/Types/Unity/UnityKeyboard.py
--rw-r--r--   0        0        0        0 2023-06-15 11:26:24.075303 gamium-2.0.2/gamium/protocol/generated/Types/Unity/__init__.py
--rw-r--r--   0        0        0     1681 2023-06-15 11:26:24.077009 gamium-2.0.2/gamium/protocol/generated/Types/Vector2.py
--rw-r--r--   0        0        0     1947 2023-06-15 11:26:24.077618 gamium-2.0.2/gamium/protocol/generated/Types/Vector3.py
--rw-r--r--   0        0        0     2212 2023-06-15 11:26:24.078160 gamium-2.0.2/gamium/protocol/generated/Types/Vector4.py
--rw-r--r--   0        0        0        0 2023-06-15 11:26:24.077402 gamium-2.0.2/gamium/protocol/generated/Types/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 11:26:24.083226 gamium-2.0.2/gamium/protocol/generated/__init__.py
--rw-r--r--   0        0        0     3296 2023-06-15 11:31:15.207252 gamium-2.0.2/gamium/protocol/types.py
--rw-r--r--   0        0        0     3887 2023-06-14 11:50:40.615607 gamium-2.0.2/gamium/ui/ui.py
--rw-r--r--   0        0        0       80 2023-06-14 11:50:40.615691 gamium-2.0.2/gamium/utils/generics.py
--rw-r--r--   0        0        0       79 2023-06-14 11:50:40.615755 gamium-2.0.2/gamium/utils/time.py
--rw-r--r--   0        0        0      598 2023-06-14 11:50:40.615818 gamium-2.0.2/gamium/utils/try_utils.py
--rw-r--r--   0        0        0     1873 2023-06-14 11:50:40.615906 gamium-2.0.2/gamium/utils/wait.py
--rw-r--r--   0        0        0      278 2023-06-15 11:32:08.731408 gamium-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 gamium-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1007 2023-05-30 02:56:42.090478 gamium-2.0.3/README.md
+-rw-r--r--   0        0        0      713 2023-08-04 09:39:16.231374 gamium-2.0.3/gamium/__init__.py
+-rw-r--r--   0        0        0      596 2023-08-04 09:39:16.231715 gamium-2.0.3/gamium/__main__.py
+-rw-r--r--   0        0        0    11199 2023-08-04 09:39:16.232022 gamium-2.0.3/gamium/actions/action_chain.py
+-rw-r--r--   0        0        0     1449 2023-05-30 02:56:42.104757 gamium-2.0.3/gamium/actions/key_by.py
+-rw-r--r--   0        0        0      471 2023-05-30 02:56:42.105088 gamium-2.0.3/gamium/condition/condition.py
+-rw-r--r--   0        0        0     2138 2023-05-30 02:56:42.105471 gamium-2.0.3/gamium/condition/until.py
+-rw-r--r--   0        0        0      245 2023-05-30 02:56:42.105619 gamium-2.0.3/gamium/condition/wait_condition.py
+-rw-r--r--   0        0        0      269 2023-05-30 02:56:42.106207 gamium-2.0.3/gamium/errors/gamium_error.py
+-rw-r--r--   0        0        0     6353 2023-08-04 09:39:16.232308 gamium-2.0.3/gamium/gamium_client.py
+-rw-r--r--   0        0        0     1318 2023-08-04 09:39:16.232628 gamium-2.0.3/gamium/igamium_client.py
+-rw-r--r--   0        0        0     4137 2023-08-04 09:39:16.233063 gamium-2.0.3/gamium/igamium_service.py
+-rw-r--r--   0        0        0       62 2023-05-30 02:56:42.107518 gamium-2.0.3/gamium/internal/__init__.py
+-rw-r--r--   0        0        0     1147 2023-05-30 02:56:42.107769 gamium-2.0.3/gamium/internal/logger.py
+-rw-r--r--   0        0        0      672 2023-05-30 02:56:42.108057 gamium-2.0.3/gamium/internal/size_prefixed_recv_queue.py
+-rw-r--r--   0        0        0      349 2023-05-30 02:56:42.108210 gamium-2.0.3/gamium/locator/by.py
+-rw-r--r--   0        0        0       59 2023-05-30 02:56:42.108434 gamium-2.0.3/gamium/locator/locator.py
+-rw-r--r--   0        0        0      906 2023-05-30 02:56:42.108572 gamium-2.0.3/gamium/locator/rpc_by.py
+-rw-r--r--   0        0        0       47 2023-05-30 02:56:42.108962 gamium-2.0.3/gamium/locator/rpc_locator.py
+-rw-r--r--   0        0        0     1999 2023-08-04 09:39:16.233306 gamium-2.0.3/gamium/object/player.py
+-rw-r--r--   0        0        0     3928 2023-08-04 09:39:16.233538 gamium-2.0.3/gamium/object/ui_element.py
+-rw-r--r--   0        0        0      390 2023-05-30 02:56:42.109820 gamium-2.0.3/gamium/options/__init__.py
+-rw-r--r--   0        0        0      142 2023-05-30 02:56:42.109956 gamium-2.0.3/gamium/options/action_click_options.py
+-rw-r--r--   0        0        0      204 2023-05-30 02:56:42.110102 gamium-2.0.3/gamium/options/action_drag_options.py
+-rw-r--r--   0        0        0       92 2023-05-30 02:56:42.110492 gamium-2.0.3/gamium/options/action_move_options.py
+-rw-r--r--   0        0        0      144 2023-05-30 02:56:42.110628 gamium-2.0.3/gamium/options/action_scroll_options.py
+-rw-r--r--   0        0        0      171 2023-05-30 02:56:42.110847 gamium-2.0.3/gamium/options/execute_rpc_options.py
+-rw-r--r--   0        0        0      132 2023-05-30 02:56:42.111002 gamium-2.0.3/gamium/options/find_objects_options.py
+-rw-r--r--   0        0        0      374 2023-05-30 02:56:42.111161 gamium-2.0.3/gamium/options/move_player_options.py
+-rw-r--r--   0        0        0      262 2023-05-30 02:56:42.111311 gamium-2.0.3/gamium/options/query_object_interactable_options.py
+-rw-r--r--   0        0        0      139 2023-05-30 02:56:42.111458 gamium-2.0.3/gamium/options/send_key_options.py
+-rw-r--r--   0        0        0       89 2023-05-30 02:56:42.111703 gamium-2.0.3/gamium/options/set_text_options.py
+-rw-r--r--   0        0        0      362 2023-05-30 02:56:42.111866 gamium-2.0.3/gamium/options/wait_options.py
+-rw-r--r--   0        0        0        0 2023-06-23 03:07:41.040745 gamium-2.0.3/gamium/protocol/__init__.py
+-rw-r--r--   0        0        0      597 2023-06-23 03:07:41.041613 gamium-2.0.3/gamium/protocol/functions.py
+-rw-r--r--   0        0        0     1988 2023-06-23 03:07:41.042200 gamium-2.0.3/gamium/protocol/generated/Packets/ActionParam.py
+-rw-r--r--   0        0        0     4353 2023-06-23 03:07:41.042754 gamium-2.0.3/gamium/protocol/generated/Packets/ActionParamSingle.py
+-rw-r--r--   0        0        0     2917 2023-06-23 03:07:41.043015 gamium-2.0.3/gamium/protocol/generated/Packets/ActionResult.py
+-rw-r--r--   0        0        0     2909 2023-06-23 03:07:41.043554 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/AppQuitParam.py
+-rw-r--r--   0        0        0     4175 2023-06-23 03:07:41.043877 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/InputKeyParam.py
+-rw-r--r--   0        0        0     5031 2023-06-23 03:07:41.044026 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/InputMouseParam.py
+-rw-r--r--   0        0        0     3357 2023-06-23 03:07:41.044299 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/InputSetTextParam.py
+-rw-r--r--   0        0        0      156 2023-06-23 03:07:41.044529 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/MovePlayerBy.py
+-rw-r--r--   0        0        0     6404 2023-06-23 03:07:41.044671 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/MovePlayerParam.py
+-rw-r--r--   0        0        0     2213 2023-06-23 03:07:41.044813 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/SleepParam.py
+-rw-r--r--   0        0        0        0 2023-06-23 03:07:41.044841 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/__init__.py
+-rw-r--r--   0        0        0     3665 2023-06-23 03:07:41.045196 gamium-2.0.3/gamium/protocol/generated/Packets/ActionsParam.py
+-rw-r--r--   0        0        0     4251 2023-06-23 03:07:41.045364 gamium-2.0.3/gamium/protocol/generated/Packets/ActionsResult.py
+-rw-r--r--   0        0        0     3323 2023-06-23 03:07:41.045522 gamium-2.0.3/gamium/protocol/generated/Packets/ChangeConfigurationParam.py
+-rw-r--r--   0        0        0     2116 2023-06-23 03:07:41.045666 gamium-2.0.3/gamium/protocol/generated/Packets/ChangeConfigurationResult.py
+-rw-r--r--   0        0        0     3503 2023-06-23 03:07:41.045816 gamium-2.0.3/gamium/protocol/generated/Packets/DumpObjectsHierarchyParam.py
+-rw-r--r--   0        0        0     4913 2023-06-23 03:07:41.045974 gamium-2.0.3/gamium/protocol/generated/Packets/DumpObjectsHierarchyResult.py
+-rw-r--r--   0        0        0     2799 2023-06-23 03:07:41.046117 gamium-2.0.3/gamium/protocol/generated/Packets/Env.py
+-rw-r--r--   0        0        0     6064 2023-06-23 03:07:41.046266 gamium-2.0.3/gamium/protocol/generated/Packets/ExecuteRpcParam.py
+-rw-r--r--   0        0        0     2634 2023-06-23 03:07:41.046442 gamium-2.0.3/gamium/protocol/generated/Packets/ExecuteRpcResult.py
+-rw-r--r--   0        0        0     3093 2023-06-23 03:07:41.046596 gamium-2.0.3/gamium/protocol/generated/Packets/FindObjectsParam.py
+-rw-r--r--   0        0        0     4307 2023-06-23 03:07:41.046746 gamium-2.0.3/gamium/protocol/generated/Packets/FindObjectsResult.py
+-rw-r--r--   0        0        0     1941 2023-06-23 03:07:41.046830 gamium-2.0.3/gamium/protocol/generated/Packets/GetPageSourceParam.py
+-rw-r--r--   0        0        0     2758 2023-06-23 03:07:41.046890 gamium-2.0.3/gamium/protocol/generated/Packets/GetPageSourceResult.py
+-rw-r--r--   0        0        0     2437 2023-06-23 03:07:41.047254 gamium-2.0.3/gamium/protocol/generated/Packets/HelloParam.py
+-rw-r--r--   0        0        0     8271 2023-06-23 03:07:41.047529 gamium-2.0.3/gamium/protocol/generated/Packets/HelloResult.py
+-rw-r--r--   0        0        0     4330 2023-06-23 03:07:41.047684 gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectOnScreenParam.py
+-rw-r--r--   0        0        0     5826 2023-06-23 03:07:41.047851 gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectOnScreenResult.py
+-rw-r--r--   0        0        0     2874 2023-06-23 03:07:41.047995 gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectWithIdParam.py
+-rw-r--r--   0        0        0     3294 2023-06-23 03:07:41.048137 gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectWithIdResult.py
+-rw-r--r--   0        0        0     4413 2023-06-23 03:07:41.048299 gamium-2.0.3/gamium/protocol/generated/Packets/QueryObjectInteractableParam.py
+-rw-r--r--   0        0        0     2950 2023-06-23 03:07:41.048497 gamium-2.0.3/gamium/protocol/generated/Packets/QueryObjectInteractableResult.py
+-rw-r--r--   0        0        0     1916 2023-06-23 03:07:41.048656 gamium-2.0.3/gamium/protocol/generated/Packets/QueryProfileParam.py
+-rw-r--r--   0        0        0     2466 2023-06-23 03:07:41.048807 gamium-2.0.3/gamium/protocol/generated/Packets/QueryProfileResult.py
+-rw-r--r--   0        0        0     1891 2023-06-23 03:07:41.049179 gamium-2.0.3/gamium/protocol/generated/Packets/QueryScreenParam.py
+-rw-r--r--   0        0        0     3030 2023-06-23 03:07:41.049456 gamium-2.0.3/gamium/protocol/generated/Packets/QueryScreenResult.py
+-rw-r--r--   0        0        0        0 2023-06-23 03:07:41.049572 gamium-2.0.3/gamium/protocol/generated/Packets/__init__.py
+-rw-r--r--   0        0        0     3752 2023-06-23 03:07:41.049804 gamium-2.0.3/gamium/protocol/generated/Param.py
+-rw-r--r--   0        0        0     5254 2023-06-23 03:07:41.049965 gamium-2.0.3/gamium/protocol/generated/Request.py
+-rw-r--r--   0        0        0     6436 2023-06-23 03:07:41.050115 gamium-2.0.3/gamium/protocol/generated/Response.py
+-rw-r--r--   0        0        0     3826 2023-06-23 03:07:41.050191 gamium-2.0.3/gamium/protocol/generated/Result.py
+-rw-r--r--   0        0        0     3222 2023-06-23 03:07:41.050385 gamium-2.0.3/gamium/protocol/generated/Types/Configuration.py
+-rw-r--r--   0        0        0     1146 2023-06-23 03:07:41.050762 gamium-2.0.3/gamium/protocol/generated/Types/ErrorCode.py
+-rw-r--r--   0        0        0     2962 2023-06-23 03:07:41.051307 gamium-2.0.3/gamium/protocol/generated/Types/ErrorResult.py
+-rw-r--r--   0        0        0      164 2023-06-23 03:07:41.051617 gamium-2.0.3/gamium/protocol/generated/Types/ExecuteRpcBy.py
+-rw-r--r--   0        0        0      161 2023-06-23 03:07:41.051819 gamium-2.0.3/gamium/protocol/generated/Types/InputKeyBy.py
+-rw-r--r--   0        0        0      147 2023-06-23 03:07:41.052031 gamium-2.0.3/gamium/protocol/generated/Types/InputKeyPressType.py
+-rw-r--r--   0        0        0      168 2023-06-23 03:07:41.052276 gamium-2.0.3/gamium/protocol/generated/Types/InputMouseButtonCode.py
+-rw-r--r--   0        0        0      177 2023-06-23 03:07:41.052478 gamium-2.0.3/gamium/protocol/generated/Types/InputMousePressType.py
+-rw-r--r--   0        0        0     5920 2023-06-23 03:07:41.052652 gamium-2.0.3/gamium/protocol/generated/Types/ObjectHierarchyNode.py
+-rw-r--r--   0        0        0    10803 2023-06-23 03:07:41.052832 gamium-2.0.3/gamium/protocol/generated/Types/ObjectInfo.py
+-rw-r--r--   0        0        0     2955 2023-06-23 03:07:41.052991 gamium-2.0.3/gamium/protocol/generated/Types/ObjectLocator.py
+-rw-r--r--   0        0        0      146 2023-06-23 03:07:41.053158 gamium-2.0.3/gamium/protocol/generated/Types/ObjectLocatorBy.py
+-rw-r--r--   0        0        0      158 2023-06-23 03:07:41.053307 gamium-2.0.3/gamium/protocol/generated/Types/ObjectType.py
+-rw-r--r--   0        0        0     5147 2023-06-23 03:07:41.053531 gamium-2.0.3/gamium/protocol/generated/Types/ObjectsHierarchy.py
+-rw-r--r--   0        0        0     7471 2023-06-23 03:07:41.053768 gamium-2.0.3/gamium/protocol/generated/Types/Unity/UnityKeyCode.py
+-rw-r--r--   0        0        0     1944 2023-06-23 03:07:41.053911 gamium-2.0.3/gamium/protocol/generated/Types/Unity/UnityKeyboard.py
+-rw-r--r--   0        0        0        0 2023-06-23 03:07:41.053939 gamium-2.0.3/gamium/protocol/generated/Types/Unity/__init__.py
+-rw-r--r--   0        0        0     1681 2023-06-23 03:07:41.054089 gamium-2.0.3/gamium/protocol/generated/Types/Vector2.py
+-rw-r--r--   0        0        0     1947 2023-06-23 03:07:41.054251 gamium-2.0.3/gamium/protocol/generated/Types/Vector3.py
+-rw-r--r--   0        0        0     2212 2023-06-23 03:07:41.054419 gamium-2.0.3/gamium/protocol/generated/Types/Vector4.py
+-rw-r--r--   0        0        0        0 2023-06-23 03:07:41.054453 gamium-2.0.3/gamium/protocol/generated/Types/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 03:07:41.054512 gamium-2.0.3/gamium/protocol/generated/__init__.py
+-rw-r--r--   0        0        0     3296 2023-06-23 03:07:41.055005 gamium-2.0.3/gamium/protocol/types.py
+-rw-r--r--   0        0        0     4664 2023-08-04 09:39:16.233895 gamium-2.0.3/gamium/tcp_gamium_service.py
+-rw-r--r--   0        0        0     3890 2023-08-04 09:39:16.234228 gamium-2.0.3/gamium/ui/ui.py
+-rw-r--r--   0        0        0      500 2023-08-04 09:39:16.234412 gamium-2.0.3/gamium/utils/bytes.py
+-rw-r--r--   0        0        0       80 2023-05-30 02:56:42.112384 gamium-2.0.3/gamium/utils/generics.py
+-rw-r--r--   0        0        0       79 2023-05-30 02:56:42.112716 gamium-2.0.3/gamium/utils/time.py
+-rw-r--r--   0        0        0      598 2023-05-30 02:56:42.112859 gamium-2.0.3/gamium/utils/try_utils.py
+-rw-r--r--   0        0        0     1980 2023-08-04 09:39:16.234617 gamium-2.0.3/gamium/utils/wait.py
+-rw-r--r--   0        0        0     4765 2023-08-04 09:39:16.235087 gamium-2.0.3/gamium/websocket_gamium_service.py
+-rw-r--r--   0        0        0      301 2023-08-04 09:44:15.776277 gamium-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 gamium-2.0.3/PKG-INFO
```

### Comparing `gamium-2.0.2/README.md` & `gamium-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/__init__.py` & `gamium-2.0.3/gamium/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from gamium.gamium_client import *
-from gamium.gamium_service import *
+from gamium.igamium_service import *
+from gamium.tcp_gamium_service import *
+from gamium.websocket_gamium_service import *
 from gamium.locator.by import *
 from gamium.locator.locator import *
 from gamium.locator.rpc_by import *
 from gamium.locator.rpc_locator import *
 from gamium.actions.key_by import *
 from gamium.actions.action_chain import *
 from gamium.condition.condition import *
```

### Comparing `gamium-2.0.2/gamium/actions/action_chain.py` & `gamium-2.0.3/gamium/actions/action_chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,28 +26,27 @@
 )
 from gamium.protocol.generated.Packets.Actions.MovePlayerParam import (
     MovePlayerParamT,
 )
 from gamium.protocol.generated.Packets.Actions.SleepParam import SleepParamT
 from gamium.protocol.generated.Types.Vector2 import Vector2T
 from gamium.protocol.generated.Types.Vector3 import Vector3T
-from gamium.gamium_service import create_actions
+from gamium.igamium_service import IGamiumService, create_actions
 from gamium.options import (
     ActionClickOptions,
     ActionDragOptions,
     ActionMoveOptions,
     ActionScrollOptions,
     MovePlayerOptions,
     SendKeyOptions,
     SetTextOptions,
 )
 from gamium.actions.key_by import KeyBy
 from gamium.errors.gamium_error import GamiumError
 from gamium.locator.locator import Locator
-from gamium.gamium_service import GamiumService
 from gamium.protocol.types import Vector2, Vector3
 from gamium.utils.generics import P
 
 
 class ActionPacketTypes(Generic[P]):
     def __init__(self, param_type: int, param: P):
         self.param_type = param_type  # ActionParam
@@ -105,15 +104,15 @@
     param = AppQuitParamT()
     param.exitCode = exit_code
     param.delayMs = delay_ms
     return ActionPacketTypes(ActionParam.Actions_AppQuitParam, param)
 
 
 class ActionChain:
-    def __init__(self, service: GamiumService) -> None:
+    def __init__(self, service: IGamiumService) -> None:
         self._service = service
         self.actions: List[ActionPacketTypes] = []
 
     def __add_action(self, action: ActionPacketTypes):
         self.actions.append(action)
         return self
```

### Comparing `gamium-2.0.2/gamium/actions/key_by.py` & `gamium-2.0.3/gamium/actions/key_by.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/condition/until.py` & `gamium-2.0.3/gamium/condition/until.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/gamium_client.py` & `gamium-2.0.3/gamium/gamium_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 import functools
 import json
+import time
 from typing import Any, List, Optional
 from gamium.condition.wait_condition import WaitCondition
 from gamium.options.wait_options import WaitOptions
+from gamium.protocol.generated.Types import ErrorCode
 from gamium.utils.generics import T
 from gamium.utils.try_utils import TryResult, tryify
 from gamium.utils.wait import wait_generic
 from gamium.protocol.types import ObjectInfo, Vector2, Vector3, Vector4
 
 from gamium.options import FindObjectOptions, ExecuteRpcOptions, SendKeyOptions
 
 from gamium.igamium_client import IGamiumClient
 from gamium.locator.rpc_locator import RpcLocator
 from gamium.object.player import Player
 from gamium.ui.ui import UI
 from gamium.actions.key_by import KeyBy
 from gamium.actions.action_chain import ActionChain
-from gamium.gamium_service import *
+from gamium.igamium_service import *
 from gamium.errors.gamium_error import GamiumError
 from gamium.internal.logger import Logger
 from gamium.locator.locator import Locator
 
 
 class GamiumClient(IGamiumClient):
     def __init__(
         self,
-        host: str,
-        port: int,
-        request_timeout_ms: int = 50000,
+        service: IGamiumService,
         printable: Any = None,
     ):
         self.__internal_loger = Logger()
         if printable:
             self._logger.set_handler(printable)
-        self._service = GamiumService(host, port, request_timeout_ms, self._logger)
+        self._service = service
+
+    def is_connected(self) -> bool:
+        return self._service.is_connected()
 
     def connect(self) -> None:
         self._logger.info("GamiumClient.connect")
         self._service.connect()
 
     def screen(self) -> QueryScreenResultT:
         self._logger.info("GamiumClient.screen")
```

### Comparing `gamium-2.0.2/gamium/igamium_client.py` & `gamium-2.0.3/gamium/igamium_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 from gamium.utils.generics import T
 
 
 # used internally to prevent circular imports
 class IGamiumClient(metaclass=ABCMeta):
     @abstractmethod
+    def is_connected(self) -> bool:
+        pass
+
+    @abstractmethod
     def find(self, locator: Locator, options: FindObjectOptions = FindObjectOptions()) -> ObjectInfo:
         pass
 
     @abstractmethod
     def finds(self, locator: Locator, options: FindObjectOptions = FindObjectOptions()) -> List[ObjectInfo]:
         pass
```

### Comparing `gamium-2.0.2/gamium/internal/logger.py` & `gamium-2.0.3/gamium/internal/logger.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/internal/size_prefixed_recv_queue.py` & `gamium-2.0.3/gamium/internal/size_prefixed_recv_queue.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/locator/rpc_by.py` & `gamium-2.0.3/gamium/locator/rpc_by.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/object/player.py` & `gamium-2.0.3/gamium/object/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Optional, Union
 
 import numpy as np
 from gamium.protocol.generated.Types.Vector3 import Vector3T
 from gamium.protocol.types import ObjectInfo, Vector3
 from gamium.actions.action_chain import create_move_player
 from gamium.igamium_client import IGamiumClient
-from gamium.gamium_service import GamiumService
+from gamium.igamium_service import IGamiumService
 from gamium.internal.logger import Logger
 from gamium.locator.by import By
 from gamium.locator.locator import Locator
 from gamium.options.move_player_options import MovePlayerOptions
 
 
 class Player:
     def __init__(
         self,
         client: IGamiumClient,
-        service: GamiumService,
+        service: IGamiumService,
         info: ObjectInfo,
     ) -> None:
         self._client = client
         self._service = service
         self.info = info
 
     def move(
```

### Comparing `gamium-2.0.2/gamium/object/ui_element.py` & `gamium-2.0.3/gamium/object/ui_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 from typing import Optional, Union
 from gamium.condition.until import Until
 from gamium.condition.condition import Condition
 from gamium.options.action_drag_options import ActionDragOptions
 from gamium.protocol.types import ObjectInfo, Vector2
 
 from gamium.igamium_client import IGamiumClient
-from gamium.gamium_service import (
-    GamiumService,
+from gamium.igamium_service import (
+    IGamiumService,
     create_query_object_interactable,
 )
 from gamium.internal.logger import Logger
 from gamium.locator.by import By
 from gamium.options.action_click_options import ActionClickOptions
 from gamium.options.action_scroll_options import ActionScrollOptions
 from gamium.options.query_object_interactable_options import (
     QueryObjectInteractableOptions,
 )
 from gamium.options.set_text_options import SetTextOptions
 from gamium.utils.try_utils import TryResult, tryify
 
 
 class UIElement:
-    def __init__(self, client: IGamiumClient, service: GamiumService, info: ObjectInfo):
+    def __init__(self, client: IGamiumClient, service: IGamiumService, info: ObjectInfo):
         self._client = client
         self._service = service
         self.info = info
 
     def click(self, options: ActionClickOptions = ActionClickOptions()) -> None:
         self._client._logger.info(f"UIElement({self.info.path}).click")
         self.refresh()
```

### Comparing `gamium-2.0.2/gamium/protocol/functions.py` & `gamium-2.0.3/gamium/protocol/functions.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/ActionParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/ActionParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/ActionParamSingle.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/ActionParamSingle.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/ActionResult.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/ActionResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/Actions/AppQuitParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/Actions/AppQuitParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/Actions/InputKeyParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/Actions/InputKeyParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/Actions/InputMouseParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/Actions/InputMouseParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/Actions/InputSetTextParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/Actions/InputSetTextParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/Actions/MovePlayerParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/Actions/MovePlayerParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/Actions/SleepParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/Actions/SleepParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/ActionsParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/ActionsParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/ActionsResult.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/ActionsResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/ChangeConfigurationParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/ChangeConfigurationParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/ChangeConfigurationResult.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/ChangeConfigurationResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/DumpObjectsHierarchyParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/DumpObjectsHierarchyParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/DumpObjectsHierarchyResult.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/DumpObjectsHierarchyResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/Env.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/Env.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/ExecuteRpcParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/ExecuteRpcParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/ExecuteRpcResult.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/ExecuteRpcResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/FindObjectsParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/FindObjectsParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/FindObjectsResult.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/FindObjectsResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/GetPageSourceParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/GetPageSourceParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/GetPageSourceResult.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/GetPageSourceResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/HelloParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/HelloParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/HelloResult.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/HelloResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/InspectObjectOnScreenParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectOnScreenParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/InspectObjectOnScreenResult.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectOnScreenResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/InspectObjectWithIdParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectWithIdParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/InspectObjectWithIdResult.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectWithIdResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/QueryObjectInteractableParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/QueryObjectInteractableParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/QueryObjectInteractableResult.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/QueryObjectInteractableResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/QueryProfileParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/QueryProfileParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/QueryProfileResult.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/QueryProfileResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/QueryScreenParam.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/QueryScreenParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Packets/QueryScreenResult.py` & `gamium-2.0.3/gamium/protocol/generated/Packets/QueryScreenResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Param.py` & `gamium-2.0.3/gamium/protocol/generated/Param.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Request.py` & `gamium-2.0.3/gamium/protocol/generated/Request.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Response.py` & `gamium-2.0.3/gamium/protocol/generated/Response.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Result.py` & `gamium-2.0.3/gamium/protocol/generated/Result.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Types/Configuration.py` & `gamium-2.0.3/gamium/protocol/generated/Types/Configuration.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Types/ErrorCode.py` & `gamium-2.0.3/gamium/protocol/generated/Types/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Types/ErrorResult.py` & `gamium-2.0.3/gamium/protocol/generated/Types/ErrorResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Types/ObjectHierarchyNode.py` & `gamium-2.0.3/gamium/protocol/generated/Types/ObjectHierarchyNode.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Types/ObjectInfo.py` & `gamium-2.0.3/gamium/protocol/generated/Types/ObjectInfo.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Types/ObjectLocator.py` & `gamium-2.0.3/gamium/protocol/generated/Types/ObjectLocator.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Types/ObjectsHierarchy.py` & `gamium-2.0.3/gamium/protocol/generated/Types/ObjectsHierarchy.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Types/Unity/UnityKeyCode.py` & `gamium-2.0.3/gamium/protocol/generated/Types/Unity/UnityKeyCode.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Types/Unity/UnityKeyboard.py` & `gamium-2.0.3/gamium/protocol/generated/Types/Unity/UnityKeyboard.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Types/Vector2.py` & `gamium-2.0.3/gamium/protocol/generated/Types/Vector2.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Types/Vector3.py` & `gamium-2.0.3/gamium/protocol/generated/Types/Vector3.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/generated/Types/Vector4.py` & `gamium-2.0.3/gamium/protocol/generated/Types/Vector4.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/protocol/types.py` & `gamium-2.0.3/gamium/protocol/types.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/ui/ui.py` & `gamium-2.0.3/gamium/ui/ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from gamium.condition.until import Until
 from gamium.object.ui_element import UIElement
 from gamium.options.action_click_options import ActionClickOptions
 from gamium.options.action_drag_options import ActionDragOptions
 from gamium.options.action_scroll_options import ActionScrollOptions
 from gamium.protocol.types import ObjectInfo, Vector2
 from gamium.igamium_client import IGamiumClient
-from gamium.gamium_service import GamiumService
+from gamium.igamium_service import IGamiumService
 from gamium.internal.logger import Logger
 from gamium.locator.locator import Locator
 from gamium.options.find_objects_options import FindObjectOptions
 from gamium.utils.try_utils import TryResult, tryify
 
 
 class UI:
-    def __init__(self, client: IGamiumClient, service: GamiumService):
+    def __init__(self, client: IGamiumClient, service: IGamiumService):
         self._client = client
         self._service = service
 
     def find(self, locator: Locator, options: FindObjectOptions = FindObjectOptions()) -> UIElement:
         info = self._client.wait(Until.object_located(locator, options))
         return UIElement(self._client, self._service, info)
```

### Comparing `gamium-2.0.2/gamium/utils/try_utils.py` & `gamium-2.0.3/gamium/utils/try_utils.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.2/gamium/utils/wait.py` & `gamium-2.0.3/gamium/utils/wait.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 from gamium.igamium_client import IGamiumClient
 from gamium.options.wait_options import WaitOptions
 from gamium.utils.generics import T
 from gamium.utils.time import current_time_ms
 
 
 def wait_generic(client: IGamiumClient, condition: WaitCondition[T], options: WaitOptions) -> T:
+    if client.is_connected() == False:
+        raise GamiumError(ErrorCode.Disconnected, "Not connected")
+
     def call_condition(condition: WaitCondition[T]):
         if callable(condition):
             signature = inspect.signature(condition)
             parameter_count = len(signature.parameters)
             if parameter_count > 0:
                 return condition(client)  # type: ignore # no way to let mypy know that this has parameter
             else:
```

### Comparing `gamium-2.0.2/PKG-INFO` & `gamium-2.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: gamium
-Version: 2.0.2
+Version: 2.0.3
 Summary: 
 Author: dogu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: flatbuffers (==22.10.26)
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
+Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Description-Content-Type: text/markdown
 
 # gamium client - python
 
 <p align="center">
 <img src="https://s3.ap-northeast-2.amazonaws.com/public.dogutech.io/dogu/gamium/dogu-gamium-logo.png" width="100px" height="100px" title="Gamium_Logo"/>
 </p>
```

