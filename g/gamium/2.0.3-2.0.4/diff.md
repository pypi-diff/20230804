# Comparing `tmp/gamium-2.0.3.tar.gz` & `tmp/gamium-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamium-2.0.3.tar", max compression
+gzip compressed data, was "gamium-2.0.4.tar", max compression
```

## Comparing `gamium-2.0.3.tar` & `gamium-2.0.4.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     1007 2023-05-30 02:56:42.090478 gamium-2.0.3/README.md
--rw-r--r--   0        0        0      713 2023-08-04 09:39:16.231374 gamium-2.0.3/gamium/__init__.py
--rw-r--r--   0        0        0      596 2023-08-04 09:39:16.231715 gamium-2.0.3/gamium/__main__.py
--rw-r--r--   0        0        0    11199 2023-08-04 09:39:16.232022 gamium-2.0.3/gamium/actions/action_chain.py
--rw-r--r--   0        0        0     1449 2023-05-30 02:56:42.104757 gamium-2.0.3/gamium/actions/key_by.py
--rw-r--r--   0        0        0      471 2023-05-30 02:56:42.105088 gamium-2.0.3/gamium/condition/condition.py
--rw-r--r--   0        0        0     2138 2023-05-30 02:56:42.105471 gamium-2.0.3/gamium/condition/until.py
--rw-r--r--   0        0        0      245 2023-05-30 02:56:42.105619 gamium-2.0.3/gamium/condition/wait_condition.py
--rw-r--r--   0        0        0      269 2023-05-30 02:56:42.106207 gamium-2.0.3/gamium/errors/gamium_error.py
--rw-r--r--   0        0        0     6353 2023-08-04 09:39:16.232308 gamium-2.0.3/gamium/gamium_client.py
--rw-r--r--   0        0        0     1318 2023-08-04 09:39:16.232628 gamium-2.0.3/gamium/igamium_client.py
--rw-r--r--   0        0        0     4137 2023-08-04 09:39:16.233063 gamium-2.0.3/gamium/igamium_service.py
--rw-r--r--   0        0        0       62 2023-05-30 02:56:42.107518 gamium-2.0.3/gamium/internal/__init__.py
--rw-r--r--   0        0        0     1147 2023-05-30 02:56:42.107769 gamium-2.0.3/gamium/internal/logger.py
--rw-r--r--   0        0        0      672 2023-05-30 02:56:42.108057 gamium-2.0.3/gamium/internal/size_prefixed_recv_queue.py
--rw-r--r--   0        0        0      349 2023-05-30 02:56:42.108210 gamium-2.0.3/gamium/locator/by.py
--rw-r--r--   0        0        0       59 2023-05-30 02:56:42.108434 gamium-2.0.3/gamium/locator/locator.py
--rw-r--r--   0        0        0      906 2023-05-30 02:56:42.108572 gamium-2.0.3/gamium/locator/rpc_by.py
--rw-r--r--   0        0        0       47 2023-05-30 02:56:42.108962 gamium-2.0.3/gamium/locator/rpc_locator.py
--rw-r--r--   0        0        0     1999 2023-08-04 09:39:16.233306 gamium-2.0.3/gamium/object/player.py
--rw-r--r--   0        0        0     3928 2023-08-04 09:39:16.233538 gamium-2.0.3/gamium/object/ui_element.py
--rw-r--r--   0        0        0      390 2023-05-30 02:56:42.109820 gamium-2.0.3/gamium/options/__init__.py
--rw-r--r--   0        0        0      142 2023-05-30 02:56:42.109956 gamium-2.0.3/gamium/options/action_click_options.py
--rw-r--r--   0        0        0      204 2023-05-30 02:56:42.110102 gamium-2.0.3/gamium/options/action_drag_options.py
--rw-r--r--   0        0        0       92 2023-05-30 02:56:42.110492 gamium-2.0.3/gamium/options/action_move_options.py
--rw-r--r--   0        0        0      144 2023-05-30 02:56:42.110628 gamium-2.0.3/gamium/options/action_scroll_options.py
--rw-r--r--   0        0        0      171 2023-05-30 02:56:42.110847 gamium-2.0.3/gamium/options/execute_rpc_options.py
--rw-r--r--   0        0        0      132 2023-05-30 02:56:42.111002 gamium-2.0.3/gamium/options/find_objects_options.py
--rw-r--r--   0        0        0      374 2023-05-30 02:56:42.111161 gamium-2.0.3/gamium/options/move_player_options.py
--rw-r--r--   0        0        0      262 2023-05-30 02:56:42.111311 gamium-2.0.3/gamium/options/query_object_interactable_options.py
--rw-r--r--   0        0        0      139 2023-05-30 02:56:42.111458 gamium-2.0.3/gamium/options/send_key_options.py
--rw-r--r--   0        0        0       89 2023-05-30 02:56:42.111703 gamium-2.0.3/gamium/options/set_text_options.py
--rw-r--r--   0        0        0      362 2023-05-30 02:56:42.111866 gamium-2.0.3/gamium/options/wait_options.py
--rw-r--r--   0        0        0        0 2023-06-23 03:07:41.040745 gamium-2.0.3/gamium/protocol/__init__.py
--rw-r--r--   0        0        0      597 2023-06-23 03:07:41.041613 gamium-2.0.3/gamium/protocol/functions.py
--rw-r--r--   0        0        0     1988 2023-06-23 03:07:41.042200 gamium-2.0.3/gamium/protocol/generated/Packets/ActionParam.py
--rw-r--r--   0        0        0     4353 2023-06-23 03:07:41.042754 gamium-2.0.3/gamium/protocol/generated/Packets/ActionParamSingle.py
--rw-r--r--   0        0        0     2917 2023-06-23 03:07:41.043015 gamium-2.0.3/gamium/protocol/generated/Packets/ActionResult.py
--rw-r--r--   0        0        0     2909 2023-06-23 03:07:41.043554 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/AppQuitParam.py
--rw-r--r--   0        0        0     4175 2023-06-23 03:07:41.043877 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/InputKeyParam.py
--rw-r--r--   0        0        0     5031 2023-06-23 03:07:41.044026 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/InputMouseParam.py
--rw-r--r--   0        0        0     3357 2023-06-23 03:07:41.044299 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/InputSetTextParam.py
--rw-r--r--   0        0        0      156 2023-06-23 03:07:41.044529 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/MovePlayerBy.py
--rw-r--r--   0        0        0     6404 2023-06-23 03:07:41.044671 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/MovePlayerParam.py
--rw-r--r--   0        0        0     2213 2023-06-23 03:07:41.044813 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/SleepParam.py
--rw-r--r--   0        0        0        0 2023-06-23 03:07:41.044841 gamium-2.0.3/gamium/protocol/generated/Packets/Actions/__init__.py
--rw-r--r--   0        0        0     3665 2023-06-23 03:07:41.045196 gamium-2.0.3/gamium/protocol/generated/Packets/ActionsParam.py
--rw-r--r--   0        0        0     4251 2023-06-23 03:07:41.045364 gamium-2.0.3/gamium/protocol/generated/Packets/ActionsResult.py
--rw-r--r--   0        0        0     3323 2023-06-23 03:07:41.045522 gamium-2.0.3/gamium/protocol/generated/Packets/ChangeConfigurationParam.py
--rw-r--r--   0        0        0     2116 2023-06-23 03:07:41.045666 gamium-2.0.3/gamium/protocol/generated/Packets/ChangeConfigurationResult.py
--rw-r--r--   0        0        0     3503 2023-06-23 03:07:41.045816 gamium-2.0.3/gamium/protocol/generated/Packets/DumpObjectsHierarchyParam.py
--rw-r--r--   0        0        0     4913 2023-06-23 03:07:41.045974 gamium-2.0.3/gamium/protocol/generated/Packets/DumpObjectsHierarchyResult.py
--rw-r--r--   0        0        0     2799 2023-06-23 03:07:41.046117 gamium-2.0.3/gamium/protocol/generated/Packets/Env.py
--rw-r--r--   0        0        0     6064 2023-06-23 03:07:41.046266 gamium-2.0.3/gamium/protocol/generated/Packets/ExecuteRpcParam.py
--rw-r--r--   0        0        0     2634 2023-06-23 03:07:41.046442 gamium-2.0.3/gamium/protocol/generated/Packets/ExecuteRpcResult.py
--rw-r--r--   0        0        0     3093 2023-06-23 03:07:41.046596 gamium-2.0.3/gamium/protocol/generated/Packets/FindObjectsParam.py
--rw-r--r--   0        0        0     4307 2023-06-23 03:07:41.046746 gamium-2.0.3/gamium/protocol/generated/Packets/FindObjectsResult.py
--rw-r--r--   0        0        0     1941 2023-06-23 03:07:41.046830 gamium-2.0.3/gamium/protocol/generated/Packets/GetPageSourceParam.py
--rw-r--r--   0        0        0     2758 2023-06-23 03:07:41.046890 gamium-2.0.3/gamium/protocol/generated/Packets/GetPageSourceResult.py
--rw-r--r--   0        0        0     2437 2023-06-23 03:07:41.047254 gamium-2.0.3/gamium/protocol/generated/Packets/HelloParam.py
--rw-r--r--   0        0        0     8271 2023-06-23 03:07:41.047529 gamium-2.0.3/gamium/protocol/generated/Packets/HelloResult.py
--rw-r--r--   0        0        0     4330 2023-06-23 03:07:41.047684 gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectOnScreenParam.py
--rw-r--r--   0        0        0     5826 2023-06-23 03:07:41.047851 gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectOnScreenResult.py
--rw-r--r--   0        0        0     2874 2023-06-23 03:07:41.047995 gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectWithIdParam.py
--rw-r--r--   0        0        0     3294 2023-06-23 03:07:41.048137 gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectWithIdResult.py
--rw-r--r--   0        0        0     4413 2023-06-23 03:07:41.048299 gamium-2.0.3/gamium/protocol/generated/Packets/QueryObjectInteractableParam.py
--rw-r--r--   0        0        0     2950 2023-06-23 03:07:41.048497 gamium-2.0.3/gamium/protocol/generated/Packets/QueryObjectInteractableResult.py
--rw-r--r--   0        0        0     1916 2023-06-23 03:07:41.048656 gamium-2.0.3/gamium/protocol/generated/Packets/QueryProfileParam.py
--rw-r--r--   0        0        0     2466 2023-06-23 03:07:41.048807 gamium-2.0.3/gamium/protocol/generated/Packets/QueryProfileResult.py
--rw-r--r--   0        0        0     1891 2023-06-23 03:07:41.049179 gamium-2.0.3/gamium/protocol/generated/Packets/QueryScreenParam.py
--rw-r--r--   0        0        0     3030 2023-06-23 03:07:41.049456 gamium-2.0.3/gamium/protocol/generated/Packets/QueryScreenResult.py
--rw-r--r--   0        0        0        0 2023-06-23 03:07:41.049572 gamium-2.0.3/gamium/protocol/generated/Packets/__init__.py
--rw-r--r--   0        0        0     3752 2023-06-23 03:07:41.049804 gamium-2.0.3/gamium/protocol/generated/Param.py
--rw-r--r--   0        0        0     5254 2023-06-23 03:07:41.049965 gamium-2.0.3/gamium/protocol/generated/Request.py
--rw-r--r--   0        0        0     6436 2023-06-23 03:07:41.050115 gamium-2.0.3/gamium/protocol/generated/Response.py
--rw-r--r--   0        0        0     3826 2023-06-23 03:07:41.050191 gamium-2.0.3/gamium/protocol/generated/Result.py
--rw-r--r--   0        0        0     3222 2023-06-23 03:07:41.050385 gamium-2.0.3/gamium/protocol/generated/Types/Configuration.py
--rw-r--r--   0        0        0     1146 2023-06-23 03:07:41.050762 gamium-2.0.3/gamium/protocol/generated/Types/ErrorCode.py
--rw-r--r--   0        0        0     2962 2023-06-23 03:07:41.051307 gamium-2.0.3/gamium/protocol/generated/Types/ErrorResult.py
--rw-r--r--   0        0        0      164 2023-06-23 03:07:41.051617 gamium-2.0.3/gamium/protocol/generated/Types/ExecuteRpcBy.py
--rw-r--r--   0        0        0      161 2023-06-23 03:07:41.051819 gamium-2.0.3/gamium/protocol/generated/Types/InputKeyBy.py
--rw-r--r--   0        0        0      147 2023-06-23 03:07:41.052031 gamium-2.0.3/gamium/protocol/generated/Types/InputKeyPressType.py
--rw-r--r--   0        0        0      168 2023-06-23 03:07:41.052276 gamium-2.0.3/gamium/protocol/generated/Types/InputMouseButtonCode.py
--rw-r--r--   0        0        0      177 2023-06-23 03:07:41.052478 gamium-2.0.3/gamium/protocol/generated/Types/InputMousePressType.py
--rw-r--r--   0        0        0     5920 2023-06-23 03:07:41.052652 gamium-2.0.3/gamium/protocol/generated/Types/ObjectHierarchyNode.py
--rw-r--r--   0        0        0    10803 2023-06-23 03:07:41.052832 gamium-2.0.3/gamium/protocol/generated/Types/ObjectInfo.py
--rw-r--r--   0        0        0     2955 2023-06-23 03:07:41.052991 gamium-2.0.3/gamium/protocol/generated/Types/ObjectLocator.py
--rw-r--r--   0        0        0      146 2023-06-23 03:07:41.053158 gamium-2.0.3/gamium/protocol/generated/Types/ObjectLocatorBy.py
--rw-r--r--   0        0        0      158 2023-06-23 03:07:41.053307 gamium-2.0.3/gamium/protocol/generated/Types/ObjectType.py
--rw-r--r--   0        0        0     5147 2023-06-23 03:07:41.053531 gamium-2.0.3/gamium/protocol/generated/Types/ObjectsHierarchy.py
--rw-r--r--   0        0        0     7471 2023-06-23 03:07:41.053768 gamium-2.0.3/gamium/protocol/generated/Types/Unity/UnityKeyCode.py
--rw-r--r--   0        0        0     1944 2023-06-23 03:07:41.053911 gamium-2.0.3/gamium/protocol/generated/Types/Unity/UnityKeyboard.py
--rw-r--r--   0        0        0        0 2023-06-23 03:07:41.053939 gamium-2.0.3/gamium/protocol/generated/Types/Unity/__init__.py
--rw-r--r--   0        0        0     1681 2023-06-23 03:07:41.054089 gamium-2.0.3/gamium/protocol/generated/Types/Vector2.py
--rw-r--r--   0        0        0     1947 2023-06-23 03:07:41.054251 gamium-2.0.3/gamium/protocol/generated/Types/Vector3.py
--rw-r--r--   0        0        0     2212 2023-06-23 03:07:41.054419 gamium-2.0.3/gamium/protocol/generated/Types/Vector4.py
--rw-r--r--   0        0        0        0 2023-06-23 03:07:41.054453 gamium-2.0.3/gamium/protocol/generated/Types/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 03:07:41.054512 gamium-2.0.3/gamium/protocol/generated/__init__.py
--rw-r--r--   0        0        0     3296 2023-06-23 03:07:41.055005 gamium-2.0.3/gamium/protocol/types.py
--rw-r--r--   0        0        0     4664 2023-08-04 09:39:16.233895 gamium-2.0.3/gamium/tcp_gamium_service.py
--rw-r--r--   0        0        0     3890 2023-08-04 09:39:16.234228 gamium-2.0.3/gamium/ui/ui.py
--rw-r--r--   0        0        0      500 2023-08-04 09:39:16.234412 gamium-2.0.3/gamium/utils/bytes.py
--rw-r--r--   0        0        0       80 2023-05-30 02:56:42.112384 gamium-2.0.3/gamium/utils/generics.py
--rw-r--r--   0        0        0       79 2023-05-30 02:56:42.112716 gamium-2.0.3/gamium/utils/time.py
--rw-r--r--   0        0        0      598 2023-05-30 02:56:42.112859 gamium-2.0.3/gamium/utils/try_utils.py
--rw-r--r--   0        0        0     1980 2023-08-04 09:39:16.234617 gamium-2.0.3/gamium/utils/wait.py
--rw-r--r--   0        0        0     4765 2023-08-04 09:39:16.235087 gamium-2.0.3/gamium/websocket_gamium_service.py
--rw-r--r--   0        0        0      301 2023-08-04 09:44:15.776277 gamium-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 gamium-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1007 2023-05-30 02:56:42.090478 gamium-2.0.4/README.md
+-rw-r--r--   0        0        0      713 2023-08-04 09:39:16.231374 gamium-2.0.4/gamium/__init__.py
+-rw-r--r--   0        0        0      596 2023-08-04 09:39:16.231715 gamium-2.0.4/gamium/__main__.py
+-rw-r--r--   0        0        0    11199 2023-08-04 09:39:16.232022 gamium-2.0.4/gamium/actions/action_chain.py
+-rw-r--r--   0        0        0     1449 2023-05-30 02:56:42.104757 gamium-2.0.4/gamium/actions/key_by.py
+-rw-r--r--   0        0        0      471 2023-05-30 02:56:42.105088 gamium-2.0.4/gamium/condition/condition.py
+-rw-r--r--   0        0        0     2138 2023-05-30 02:56:42.105471 gamium-2.0.4/gamium/condition/until.py
+-rw-r--r--   0        0        0      245 2023-05-30 02:56:42.105619 gamium-2.0.4/gamium/condition/wait_condition.py
+-rw-r--r--   0        0        0      269 2023-05-30 02:56:42.106207 gamium-2.0.4/gamium/errors/gamium_error.py
+-rw-r--r--   0        0        0     6353 2023-08-04 09:39:16.232308 gamium-2.0.4/gamium/gamium_client.py
+-rw-r--r--   0        0        0     1318 2023-08-04 09:39:16.232628 gamium-2.0.4/gamium/igamium_client.py
+-rw-r--r--   0        0        0     4137 2023-08-04 09:39:16.233063 gamium-2.0.4/gamium/igamium_service.py
+-rw-r--r--   0        0        0       62 2023-05-30 02:56:42.107518 gamium-2.0.4/gamium/internal/__init__.py
+-rw-r--r--   0        0        0     1147 2023-05-30 02:56:42.107769 gamium-2.0.4/gamium/internal/logger.py
+-rw-r--r--   0        0        0      672 2023-05-30 02:56:42.108057 gamium-2.0.4/gamium/internal/size_prefixed_recv_queue.py
+-rw-r--r--   0        0        0      349 2023-05-30 02:56:42.108210 gamium-2.0.4/gamium/locator/by.py
+-rw-r--r--   0        0        0       59 2023-05-30 02:56:42.108434 gamium-2.0.4/gamium/locator/locator.py
+-rw-r--r--   0        0        0      906 2023-05-30 02:56:42.108572 gamium-2.0.4/gamium/locator/rpc_by.py
+-rw-r--r--   0        0        0       47 2023-05-30 02:56:42.108962 gamium-2.0.4/gamium/locator/rpc_locator.py
+-rw-r--r--   0        0        0     1999 2023-08-04 09:39:16.233306 gamium-2.0.4/gamium/object/player.py
+-rw-r--r--   0        0        0     3928 2023-08-04 09:39:16.233538 gamium-2.0.4/gamium/object/ui_element.py
+-rw-r--r--   0        0        0      390 2023-05-30 02:56:42.109820 gamium-2.0.4/gamium/options/__init__.py
+-rw-r--r--   0        0        0      142 2023-05-30 02:56:42.109956 gamium-2.0.4/gamium/options/action_click_options.py
+-rw-r--r--   0        0        0      204 2023-05-30 02:56:42.110102 gamium-2.0.4/gamium/options/action_drag_options.py
+-rw-r--r--   0        0        0       92 2023-05-30 02:56:42.110492 gamium-2.0.4/gamium/options/action_move_options.py
+-rw-r--r--   0        0        0      144 2023-05-30 02:56:42.110628 gamium-2.0.4/gamium/options/action_scroll_options.py
+-rw-r--r--   0        0        0      171 2023-05-30 02:56:42.110847 gamium-2.0.4/gamium/options/execute_rpc_options.py
+-rw-r--r--   0        0        0      132 2023-05-30 02:56:42.111002 gamium-2.0.4/gamium/options/find_objects_options.py
+-rw-r--r--   0        0        0      374 2023-05-30 02:56:42.111161 gamium-2.0.4/gamium/options/move_player_options.py
+-rw-r--r--   0        0        0      262 2023-05-30 02:56:42.111311 gamium-2.0.4/gamium/options/query_object_interactable_options.py
+-rw-r--r--   0        0        0      139 2023-05-30 02:56:42.111458 gamium-2.0.4/gamium/options/send_key_options.py
+-rw-r--r--   0        0        0       89 2023-05-30 02:56:42.111703 gamium-2.0.4/gamium/options/set_text_options.py
+-rw-r--r--   0        0        0      362 2023-05-30 02:56:42.111866 gamium-2.0.4/gamium/options/wait_options.py
+-rw-r--r--   0        0        0        0 2023-06-23 03:07:41.040745 gamium-2.0.4/gamium/protocol/__init__.py
+-rw-r--r--   0        0        0      597 2023-06-23 03:07:41.041613 gamium-2.0.4/gamium/protocol/functions.py
+-rw-r--r--   0        0        0     1988 2023-06-23 03:07:41.042200 gamium-2.0.4/gamium/protocol/generated/Packets/ActionParam.py
+-rw-r--r--   0        0        0     4353 2023-06-23 03:07:41.042754 gamium-2.0.4/gamium/protocol/generated/Packets/ActionParamSingle.py
+-rw-r--r--   0        0        0     2917 2023-06-23 03:07:41.043015 gamium-2.0.4/gamium/protocol/generated/Packets/ActionResult.py
+-rw-r--r--   0        0        0     2909 2023-06-23 03:07:41.043554 gamium-2.0.4/gamium/protocol/generated/Packets/Actions/AppQuitParam.py
+-rw-r--r--   0        0        0     4175 2023-06-23 03:07:41.043877 gamium-2.0.4/gamium/protocol/generated/Packets/Actions/InputKeyParam.py
+-rw-r--r--   0        0        0     5031 2023-06-23 03:07:41.044026 gamium-2.0.4/gamium/protocol/generated/Packets/Actions/InputMouseParam.py
+-rw-r--r--   0        0        0     3357 2023-06-23 03:07:41.044299 gamium-2.0.4/gamium/protocol/generated/Packets/Actions/InputSetTextParam.py
+-rw-r--r--   0        0        0      156 2023-06-23 03:07:41.044529 gamium-2.0.4/gamium/protocol/generated/Packets/Actions/MovePlayerBy.py
+-rw-r--r--   0        0        0     6404 2023-06-23 03:07:41.044671 gamium-2.0.4/gamium/protocol/generated/Packets/Actions/MovePlayerParam.py
+-rw-r--r--   0        0        0     2213 2023-06-23 03:07:41.044813 gamium-2.0.4/gamium/protocol/generated/Packets/Actions/SleepParam.py
+-rw-r--r--   0        0        0        0 2023-06-23 03:07:41.044841 gamium-2.0.4/gamium/protocol/generated/Packets/Actions/__init__.py
+-rw-r--r--   0        0        0     3665 2023-06-23 03:07:41.045196 gamium-2.0.4/gamium/protocol/generated/Packets/ActionsParam.py
+-rw-r--r--   0        0        0     4251 2023-06-23 03:07:41.045364 gamium-2.0.4/gamium/protocol/generated/Packets/ActionsResult.py
+-rw-r--r--   0        0        0     3323 2023-06-23 03:07:41.045522 gamium-2.0.4/gamium/protocol/generated/Packets/ChangeConfigurationParam.py
+-rw-r--r--   0        0        0     2116 2023-06-23 03:07:41.045666 gamium-2.0.4/gamium/protocol/generated/Packets/ChangeConfigurationResult.py
+-rw-r--r--   0        0        0     3503 2023-06-23 03:07:41.045816 gamium-2.0.4/gamium/protocol/generated/Packets/DumpObjectsHierarchyParam.py
+-rw-r--r--   0        0        0     4913 2023-06-23 03:07:41.045974 gamium-2.0.4/gamium/protocol/generated/Packets/DumpObjectsHierarchyResult.py
+-rw-r--r--   0        0        0     2799 2023-06-23 03:07:41.046117 gamium-2.0.4/gamium/protocol/generated/Packets/Env.py
+-rw-r--r--   0        0        0     6064 2023-06-23 03:07:41.046266 gamium-2.0.4/gamium/protocol/generated/Packets/ExecuteRpcParam.py
+-rw-r--r--   0        0        0     2634 2023-06-23 03:07:41.046442 gamium-2.0.4/gamium/protocol/generated/Packets/ExecuteRpcResult.py
+-rw-r--r--   0        0        0     3093 2023-06-23 03:07:41.046596 gamium-2.0.4/gamium/protocol/generated/Packets/FindObjectsParam.py
+-rw-r--r--   0        0        0     4307 2023-06-23 03:07:41.046746 gamium-2.0.4/gamium/protocol/generated/Packets/FindObjectsResult.py
+-rw-r--r--   0        0        0     1941 2023-06-23 03:07:41.046830 gamium-2.0.4/gamium/protocol/generated/Packets/GetPageSourceParam.py
+-rw-r--r--   0        0        0     2758 2023-06-23 03:07:41.046890 gamium-2.0.4/gamium/protocol/generated/Packets/GetPageSourceResult.py
+-rw-r--r--   0        0        0     2437 2023-06-23 03:07:41.047254 gamium-2.0.4/gamium/protocol/generated/Packets/HelloParam.py
+-rw-r--r--   0        0        0     8271 2023-06-23 03:07:41.047529 gamium-2.0.4/gamium/protocol/generated/Packets/HelloResult.py
+-rw-r--r--   0        0        0     4330 2023-06-23 03:07:41.047684 gamium-2.0.4/gamium/protocol/generated/Packets/InspectObjectOnScreenParam.py
+-rw-r--r--   0        0        0     5826 2023-06-23 03:07:41.047851 gamium-2.0.4/gamium/protocol/generated/Packets/InspectObjectOnScreenResult.py
+-rw-r--r--   0        0        0     2874 2023-06-23 03:07:41.047995 gamium-2.0.4/gamium/protocol/generated/Packets/InspectObjectWithIdParam.py
+-rw-r--r--   0        0        0     3294 2023-06-23 03:07:41.048137 gamium-2.0.4/gamium/protocol/generated/Packets/InspectObjectWithIdResult.py
+-rw-r--r--   0        0        0     4413 2023-06-23 03:07:41.048299 gamium-2.0.4/gamium/protocol/generated/Packets/QueryObjectInteractableParam.py
+-rw-r--r--   0        0        0     2950 2023-06-23 03:07:41.048497 gamium-2.0.4/gamium/protocol/generated/Packets/QueryObjectInteractableResult.py
+-rw-r--r--   0        0        0     1916 2023-06-23 03:07:41.048656 gamium-2.0.4/gamium/protocol/generated/Packets/QueryProfileParam.py
+-rw-r--r--   0        0        0     2466 2023-06-23 03:07:41.048807 gamium-2.0.4/gamium/protocol/generated/Packets/QueryProfileResult.py
+-rw-r--r--   0        0        0     1891 2023-06-23 03:07:41.049179 gamium-2.0.4/gamium/protocol/generated/Packets/QueryScreenParam.py
+-rw-r--r--   0        0        0     3030 2023-06-23 03:07:41.049456 gamium-2.0.4/gamium/protocol/generated/Packets/QueryScreenResult.py
+-rw-r--r--   0        0        0        0 2023-06-23 03:07:41.049572 gamium-2.0.4/gamium/protocol/generated/Packets/__init__.py
+-rw-r--r--   0        0        0     3752 2023-06-23 03:07:41.049804 gamium-2.0.4/gamium/protocol/generated/Param.py
+-rw-r--r--   0        0        0     5254 2023-06-23 03:07:41.049965 gamium-2.0.4/gamium/protocol/generated/Request.py
+-rw-r--r--   0        0        0     6436 2023-06-23 03:07:41.050115 gamium-2.0.4/gamium/protocol/generated/Response.py
+-rw-r--r--   0        0        0     3826 2023-06-23 03:07:41.050191 gamium-2.0.4/gamium/protocol/generated/Result.py
+-rw-r--r--   0        0        0     3222 2023-06-23 03:07:41.050385 gamium-2.0.4/gamium/protocol/generated/Types/Configuration.py
+-rw-r--r--   0        0        0     1146 2023-06-23 03:07:41.050762 gamium-2.0.4/gamium/protocol/generated/Types/ErrorCode.py
+-rw-r--r--   0        0        0     2962 2023-06-23 03:07:41.051307 gamium-2.0.4/gamium/protocol/generated/Types/ErrorResult.py
+-rw-r--r--   0        0        0      164 2023-06-23 03:07:41.051617 gamium-2.0.4/gamium/protocol/generated/Types/ExecuteRpcBy.py
+-rw-r--r--   0        0        0      161 2023-06-23 03:07:41.051819 gamium-2.0.4/gamium/protocol/generated/Types/InputKeyBy.py
+-rw-r--r--   0        0        0      147 2023-06-23 03:07:41.052031 gamium-2.0.4/gamium/protocol/generated/Types/InputKeyPressType.py
+-rw-r--r--   0        0        0      168 2023-06-23 03:07:41.052276 gamium-2.0.4/gamium/protocol/generated/Types/InputMouseButtonCode.py
+-rw-r--r--   0        0        0      177 2023-06-23 03:07:41.052478 gamium-2.0.4/gamium/protocol/generated/Types/InputMousePressType.py
+-rw-r--r--   0        0        0     5920 2023-06-23 03:07:41.052652 gamium-2.0.4/gamium/protocol/generated/Types/ObjectHierarchyNode.py
+-rw-r--r--   0        0        0    10803 2023-06-23 03:07:41.052832 gamium-2.0.4/gamium/protocol/generated/Types/ObjectInfo.py
+-rw-r--r--   0        0        0     2955 2023-06-23 03:07:41.052991 gamium-2.0.4/gamium/protocol/generated/Types/ObjectLocator.py
+-rw-r--r--   0        0        0      146 2023-06-23 03:07:41.053158 gamium-2.0.4/gamium/protocol/generated/Types/ObjectLocatorBy.py
+-rw-r--r--   0        0        0      158 2023-06-23 03:07:41.053307 gamium-2.0.4/gamium/protocol/generated/Types/ObjectType.py
+-rw-r--r--   0        0        0     5147 2023-06-23 03:07:41.053531 gamium-2.0.4/gamium/protocol/generated/Types/ObjectsHierarchy.py
+-rw-r--r--   0        0        0     7471 2023-06-23 03:07:41.053768 gamium-2.0.4/gamium/protocol/generated/Types/Unity/UnityKeyCode.py
+-rw-r--r--   0        0        0     1944 2023-06-23 03:07:41.053911 gamium-2.0.4/gamium/protocol/generated/Types/Unity/UnityKeyboard.py
+-rw-r--r--   0        0        0        0 2023-06-23 03:07:41.053939 gamium-2.0.4/gamium/protocol/generated/Types/Unity/__init__.py
+-rw-r--r--   0        0        0     1681 2023-06-23 03:07:41.054089 gamium-2.0.4/gamium/protocol/generated/Types/Vector2.py
+-rw-r--r--   0        0        0     1947 2023-06-23 03:07:41.054251 gamium-2.0.4/gamium/protocol/generated/Types/Vector3.py
+-rw-r--r--   0        0        0     2212 2023-06-23 03:07:41.054419 gamium-2.0.4/gamium/protocol/generated/Types/Vector4.py
+-rw-r--r--   0        0        0        0 2023-06-23 03:07:41.054453 gamium-2.0.4/gamium/protocol/generated/Types/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 03:07:41.054512 gamium-2.0.4/gamium/protocol/generated/__init__.py
+-rw-r--r--   0        0        0     3296 2023-06-23 03:07:41.055005 gamium-2.0.4/gamium/protocol/types.py
+-rw-r--r--   0        0        0     4664 2023-08-04 09:39:16.233895 gamium-2.0.4/gamium/tcp_gamium_service.py
+-rw-r--r--   0        0        0     3890 2023-08-04 09:39:16.234228 gamium-2.0.4/gamium/ui/ui.py
+-rw-r--r--   0        0        0      500 2023-08-04 09:39:16.234412 gamium-2.0.4/gamium/utils/bytes.py
+-rw-r--r--   0        0        0       80 2023-05-30 02:56:42.112384 gamium-2.0.4/gamium/utils/generics.py
+-rw-r--r--   0        0        0       79 2023-05-30 02:56:42.112716 gamium-2.0.4/gamium/utils/time.py
+-rw-r--r--   0        0        0      598 2023-05-30 02:56:42.112859 gamium-2.0.4/gamium/utils/try_utils.py
+-rw-r--r--   0        0        0     1980 2023-08-04 09:39:16.234617 gamium-2.0.4/gamium/utils/wait.py
+-rw-r--r--   0        0        0     4765 2023-08-04 09:39:16.235087 gamium-2.0.4/gamium/websocket_gamium_service.py
+-rw-r--r--   0        0        0      301 2023-08-04 10:14:55.457893 gamium-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 gamium-2.0.4/PKG-INFO
```

### Comparing `gamium-2.0.3/README.md` & `gamium-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/__init__.py` & `gamium-2.0.4/gamium/__init__.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/__main__.py` & `gamium-2.0.4/gamium/__main__.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/actions/action_chain.py` & `gamium-2.0.4/gamium/actions/action_chain.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/actions/key_by.py` & `gamium-2.0.4/gamium/actions/key_by.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/condition/until.py` & `gamium-2.0.4/gamium/condition/until.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/gamium_client.py` & `gamium-2.0.4/gamium/gamium_client.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/igamium_client.py` & `gamium-2.0.4/gamium/igamium_client.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/igamium_service.py` & `gamium-2.0.4/gamium/igamium_service.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/internal/logger.py` & `gamium-2.0.4/gamium/internal/logger.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/internal/size_prefixed_recv_queue.py` & `gamium-2.0.4/gamium/internal/size_prefixed_recv_queue.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/locator/rpc_by.py` & `gamium-2.0.4/gamium/locator/rpc_by.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/object/player.py` & `gamium-2.0.4/gamium/object/player.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/object/ui_element.py` & `gamium-2.0.4/gamium/object/ui_element.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/functions.py` & `gamium-2.0.4/gamium/protocol/functions.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/ActionParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/ActionParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/ActionParamSingle.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/ActionParamSingle.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/ActionResult.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/ActionResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/Actions/AppQuitParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/Actions/AppQuitParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/Actions/InputKeyParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/Actions/InputKeyParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/Actions/InputMouseParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/Actions/InputMouseParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/Actions/InputSetTextParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/Actions/InputSetTextParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/Actions/MovePlayerParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/Actions/MovePlayerParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/Actions/SleepParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/Actions/SleepParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/ActionsParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/ActionsParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/ActionsResult.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/ActionsResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/ChangeConfigurationParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/ChangeConfigurationParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/ChangeConfigurationResult.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/ChangeConfigurationResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/DumpObjectsHierarchyParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/DumpObjectsHierarchyParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/DumpObjectsHierarchyResult.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/DumpObjectsHierarchyResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/Env.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/Env.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/ExecuteRpcParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/ExecuteRpcParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/ExecuteRpcResult.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/ExecuteRpcResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/FindObjectsParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/FindObjectsParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/FindObjectsResult.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/FindObjectsResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/GetPageSourceParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/GetPageSourceParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/GetPageSourceResult.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/GetPageSourceResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/HelloParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/HelloParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/HelloResult.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/HelloResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectOnScreenParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/InspectObjectOnScreenParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectOnScreenResult.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/InspectObjectOnScreenResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectWithIdParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/InspectObjectWithIdParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/InspectObjectWithIdResult.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/InspectObjectWithIdResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/QueryObjectInteractableParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/QueryObjectInteractableParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/QueryObjectInteractableResult.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/QueryObjectInteractableResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/QueryProfileParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/QueryProfileParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/QueryProfileResult.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/QueryProfileResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/QueryScreenParam.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/QueryScreenParam.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Packets/QueryScreenResult.py` & `gamium-2.0.4/gamium/protocol/generated/Packets/QueryScreenResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Param.py` & `gamium-2.0.4/gamium/protocol/generated/Param.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Request.py` & `gamium-2.0.4/gamium/protocol/generated/Request.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Response.py` & `gamium-2.0.4/gamium/protocol/generated/Response.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Result.py` & `gamium-2.0.4/gamium/protocol/generated/Result.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Types/Configuration.py` & `gamium-2.0.4/gamium/protocol/generated/Types/Configuration.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Types/ErrorCode.py` & `gamium-2.0.4/gamium/protocol/generated/Types/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Types/ErrorResult.py` & `gamium-2.0.4/gamium/protocol/generated/Types/ErrorResult.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Types/ObjectHierarchyNode.py` & `gamium-2.0.4/gamium/protocol/generated/Types/ObjectHierarchyNode.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Types/ObjectInfo.py` & `gamium-2.0.4/gamium/protocol/generated/Types/ObjectInfo.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Types/ObjectLocator.py` & `gamium-2.0.4/gamium/protocol/generated/Types/ObjectLocator.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Types/ObjectsHierarchy.py` & `gamium-2.0.4/gamium/protocol/generated/Types/ObjectsHierarchy.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Types/Unity/UnityKeyCode.py` & `gamium-2.0.4/gamium/protocol/generated/Types/Unity/UnityKeyCode.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Types/Unity/UnityKeyboard.py` & `gamium-2.0.4/gamium/protocol/generated/Types/Unity/UnityKeyboard.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Types/Vector2.py` & `gamium-2.0.4/gamium/protocol/generated/Types/Vector2.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Types/Vector3.py` & `gamium-2.0.4/gamium/protocol/generated/Types/Vector3.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/generated/Types/Vector4.py` & `gamium-2.0.4/gamium/protocol/generated/Types/Vector4.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/protocol/types.py` & `gamium-2.0.4/gamium/protocol/types.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/tcp_gamium_service.py` & `gamium-2.0.4/gamium/tcp_gamium_service.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/ui/ui.py` & `gamium-2.0.4/gamium/ui/ui.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/utils/try_utils.py` & `gamium-2.0.4/gamium/utils/try_utils.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/utils/wait.py` & `gamium-2.0.4/gamium/utils/wait.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/gamium/websocket_gamium_service.py` & `gamium-2.0.4/gamium/websocket_gamium_service.py`

 * *Files identical despite different names*

### Comparing `gamium-2.0.3/PKG-INFO` & `gamium-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamium
-Version: 2.0.3
+Version: 2.0.4
 Summary: 
 Author: dogu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

