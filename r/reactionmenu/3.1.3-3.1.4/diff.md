# Comparing `tmp/reactionmenu-3.1.3.tar.gz` & `tmp/reactionmenu-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactionmenu-3.1.3.tar", last modified: Thu Feb  9 18:57:16 2023, max compression
+gzip compressed data, was "reactionmenu-3.1.4.tar", last modified: Fri Aug  4 15:25:33 2023, max compression
```

## Comparing `reactionmenu-3.1.3.tar` & `reactionmenu-3.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-02-09 18:57:16.618296 reactionmenu-3.1.3/
--rw-rw-rw-   0        0        0     1101 2022-01-18 02:07:36.000000 reactionmenu-3.1.3/LICENSE
--rw-rw-rw-   0        0        0    50852 2023-02-09 18:57:16.617299 reactionmenu-3.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    49457 2022-08-23 19:46:42.000000 reactionmenu-3.1.3/README.md
--rw-rw-rw-   0        0        0     1828 2023-02-07 12:29:58.000000 reactionmenu-3.1.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-02-09 18:57:16.608264 reactionmenu-3.1.3/reactionmenu/
--rw-rw-rw-   0        0        0      621 2023-01-09 04:12:38.000000 reactionmenu-3.1.3/reactionmenu/__init__.py
--rw-rw-rw-   0        0        0    63206 2023-02-07 12:11:29.000000 reactionmenu-3.1.3/reactionmenu/abc.py
--rw-rw-rw-   0        0        0    23136 2022-08-21 17:02:00.000000 reactionmenu-3.1.3/reactionmenu/buttons.py
--rw-rw-rw-   0        0        0    31472 2022-08-21 17:02:00.000000 reactionmenu-3.1.3/reactionmenu/core.py
--rw-rw-rw-   0        0        0     2365 2022-07-23 18:36:30.000000 reactionmenu-3.1.3/reactionmenu/decorators.py
--rw-rw-rw-   0        0        0     3843 2022-07-23 18:36:30.000000 reactionmenu-3.1.3/reactionmenu/errors.py
--rw-rw-rw-   0        0        0    68673 2022-08-21 17:02:00.000000 reactionmenu-3.1.3/reactionmenu/views_menu.py
-drwxrwxrwx   0        0        0        0 2023-02-09 18:57:16.615305 reactionmenu-3.1.3/reactionmenu.egg-info/
--rw-rw-rw-   0        0        0    50852 2023-02-09 18:57:16.000000 reactionmenu-3.1.3/reactionmenu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-02-09 18:57:16.000000 reactionmenu-3.1.3/reactionmenu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-09 18:57:16.000000 reactionmenu-3.1.3/reactionmenu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-02-09 18:57:16.000000 reactionmenu-3.1.3/reactionmenu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-09 18:57:16.000000 reactionmenu-3.1.3/reactionmenu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-09 18:57:16.618296 reactionmenu-3.1.3/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-01-09 02:24:50.000000 reactionmenu-3.1.3/setup.py
+drwxr-xr-x   0 jaggenneil   (501) staff       (20)        0 2023-08-04 15:25:33.955252 reactionmenu-3.1.4/
+-rw-r--r--   0 jaggenneil   (501) staff       (20)     1101 2022-08-15 22:52:56.000000 reactionmenu-3.1.4/LICENSE
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    49832 2023-08-04 15:25:33.955116 reactionmenu-3.1.4/PKG-INFO
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    49457 2022-08-23 23:34:35.000000 reactionmenu-3.1.4/README.md
+-rw-r--r--   0 jaggenneil   (501) staff       (20)     1756 2023-07-03 07:10:24.000000 reactionmenu-3.1.4/pyproject.toml
+drwxr-xr-x   0 jaggenneil   (501) staff       (20)        0 2023-08-04 15:25:33.953749 reactionmenu-3.1.4/reactionmenu/
+-rw-r--r--   0 jaggenneil   (501) staff       (20)      595 2022-08-22 01:33:06.000000 reactionmenu-3.1.4/reactionmenu/__init__.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    62302 2023-07-03 07:21:10.000000 reactionmenu-3.1.4/reactionmenu/abc.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    22469 2022-08-20 06:21:05.000000 reactionmenu-3.1.4/reactionmenu/buttons.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    30760 2022-08-20 11:05:01.000000 reactionmenu-3.1.4/reactionmenu/core.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)     2311 2022-08-15 22:52:56.000000 reactionmenu-3.1.4/reactionmenu/decorators.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)     3747 2022-08-15 22:52:56.000000 reactionmenu-3.1.4/reactionmenu/errors.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    67218 2022-08-20 11:05:10.000000 reactionmenu-3.1.4/reactionmenu/views_menu.py
+drwxr-xr-x   0 jaggenneil   (501) staff       (20)        0 2023-08-04 15:25:33.954914 reactionmenu-3.1.4/reactionmenu.egg-info/
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    49832 2023-08-04 15:25:33.000000 reactionmenu-3.1.4/reactionmenu.egg-info/PKG-INFO
+-rw-r--r--   0 jaggenneil   (501) staff       (20)      387 2023-08-04 15:25:33.000000 reactionmenu-3.1.4/reactionmenu.egg-info/SOURCES.txt
+-rw-r--r--   0 jaggenneil   (501) staff       (20)        1 2023-08-04 15:25:33.000000 reactionmenu-3.1.4/reactionmenu.egg-info/dependency_links.txt
+-rw-r--r--   0 jaggenneil   (501) staff       (20)       18 2023-08-04 15:25:33.000000 reactionmenu-3.1.4/reactionmenu.egg-info/requires.txt
+-rw-r--r--   0 jaggenneil   (501) staff       (20)       13 2023-08-04 15:25:33.000000 reactionmenu-3.1.4/reactionmenu.egg-info/top_level.txt
+-rw-r--r--   0 jaggenneil   (501) staff       (20)       38 2023-08-04 15:25:33.955295 reactionmenu-3.1.4/setup.cfg
+-rw-r--r--   0 jaggenneil   (501) staff       (20)       71 2023-06-02 14:27:33.000000 reactionmenu-3.1.4/setup.py
```

### Comparing `reactionmenu-3.1.3/LICENSE` & `reactionmenu-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `reactionmenu-3.1.3/PKG-INFO` & `reactionmenu-3.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: reactionmenu
-Version: 3.1.3
-Summary: A library to create a discord.py 2.0+ paginator. Supports pagination with buttons, reactions, and category selection using selects.
-Author: Defxult#8269
-License: MIT
-Project-URL: Homepage, https://github.com/Defxult/reactionmenu
-Project-URL: Changelog, https://github.com/Defxult/reactionmenu/blob/main/CHANGELOG.md
-Keywords: buttons,buttons paginator,buttons menu,discord,discord.py,discord.py 2.0,d.py,components,components paginator,components menu,discord components,discord components menu,discord buttons,discord buttons paginator,discord buttons menu,discord paginator,discord pagination,discord reaction menu,discord reactions,discord embed,discord menu,discord interactions,embed menu,embed reaction menu,embed paginator,interactions,interactions menu,interactions paginator,menus,paginator,pagination,pagination menu,reaction menu
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![logo](https://cdn.discordapp.com/attachments/655186216060321816/820162226316378162/discord.jpg)
 <div align="center">
 
 [![Downloads](https://pepy.tech/badge/reactionmenu)](https://pepy.tech/project/reactionmenu) 
 [![Downloads](https://pepy.tech/badge/reactionmenu/month)](https://pepy.tech/project/reactionmenu)
 [![Downloads](https://pepy.tech/badge/reactionmenu/week)](https://pepy.tech/project/reactionmenu)
```

### Comparing `reactionmenu-3.1.3/README.md` & `reactionmenu-3.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,995 +1,1015 @@
-![logo](https://cdn.discordapp.com/attachments/655186216060321816/820162226316378162/discord.jpg)
-<div align="center">
-
-[![Downloads](https://pepy.tech/badge/reactionmenu)](https://pepy.tech/project/reactionmenu) 
-[![Downloads](https://pepy.tech/badge/reactionmenu/month)](https://pepy.tech/project/reactionmenu)
-[![Downloads](https://pepy.tech/badge/reactionmenu/week)](https://pepy.tech/project/reactionmenu)
-
-![python_version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
-</div>
-
-## How to install
-You can install the latest [PyPI](https://pypi.org/project/reactionmenu/) version of the library by doing:
-```
-$ pip install reactionmenu
-```
-Or the development version:
-```
-$ pip install git+https://github.com/Defxult/reactionmenu
-```
-
-## Intents
-Minimum intents needed
-```py
-bot = commands.Bot(..., intents=discord.Intents(messages=True, guilds=True, reactions=True, members=True))
-```
----
-## ReactionMenu
-
-```
-class reactionmenu.ReactionMenu(method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs)
-```
-
-A `ReactionMenu` is a menu that uses emojis which are either custom guild emojis or a normal emoji to control the pagination process. If you're not looking for any of the fancy features and just want something simple, this is the one to use.
-
-![showcase](https://cdn.discordapp.com/attachments/655186216060321816/819885696176226314/showcase.gif)
-
-<details>
-  <summary><b>Click to show ReactionMenu documentation</b></summary>
-
-### How to import
-```py
-from reactionmenu import ReactionMenu, ReactionButton
-```
-This library comes with several methods and options in order to make a discord reaction menu simple. Once you have imported the proper classes, you will initialize the constructor like so:
-```py
-menu = ReactionMenu(method, menu_type=ReactionMenu.TypeEmbed)
-```
-
-
-### Parameters of the ReactionMenu constructor
-* `method` (`Union[discord.ext.commands.Context, discord.Interaction]`) A context or interaction object
-* `menu_type` (`MenuType`) The configuration of the menu
-  * `ReactionMenu.TypeEmbed`, a normal embed pagination menu
-  * `ReactionMenu.TypeEmbedDynamic`, an embed pagination menu with dynamic data
-  * `ReactionMenu.TypeText`, a text only pagination menu
-
-
-### Kwargs of the ReactionMenu constructor
-| Name | Type | Default Value | Used for | Info 
--------|------|---------------|----------|------
-| `wrap_in_codeblock` | `str` | `None` | `ReactionMenu.TypeEmbedDynamic` | The discord codeblock language identifier to wrap your data in. Example: `ReactionMenu(ctx, ..., wrap_in_codeblock='py')`
-| `custom_embed` | `discord.Embed` | `None` | `ReactionMenu.TypeEmbedDynamic` | Embed object to use when adding data with `ReactionMenu.add_row()`. Used for styling purposes
-| `delete_on_timeout` | `bool` | `False` | `All menu types` | Delete the menu when it times out
-| `clear_reactions_after` | `bool` | `True` | `All menu types` | delete all reactions after the menu times out
-| `navigation_speed` | `str` | `ReactionMenu.NORMAL` | `All menu types` | Sets if the user needs to wait for the reaction to be removed by the bot before "turning" the page. Setting the speed to `ReactionMenu.FAST` makes it so that there is no need to wait (reactions are not removed on each press) and can navigate lengthy menu's more quickly
-| `only_roles` | `List[discord.Role]` | `None` | `All menu types` | If set, only members with any of the given roles are allowed to control the menu. The menu owner can always control the menu
-| `timeout` | `Union[int, float, None]` | `60.0` | `All menu types` | The timer for when the menu times out. Can be `None` for no timeout
-| `show_page_director` | `bool` | `True` | `All menu types` | Shown at the bottom of each embed page. "Page 1/20"
-| `name` | `str` | `None` | `All menu types` | A name you can set for the menu
-| `style` | `str` | `"Page $/&"` | `All menu types` | A custom page director style you can select. "$" represents the current page, "&" represents the total amount of pages. Example: `ReactionMenu(ctx, ..., style='On $ out of &')`
-| `all_can_click` | `bool` | `False` | `All menu types` | Sets if everyone is allowed to control when pages are 'turned' when buttons are clicked
-| `delete_interactions` | `bool` | `True` | `All menu types` | Delete the prompt message by the bot and response message by the user when asked what page they would like to go to when using `ReactionButton.Type.GO_TO_PAGE`
-| `rows_requested` | `int` | `None` | `ReactionMenu.TypeEmbedDynamic` | The amount of information per `ReactionMenu.add_row()` you would like applied to each embed page
-| `remove_extra_emojis` | `bool` | `False` | `All menu types` | If `True`, all emojis (reactions) added to the menu message that were not originally added to the menu will be removed
----
-
-### Pages for ReactionMenu
-Depending on the `menu_type`, pages can either be a `str`, `discord.Embed`, or a combination of `content` and `files` ([example below](#stacked-pages))
-* If the `menu_type` is `ReactionMenu.TypeEmbed`, use embeds
-* If the `menu_type` is `ReactionMenu.TypeText` (text only menu) or `ReactionMenu.TypeEmbedDynamic` (embed only menu), use strings.
-* Associated methods
-  * `ReactionMenu.add_page(embed: discord.Embed=MISSING, content: Optional[str]=None, files: Optional[Sequence[discord.File]]=None)`
-  * `ReactionMenu.add_pages(pages: Sequence[Union[discord.Embed, str]])`
-  * `ReactionMenu.add_row(data: str)`
-  * `ReactionMenu.remove_all_pages()`
-  * `ReactionMenu.clear_all_row_data()`
-  * `ReactionMenu.remove_page(page_number: int)`
-  * `ReactionMenu.set_main_pages(*embeds: Embed)`
-  * `ReactionMenu.set_last_pages(*embeds: Embed)`
-
-
-#### Adding Pages
-```py
-# ReactionMenu.TypeEmbed
-menu = ReactionMenu(method, menu_type=ReactionMenu.TypeEmbed)
-menu.add_page(summer_embed)
-menu.add_page(winter_embed)
-
-# ReactionMenu.TypeText
-menu = ReactionMenu(method, menu_type=ReactionMenu.TypeText)
-menu.add_page(content='Its so hot!')
-menu.add_page(content='Its so cold!')
-```
-
-#### ReactionMenu.TypeText
-A `TypeText` menu is a text based pagination menu. No embeds are involved in the pagination process, only plain text is used.
-
-![showcase-text](https://cdn.discordapp.com/attachments/655186216060321816/929172629947027466/text_showcase.gif)
-
-#### Stacked Pages
-With `v3.1.0+`, you can paginate with more than just an embed or text. You can combine text, embeds, as well as files. But depending on the `menu_type` the combination can be restricted. Here is an example of a menu with a `menu_type` of `TypeEmbed` that is stacked.
-
-```py
-# You can use regular commands as well
-@bot.tree.command(description="These are stacked pages", guild=discord.Object(id=...))
-async def stacked(interaction: discord.Interaction):
-    menu = ReactionMenu(interaction, menu_type=ReactionMenu.TypeEmbed)
-
-    menu.add_page(discord.Embed(title="My Embed"), content="This content is stacked on top of a file", files=[discord.File("stacked.py")])
-    menu.add_page(discord.Embed(title="Hey Wumpos, can you say hi to the person reading this? 😃"))
-    menu.add_page(discord.Embed(title="Hi, I'm Wumpos!"), files=[discord.File("wumpos.gif")])
-    
-    menu.add_button(ReactionButton.back())
-    menu.add_button(ReactionButton.next())
-    
-    await menu.start()
-```
-![stacked](https://cdn.discordapp.com/attachments/655186216060321816/955966821268332554/stacked.gif)
-
-Since the `menu_type` is `TypeEmbed`, there always has to be an embed on each page. If the `menu_type` was `TypeText`, embeds aren't allowed and you will be restricted to only using the `files` parameter.
-
-#### ReactionMenu.TypeEmbedDynamic
-A dynamic menu is used when you do not know how much information will be applied to the menu. For example, if you were to request information from a database, that information can always change. You query something and you might get 1,500 results back, and the next maybe only 800. A dynamic menu pieces all this information together for you and adds it to an embed page by rows of data. `ReactionMenu.add_row()` is best used in some sort of `Iterable` where everything can be looped through, but only add the amount of data you want to the menu page.
-> **NOTE:** In a dynamic menu, all added data is placed in the description section of an embed. If you choose to use a `custom_embed`, all text in the description will be overridden with the data you add
-* Associated methods
-    * `ReactionMenu.add_row(data: str)`
-    * `ReactionMenu.clear_all_row_data()`
-    * `ReactionMenu.set_main_pages(*embeds: Embed)`
-    * `ReactionMenu.set_last_pages(*embeds: Embed)`
-* The kwargs specifically made for a dynamic menu are:
-    * `rows_requested` - The amount of rows you would like on each embed page before making a new page
-        * `ReactionMenu(..., rows_requested=5)`
-    * `custom_embed` - An embed you have created to use as the embed pages. Used for your menu aesthetic
-        * `ReactionMenu(..., custom_embed=red_embed)`
-    * `wrap_in_codeblock` - The language identifier when wrapping your data in a discord codeblock. 
-        * `ReactionMenu(..., wrap_in_codeblock='py')`
-
-##### Adding Rows/data
-```py
-menu = ReactionMenu(ctx, menu_type=ReactionMenu.TypeEmbedDynamic, rows_requested=5)
-
-for data in database.request('SELECT * FROM customers'):
-    menu.add_row(data)
-```
-##### Deleting Data
-You can remove all the data you've added to a menu by using `menu.clear_all_row_data()`
-
-##### Main/Last Pages
-When using a dynamic menu, the only embed pages you see are from the data you've added. But if you would like to show more pages other than just the data, you can use methods `ReactionMenu.set_main_pages()` and `ReactionMenu.set_last_pages()`. Setting the main page(s), the embeds you set will be the first embeds that are shown when the menu starts. Setting the last page(s) are the last embeds shown
-```py
-menu.set_main_pages(welcome_embed, announcement_embed)
-
-for data in get_information():
-    menu.add_row(data)
-
-menu.set_last_pages(additional_info_embed)
-# NOTE: setting main/last pages can be set in any order
-```
-
-### ReactionButtons and ButtonTypes
-Buttons/button types are used when you want to add a reaction to the menu that does a certain function. Buttons and button types work together to achieve the desired action.
-```
-class reactionmenu.ReactionButton(*, emoji: str, linked_to: ButtonType, **kwargs)
-```
-### Parameters of the ReactionButton constructor
-* `emoji` (`str`) The emoji you would like to use as the reaction
-* `linked_to` (`ReactionButton.Type`) When the reaction is pressed, this is what determines what it will do
-
-### Kwargs of the ReactionButton constructor
-| Name | Type | Default Value | Used for
-|------|------|---------------|----------
-| `embed` | `discord.Embed` | `None` | When the reaction is pressed, go to the specified embed
-| `name` | `str` | `None` | The name of the button
-| `details` | [info below](#reactionbuttons-with-reactionbuttontypecaller) | `None` | Assigns the function and it's arguments to call when a `ReactionButton` with `ReactionButton.Type.CALLER` is pressed
-| `event` | `ReactionButton.Event` | `None` | Determine when a button should be removed depending on how many times it has been pressed
-| `skip` | `ReactionButton.Skip` | `None` | Set the action and the amount of pages to skip when using a `linked_to` of `ReactionButton.Type.SKIP`. For example using this button type, setting the action to "+" and the amount 3. If you are on "Page 1/20", pressing that button will bring you to "Page 4/20"
-
-### Attributes for ReactionButton
-| Property | Return Type | Info
-|----------|-------------|------
-| `clicked_by` | `Set[discord.Member]` | The members who clicked the button
-| `total_clicks` | `int` | Amount of clicks from the button
-| `last_clicked` | `Optional[datetime.datetime]` | The time in UTC for when the button was last clicked
-| `menu` | `Optional[ReactionMenu]` | The menu the button is attached to
-
-* Associated methods
-    * `ReactionMenu.add_button(button: ReactionButton)`
-    * `ReactionMenu.remove_all_buttons()`
-    * `ReactionMenu.remove_button(button: ReactionButton)`
-    * `ReactionMenu.get_button(identity: Union[str, int], *, search_by='name')`
-    * `ReactionButton.set_caller_details(func: Callable[..., None], *args, **kwargs)`
-
-
-### All ButtonTypes
-| Type | Info |
-|-------|------|
-| `ReactionButton.Type.NEXT_PAGE` | Go to the next page in the menu session
-| `ReactionButton.Type.PREVIOUS_PAGE` | Go to the previous page in the menu session
-| `ReactionButton.Type.GO_TO_FIRST_PAGE` | Go to the first page in the menu session
-| `ReactionButton.Type.GO_TO_LAST_PAGE` | Go to the last page in the menu session
-| `ReactionButton.Type.GO_TO_PAGE` | Prompts you to type in the page you'd like to go to
-| `ReactionButton.Type.END_SESSION` | Stops the session and deletes the menu message
-| `ReactionButton.Type.CUSTOM_EMBED` | Used separately from the navigation buttons. Once pressed, go to the specified embed 
-| `ReactionButton.Type.CALLER` | Used when specifying the function to call and it's arguments when the button is pressed
-| `ReactionButton.Type.SKIP` | Used to paginate through multiple pages in a single button press
-
-
-### Adding Buttons
-You can add buttons (reactions) to the menu using a `ReactionButton`. Below are examples on how to use each `ButtonType`. 
-> **NOTE:** ReactionButtons with `ReactionButton.Type.CALLER` are a little different, so there is a dedicated section explaining how they work and how to implement them further below
-
-```py
-menu = ReactionMenu(...)
-
-# first and last pages
-fpb = ReactionButton(emoji='⏪', linked_to=ReactionButton.Type.GO_TO_FIRST_PAGE)
-lpb = ReactionButton(emoji='⏩', linked_to=ReactionButton.Type.GO_TO_LAST_PAGE)
-
-# go to page
-gtpb = ReactionButton(emoji='🔢', linked_to=ReactionButton.Type.GO_TO_PAGE)
-
-# end session
-esb = ReactionButton(emoji='⏹️', linked_to=ReactionButton.Type.END_SESSION)
-
-# custom embed
-ceb = ReactionButton(emoji='😎', linked_to=ReactionButton.Type.CUSTOM_EMBED, embed=discord.Embed(title='Hello'))
-
-# skip button
-sb = ReactionButton(emoji='5️⃣', linked_to=ReactionButton.Type.SKIP, skip=ReactionButton.Skip(action='+', amount=5))
-
-menu.add_button(fpb)
-...
-```
-### Deleting Buttons
-Remove all buttons with `menu.remove_all_buttons()`. You can also remove an individual button using its name if you have it set, or the button object itself with `menu.remove_button()`
-
-### ReactionButtons with ReactionButton.Type.CALLER
-`ReactionButton.Type.CALLER` buttons are used to implement your own functionality into the menu. Maybe you want to add a button that creates a text channel, sends a message, or add something to a database, whatever it may be. In order to work with `ReactionButton.Type.CALLER`, use the class method below.
-
-* `ReactionButton.set_caller_details(func: Callable[..., None], *args, **kwargs)`
-  
-This class method is used to setup a function and it's arguments that are later called when the button is pressed. The `ReactionButton` constructor has the kwarg `details`, and that's what you'll use with `.set_caller_details()` to assign the values needed. Some examples are below on how to properly implement `ReactionButton.Type.CALLER`
-
-```py
-@bot.command()
-async def user(ctx, name, *, message):
-    await ctx.send(f"Hi {name}! {message}. We're glad you're here!")
-
-def car(year, make, model):
-    print(f"I have a {year} {make} {model}")
-
-ub = ReactionButton(emoji='👋', linked_to=ReactionButton.Type.CALLER, details=ReactionButton.set_caller_details(user, ctx, 'Defxult', message='Welcome to the server'))
-cb = ReactionButton(emoji='🚗', linked_to=ReactionButton.Type.CALLER, details=ReactionButton.set_caller_details(car, 2021, 'Ford', 'Mustang'))
-```
-> **NOTE:** The function you pass in should not return anything. Calling functions with `ReactionButton.Type.CALLER` does not store or handle anything returned by that function
----
-
-### ReactionButton Methods
-The `ReactionButton` class comes with a set factory methods (class methods) that returns a `ReactionButton` with parameters set according to their `linked_to`.
-
-* `ReactionButton.back()`
-  * `emoji`: "◀️"
-  * `linked_to`: `ReactionButton.Type.PREVIOUS_PAGE`
-* `ReactionButton.next()`
-	* `emoji`: "▶️"
-	* `linked_to`: `ReactionButton.Type.NEXT_PAGE`
-* `ReactionButton.go_to_first_page()`
-	* `emoji`: "⏪"
-	* `linked_to`: `ReactionButton.Type.GO_TO_FIRST_PAGE`
-* `ReactionButton.go_to_last_page()`
-	* `emoji`: "⏩"
-	* `linked_to`: `ReactionButton.Type.GO_TO_LAST_PAGE`
-* `ReactionButton.go_to_page()`
-	* `emoji`: "🔢"
-	* `linked_to`: `ReactionButton.Type.GO_TO_PAGE`
-* `ReactionButton.end_session()`
-	* `emoji`: "⏹️"
-	* `linked_to`: `ReactionButton.Type.END_SESSION`
-* `ReactionButton.all()`
-  * Returns a `list` of `ReactionButton` in the following order
-  * `.go_to_first_page()` `.back()` `.next()` `.go_to_last_page()` `.go_to_page()` `.end_session()`
-* `ReactionButton.generate_skip(emoji: str, action: str, amount: int)`
-  * `emoji`: `<emoji>`
-  * `linked_to`: `ReactionButton.Type.SKIP`
-  * `skip`: `ReactionButton.Skip(<action>, <amount>)`
-
----
-### Setting Limits
-If you'd like, you can limit the amount of reaction menus that can be active at the same time *per* "guild", "member", or "channel" 
-* Associated CLASS Methods
-    * `ReactionMenu.set_sessions_limit(limit: int, per='guild', message='Too many active menus. Wait for other menus to be finished.')` 
-    * `ReactionMenu.remove_limit()`
-
-Example:
-```py
-@bot.command()
-async def limit(ctx):
-    ReactionMenu.set_sessions_limit(3, per='member', message='Sessions are limited to 3 per member')
-```
-
-With the above example, only 3 menus can be active at once for each member, and if they try to create more before their other menu's are finished, they will get an error message saying "Sessions are limited to 3 per member".
-
-### ReactionButton Events
-You can set a `ReactionButton` to be removed when it has been pressed a certain amount of times
-
-```
-class ReactionButton.Event(event_type: str, value: int)
-```
-
-#### Parameters for ReactionButton.Event
-* `event_type` (`str`) The action to take. The only available option is "remove"
-* `value` (`int`) The amount set for the specified event. Must be >= 1. If value is <= 0, it is implicitly set to 1
-
-Example:
-```py
-menu = ReactionMenu(ctx, ...)
-
-# remove a button after 10 clicks
-button = ReactionButton(..., event=ReactionButton.Event('remove', 10))
-menu.add_button(button)
-```
-> **NOTE:** Not ideal for buttons with a `linked_to` of `ReactionButton.Type.END_SESSION`
----
-### ReactionMenu Relays
-Menu relays are functions that are called anytime a button that is apart of a menu is pressed. It is considered as an extension of a `ReactionButton` with a `linked_to` of `ReactionButton.Type.CALLER`. Unlike caller buttons which provides no details about the interactions on the menu, relays do.
-* Associated methods
-  * `ReactionMenu.set_relay(func: Callable[[NamedTuple], None], *, only: Optional[List[ReactionButton]]=None)`
-  * `ReactionMenu.remove_relay()`
-
-When creating a function for your relay, that function must contain a single positional argument. When a button is pressed, a `RelayPayload` object (a named tuple) is passed to that function. The attributes of `RelayPayload` are:
-* `member` (`discord.Member`) The person who pressed the button
-* `button` (`ReactionButton`) The button that was pressed
-
-Example:
-```py
-async def enter_giveaway(payload):
-    member = payload.member
-    channel = payload.button.menu.message.channel
-    await channel.send(f"{member.mention}, you've entered the giveaway!")
-
-menu = ReactionMenu(ctx, ...)
-menu.set_relay(enter_giveaway)
-```
-The `set_relay` method comes with the `only` parameter. If that parameter is `None`, all buttons that are pressed will be relayed. You can provide a `list` of buttons to that parameter so only button presses from those specified buttons will be relayed.
-```py
-def example(payload):
-    ...
-
-menu = ReactionMenu(ctx, ...)
-
-back_button = ReactionButton.back()
-next_button = ReactionButton.next()
-
-menu.set_relay(example, only=[back_button])
-```
-
----
-### Starting/Stopping the ReactionMenu
-* Associated methods
-  * `await ReactionMenu.start(*, send_to=None, reply=False)`
-  * `await ReactionMenu.stop(*, delete_menu_message=False, clear_reactions=False)`
-
-When starting the menu, you have the option to send the menu to a certain channel. Parameter `send_to` is the channel you'd like to send the menu to. You can set `send_to` as the channel name (`str`), channel ID (`int`), or channel object (`discord.TextChannel` / `discord.Thread`). Example:
-```py
-menu = ReactionMenu(...)
-# channel name
-await menu.start(send_to='bot-commands')
-
-# channel ID
-await menu.start(send_to=1234567890123456)
-
-# channel object
-channel = guild.get_channel(1234567890123456)
-await menu.start(send_to=channel)
-
-# there's no need to specify send_to unless you want the menu to be sent to a different channel
-# from the one you're sending the initial message/using the command in. the menu can be started
-# in the current channel by omitting the send_to parameter
-await menu.start()
-```
-> **NOTE:** `send_to` is not valid if a menu was started in DM's
-
-### Full Example
-Here is a basic implementation of `ReactionMenu` that you can copy & paste for a quick demonstration.
-```py
-import asyncio
-import discord
-from discord.ext import commands
-from reactionmenu import ReactionMenu, ReactionButton
-
-bot = commands.Bot(command_prefix='!', intents=discord.Intents.all())
-
-async def start_bot():
-    async with bot:
-        await bot.start('...')
-
-@bot.command()
-async def example(ctx):
-    menu = ReactionMenu(ctx, menu_type=ReactionMenu.TypeEmbed)
-    
-    for member in ctx.guild.members:
-        if member.avatar:
-            embed = discord.Embed(description=f'Joined {member.joined_at.strftime("%b. %d, %Y")}')
-            embed.set_author(name=member.name, icon_url=member.avatar.url)
-            menu.add_page(embed)
-    
-    menu.add_button(ReactionButton.back())
-    menu.add_button(ReactionButton.next())
-    menu.add_button(ReactionButton.end_session())
-    
-    await menu.start()
-
-asyncio.run(start_bot())
-```
-</details>
-
-
-
-
-
-
-
-
-
-
----
-
-
-
-
-
-
-
-
-
-
-## ViewMenu
-```
-class reactionmenu.ViewMenu(method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs)
-```
-
-A `ViewMenu` is a menu that uses discords Buttons feature. With buttons, you can enable and disable them, set a certain color for them with emojis, have buttons that send hidden messages, and add hyperlinks. This library offers a broader range of functionalities such as who pressed the button, how many times it was pressed and more. It uses views (`discord.ui.View`) to implement the Buttons functionality, but uses some of its own methods in order to make a Button pagination menu simple.
-
-![image](https://cdn.discordapp.com/attachments/655186216060321816/855818139450081280/buttons_showcase_reduced.gif)
-
-<details>
-  <summary><b>Click to show ViewMenu documentation</b></summary>
-
-
-### How to import
-```py
-from reactionmenu import ViewMenu, ViewButton
-```
----
-
-### Parameters of the ViewMenu constructor
-* `method` (`Union[discord.ext.commands.Context, discord.Interaction]`) A context or interaction object
-* `menu_type` (`MenuType`) The configuration of the menu
-  * `ViewMenu.TypeEmbed`, a normal embed pagination menu
-  * `ViewMenu.TypeEmbedDynamic`, an embed pagination menu with dynamic data
-  * `ViewMenu.TypeText`, a text only pagination menu
-
----
-### Kwargs of the ViewMenu constructor
-| Name | Type | Default Value | Used for | Info 
--------|------|---------------|----------|------
-| `wrap_in_codeblock` | `str` | `None` | `ViewMenu.TypeEmbedDynamic` | The discord codeblock language identifier to wrap your data in. Example: `ViewMenu(ctx, ..., wrap_in_codeblock='py')`
-| `custom_embed` | `discord.Embed` | `None` | `ViewMenu.TypeEmbedDynamic` | Embed object to use when adding data with `ViewMenu.add_row()`. Used for styling purposes
-| `delete_on_timeout` | `bool` | `False` | `All menu types` | Delete the menu when it times out
-| `disable_items_on_timeout` | `bool` | `True` | `All menu types` | Disable the items on the menu when the menu times out
-| `remove_items_on_timeout` | `bool` | `False` | `All menu types` | Remove the items on the menu when the menu times out
-| `only_roles` | `List[discord.Role]` | `None` | `All menu types` | If set, only members with any of the given roles are allowed to control the menu. The menu owner can always control the menu
-| `timeout` | `Union[int, float, None]` | `60.0` | `All menu types` | The timer for when the menu times out. Can be `None` for no timeout
-| `show_page_director` | `bool` | `True` | `All menu types` | Shown at the bottom of each embed page. "Page 1/20"
-| `name` | `str` | `None` | `All menu types` | A name you can set for the menu
-| `style` | `str` | `"Page $/&"` | `All menu types` | A custom page director style you can select. "$" represents the current page, "&" represents the total amount of pages. Example: `ViewMenu(ctx, ..., style='On $ out of &')`
-| `all_can_click` | `bool` | `False` | `All menu types` | Sets if everyone is allowed to control when pages are 'turned' when buttons are clicked
-| `delete_interactions` | `bool` | `True` | `All menu types` | Delete the prompt message by the bot and response message by the user when asked what page they would like to go to when using `ViewButton.ID_GO_TO_PAGE`
-| `rows_requested` | `int` | `None` | `ViewMenu.TypeEmbedDynamic` | The amount of information per `ViewMenu.add_row()` you would like applied to each embed page
----
-
-### Pages for ViewMenu
-Depending on the `menu_type`, pages can either be a `str`, `discord.Embed`, or a combination of `content` or `files` ([example below](#stacked-pages-1))
-* If the `menu_type` is `ViewMenu.TypeEmbed`, use embeds
-* If the `menu_type` is `ViewMenu.TypeText` (text only menu) or `ViewMenu.TypeEmbedDynamic` (embed only menu), use strings.
-* Associated methods
-  * `ViewMenu.add_page(embed: discord.Embed=MISSING, content: Optional[str]=None, files: Optional[Sequence[discord.File]]=None)`
-  * `ViewMenu.add_pages(pages: Sequence[Union[discord.Embed, str]])`
-  * `ViewMenu.add_row(data: str)`
-  * `ViewMenu.remove_all_pages()`
-  * `ViewMenu.clear_all_row_data()`
-  * `ViewMenu.remove_page(page_number: int)`
-  * `ViewMenu.set_main_pages(*embeds: Embed)`
-  * `ViewMenu.set_last_pages(*embeds: Embed)`
-
-#### Adding Pages
-```py
-# ViewMenu.TypeEmbed
-menu = ViewMenu(method, menu_type=ViewMenu.TypeEmbed)
-menu.add_page(summer_embed)
-menu.add_page(winter_embed)
-
-# ViewMenu.TypeText
-menu = ViewMenu(method, menu_type=ViewMenu.TypeText)
-menu.add_page(content='Its so hot!')
-menu.add_page(content='Its so cold!')
-```
-
-#### ViewMenu.TypeText
-A `TypeText` menu is a text based pagination menu. No embeds are involved in the pagination process, only plain text is used.
-
-![text_view_showcase](https://cdn.discordapp.com/attachments/655186216060321816/929744985656549386/text_view_showcase.gif)
-
-#### Stacked Pages
-With `v3.1.0+`, you can paginate with more than just an embed or text. You can combine text, embeds, as well as files. But depending on the `menu_type` the combination can be restricted. Here is an example of a menu with a `menu_type` of `TypeEmbed` that is stacked.
-
-```py
-# You can use regular commands as well
-@bot.tree.command(description="These are stacked pages", guild=discord.Object(id=...))
-async def stacked(interaction: discord.Interaction):
-    menu = ViewMenu(interaction, menu_type=ViewMenu.TypeEmbed)
-
-    menu.add_page(discord.Embed(title="My Embed"), content="This content is stacked on top of a file", files=[discord.File("stacked.py")])
-    menu.add_page(discord.Embed(title="Hey Wumpos, can you say hi to the person reading this? 😃"))
-    menu.add_page(discord.Embed(title="Hi, I'm Wumpos!"), files=[discord.File("wumpos.gif")])
-    
-    menu.add_button(ViewButton.back())
-    menu.add_button(ViewButton.next())
-    
-    await menu.start()
-```
-![stacked_view](https://cdn.discordapp.com/attachments/655186216060321816/955983620038860910/stacked_view.gif)
-
-Since the `menu_type` is `TypeEmbed`, there always has to be an embed on each page. If the `menu_type` was `TypeText`, embeds aren't allowed and you will be restricted to only using the `files` parameter.
-
-#### ViewMenu.TypeEmbedDynamic
-A dynamic menu is used when you do not know how much information will be applied to the menu. For example, if you were to request information from a database, that information can always change. You query something and you might get 1,500 results back, and the next maybe only 800. A dynamic menu pieces all this information together for you and adds it to an embed page by rows of data. `ViewMenu.add_row()` is best used in some sort of `Iterable` where everything can be looped through, but only add the amount of data you want to the menu page.
-> **NOTE:** In a dynamic menu, all added data is placed in the description section of an embed. If you choose to use a `custom_embed`, all text in the description will be overridden with the data you add
-* Associated methods
-    * `ViewMenu.add_row(data: str)`
-    * `ViewMenu.clear_all_row_data()`
-    * `ViewMenu.set_main_pages(*embeds: Embed)`
-    * `ViewMenu.set_last_pages(*embeds: Embed)`
-* The kwargs specifically made for a dynamic menu are:
-    * `rows_requested` - The amount of rows you would like on each embed page before making a new page
-        * `ViewMenu(..., rows_requested=5)`
-    * `custom_embed` - An embed you have created to use as the embed pages. Used for your menu aesthetic
-        * `ViewMenu(..., custom_embed=red_embed)`
-    * `wrap_in_codeblock` - The language identifier when wrapping your data in a discord codeblock. 
-        * `ViewMenu(..., wrap_in_codeblock='py')`
-
-##### Adding Rows/data
-```py
-menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbedDynamic, rows_requested=5)
-
-for data in database.request('SELECT * FROM customers'):
-    menu.add_row(data)
-```
-##### Deleting Data
-You can remove all the data you've added to a menu by using `menu.clear_all_row_data()`
-
-##### Main/Last Pages
-When using a dynamic menu, the only embed pages you see are from the data you've added. But if you would like to show more pages other than just the data, you can use methods `ViewMenu.set_main_pages()` and `ViewMenu.set_last_pages()`. Setting the main page(s), the embeds you set will be the first embeds that are shown when the menu starts. Setting the last page(s) are the last embeds shown
-```py
-menu.set_main_pages(welcome_embed, announcement_embed)
-
-for data in get_information():
-    menu.add_row(data)
-
-menu.set_last_pages(additional_info_embed)
-# NOTE: setting main/last pages can be set in any order
-```
-
-### Buttons for ViewMenu
-Buttons are what you use to interact with the menu. Unlike reactions, they look cleaner, provides less rate limit issues, and offer more in terms of interactions. Enable and disable buttons, use markdown hyperlinks in it's messages, and even send hidden messages.
-
-![discord_buttons](https://discord.com/assets/7bb017ce52cfd6575e21c058feb3883b.png)
-
-
-* Associated methods
-  * `ViewMenu.add_button(button: ViewButton)`
-  * `ViewMenu.disable_all_buttons()`
-  * `ViewMenu.disable_button(button: ViewButton)`
-  * `ViewMenu.enable_all_buttons()`
-  * `ViewMenu.enable_button(button: ViewButton)`
-  * `ViewMenu.get_button(identity: str, *, search_by='label')`
-  * `ViewMenu.remove_all_buttons()`
-  * `ViewMenu.remove_button(button: ViewButton)`
-  * `await ViewMenu.refresh_menu_items()`
-
-#### ViewButton
-```
-class reactionmenu.ViewButton(*, style=discord.ButtonStyle.secondary, label=None, disabled=False, custom_id=None, url=None, emoji=None, followup=None, event=None, **kwargs)
-```
-
-A `ViewButton` is a class that represents the discord button. It is a subclass of `discord.ui.Button`.
-
-The following are the rules set by Discord for Buttons:
-* Link buttons don't send interactions to the Discord App, so link button statistics (it's properties) are not tracked
-* Non-link buttons **must** have a `custom_id`, and cannot have a `url`
-* Link buttons **must** have a `url`, and cannot have a `custom_id`
-* There cannot be more than 25 buttons per message
----
-#### Parameters of the ViewButton constructor
-* `style` (`discord.ButtonStyle`) The button style
-* `label` (`str`) The text on the button
-* `custom_id` (`str`) An ID to determine what action that button should take. Available IDs:
-  * `ViewButton.ID_NEXT_PAGE`
-  * `ViewButton.ID_PREVIOUS_PAGE`
-  * `ViewButton.ID_GO_TO_FIRST_PAGE` 
-  * `ViewButton.ID_GO_TO_LAST_PAGE`
-  * `ViewButton.ID_GO_TO_PAGE`
-  * `ViewButton.ID_END_SESSION`
-  * `ViewButton.ID_CALLER`
-  * `ViewButton.ID_SEND_MESSAGE`
-  * `ViewButton.ID_CUSTOM_EMBED`
-  * `ViewButton.ID_SKIP`
-* `emoji` (`Union[str, discord.PartialEmoji]`) Emoji used for the button
-  * `ViewButton(..., emoji='😄')` 
-  * `ViewButton(..., emoji='<:miscTwitter:705423192818450453>')`
-  * `ViewButton(..., emoji='\U000027a1')`
-  * `ViewButton(..., emoji='\N{winking face}')`
-* `url` (`str`) URL for a button with style `discord.ButtonStyle.link`
-* `disabled` (`bool`) If the button should be disabled
-* `followup` (`ViewButton.Followup`) The message sent after the button is pressed. Only available for buttons that have a `custom_id` of `ViewButton.ID_CALLER` or `ViewButton.ID_SEND_MESSAGE`. `ViewButton.Followup` is a class that has parameters similar to `discord.abc.Messageable.send()`, and is used to control if a message is ephemeral, contains a file, embed, tts, etc...
-* `event` (`ViewButton.Event`) Set a button to be disabled or removed when it has been pressed a certain amount of times
-
-#### Kwargs of the ViewButton constructor
-| Name | Type | Default Value | Used for
-|------|------|---------------|----------
-| `name` | `str` | `None` | The name of the button
-| `skip` | `ViewButton.Skip` | `None` | Set the action and the amount of pages to skip when using a `custom_id` of `ViewButton.ID_SKIP`. For example, setting the action to "+" and the amount 3. If you are on "Page 1/20", pressing that button will bring you to "Page 4/20"
-| `persist` | `bool` | `False` | Prevents link buttons from being disabled/removed when the menu times out or is stopped so they can remain clickable
-
-#### Attributes for ViewButton
-| Property | Return Type | Info
-|----------|-------------|------
-| `clicked_by` | `Set[discord.Member]` | The members who clicked the button
-| `total_clicks` | `int` | Amount of clicks from the button
-| `last_clicked` | `Optional[datetime.datetime]` | The time in UTC for when the button was last clicked
-| `menu` | `Optional[ViewMenu]` | The menu the button is attached to
-
-#### Adding a ViewButton
-```py
-from reactionmenu import ViewMenu, ViewButton
-
-menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
-
-# Link button
-link_button = ViewButton(style=discord.ButtonStyle.link, emoji='🌍', label='Link to Google', url='https://google.com')
-menu.add_button(link_button)
-
-# Skip button
-skip = ViewButton(style=discord.ButtonStyle.primary, label='+5', custom_id=ViewButton.ID_SKIP, skip=ViewButton.Skip(action='+', amount=5))
-menu.add_button(skip)
-
-# ViewButton.ID_PREVIOUS_PAGE
-back_button = ViewButton(style=discord.ButtonStyle.primary, label='Back', custom_id=ViewButton.ID_PREVIOUS_PAGE)
-menu.add_button(back_button)
-
-# ViewButton.ID_NEXT_PAGE
-next_button = ViewButton(style=discord.ButtonStyle.secondary, label='Next', custom_id=ViewButton.ID_NEXT_PAGE)
-menu.add_button(next_button)
-
-# All other ViewButton are created the same way as the last 2 EXCEPT
-# 1 - ViewButton.ID_CALLER
-# 2 - ViewButton.ID_SEND_MESSAGE
-# 3 - ViewButton.ID_CUSTOM_EMBED
-
-
-# ViewButton.ID_CALLER
-def say_hello(name: str):
-    print('Hello', name)
-
-call_followup = ViewButton.Followup(details=ViewButton.Followup.set_caller_details(say_hello, 'John'))
-menu.add_button(ViewButton(label='Say hi', custom_id=ViewButton.ID_CALLER, followup=call_followup))
-
-# ViewButton.ID_SEND_MESSAGE
-msg_followup = ViewButton.Followup('This message is hidden!', ephemeral=True)
-menu.add_button(ViewButton(style=discord.ButtonStyle.green, label='Message', custom_id=ViewButton.ID_SEND_MESSAGE, followup=msg_followup))
-
-# ViewButton.ID_CUSTOM_EMBED
-custom_embed_button = ViewButton(style=discord.ButtonStyle.blurple, label='Social Media Info', custom_id=ViewButton.ID_CUSTOM_EMBED, followup=ViewButton.Followup(embed=discord.Embed(...)))
-```
----
-> **NOTE:** When it comes to buttons with a `custom_id` of `ViewButton.ID_CALLER`, `ViewButton.ID_SEND_MESSAGE`, `ViewButton.ID_CUSTOM_EMBED`, or link buttons, you can add as many as you'd like as long as in total it's 25 buttons or less. For all other button ID's, each menu can only have one.
-
-### Using Selects
-Selects are used when you'd like to categorize information in your menu. Selects can only be used when the menu's `menu_type` is `TypeEmbed`. You should keep in mind that discords limitations on how many menu UI items (rows) can be applied to each message.
-
-![select_showcase](https://cdn.discordapp.com/attachments/655186216060321816/971361708121653268/select_showcase.gif)
-
-* Associated Methods
-  * `ViewMenu.add_select(select: ViewSelect)`
-  * `ViewMenu.remove_select(select: ViewSelect)`
-  * `ViewMenu.remove_all_selects()`
-  * `ViewMenu.disable_select(select: ViewSelect)`
-  * `ViewMenu.disable_all_selects()`
-  * `ViewMenu.enable_select(select: ViewSelect)`
-  * `ViewMenu.enable_all_selects()`
-  * `ViewMenu.get_select(title: Union[str, None])`
-
-Example:
-```py
-from reactionmenu import ViewMenu, ViewSelect, Page
-
-menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
-menu.add_page(discord.Embed(title="A showcase of console video games", color=discord.Color.blurple()))
-
-menu.add_select(ViewSelect(title="Console Video Games", options={
-    discord.SelectOption(label="PlayStation", emoji="<:PlayStation:549638412538478602>") : [
-        Page(embed=discord.Embed(title="Ratchet & Clank", description=..., color=discord.Color.yellow()).set_image(url=...)),
-        Page(embed=discord.Embed(title="God of War", description=..., color=discord.Color.blue()).set_image(url=...))
-    ],
-    discord.SelectOption(label="Xbox", emoji="<:Xbox:501880493285834752>") : [
-        Page(embed=discord.Embed(title="Halo Infinite", description=..., color=discord.Color.green()).set_image(url=...)),
-        Page(embed=discord.Embed(title="Gears of War 4", description=..., color=discord.Color.red()).set_image(url=...))
-    ]
-}))
-
-menu.add_button(ViewButton.back())
-menu.add_button(ViewButton.next())
-await menu.start()
-```
-
-#### Go to page navigation
-You can use this type of select when you'd like to use the UI to select a page to go to.
-
-![goto_showcase](https://cdn.discordapp.com/attachments/655186216060321816/973629631905300501/Discord_6SP5AjoOOM.gif)
-
-* Associated methods
-  * `ViewMenu.add_go_to_select(goto: ViewSelect.GoTo)`
-  * `ViewMenu.enable_go_to_select(goto: ViewSelect.GoTo)`
-  * `ViewMenu.enable_all_go_to_selects()`
-  * `ViewMenu.disable_go_to_select(goto: ViewSelect.GoTo)`
-  * `ViewMenu.disable_all_go_to_selects()`
-  * `ViewMenu.remove_go_to_select(goto: ViewSelect.GoTo)`
-  * `ViewMenu.remove_all_go_to_selects()`
-
-The `page_numbers` parameter for `ViewSelect.GoTo` can be used with 3 different types
-
-1. `List[int]` If set to a list of integers, those specified values are the only options that are available when the select is clicked
-   1. `page_numbers=[1, 5, 10]`
-2. `Dict[int, Union[str, discord.Emoji, discord.PartialEmoji]]` You can use this type if you'd like to utilize emojis in your select
-   1. `page_numbers={1 : "🗯️", 2 : "📺"}`
-3. `ellipsis` You can set a *literal* ellipsis to have the library automatically assign all page numbers to the amount of pages that you've added to the menu. This can come in handy if you have 25 pages or less
-   1. `page_numbers=...`
-> **NOTE**: Setting the `page_numbers` parameter to an ellipsis (...) only works as intended if you've added the go to select AFTER you've added pages to the menu
-
-```py
-@bot.command()
-async def navigate(ctx):
-    menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
-
-    menu.add_page(discord.Embed(title="Twitter").set_image(url="..."))
-    menu.add_page(discord.Embed(title="YouTube").set_image(url="..."))
-    menu.add_page(discord.Embed(title="Discord").set_image(url="..."))
-    # ...
-    
-    menu.add_go_to_select(ViewSelect.GoTo(title="Go to page...", page_numbers=...))
-
-    menu.add_button(ViewButton.back())
-    menu.add_button(ViewButton.next())
-
-    await menu.start()
-```
-
-### Updating ViewButton and Pages
-* Associated methods
-  * `await ViewMenu.refresh_menu_items()`
-  * `await ViewMenu.update(*, new_pages: Union[List[Union[Embed, str]], None], new_buttons: Union[List[ViewButton], None])`
-
-When the menu is running, you can update the pages or buttons on the menu. Using `ViewMenu.update()`, you can replace the pages and buttons. Using `ViewMenu.refresh_menu_items()` updates the buttons you have changed.
-
-#### Updating a Button
-```py
-@bot.command()
-async def menu(ctx):
-    menu = ViewMenu(..., name='test')
-    link_button = ViewButton(..., label='Link')
-    
-    menu.add_button(link_button)
-    menu.add_page(...)
-
-    await menu.start()
-
-
-@bot.command()
-async def disable(ctx):
-    menu = ViewMenu.get_session('test')
-    link_button = menu[0].get_button('Link', search_by='label')
-    
-    menu.disable_button(link_button)
-    await menu.refresh_menu_items()
-```
-If the buttons are not refreshed with `ViewMenu.refresh_menu_items()`, the menu will not be updated when changing a button.
-
-#### Updating Pages and Buttons
-Method `ViewMenu.update(...)` is used when you want to replace all or a few of the buttons on the menu. 
-```py
-menu = ViewMenu(...)
-
-# in a different .command()
-await menu.update(new_pages=[hello_embed, goodbye_embed], new_buttons=[link_button, next_button])
-```
-
-> **NOTE**: When using `ViewMenu.update(...)`, there is no need to use `ViewMenu.refresh_menu_items()` because they are updated during the update call. 
-
----
-#### ViewButton Methods
-The `ViewButton` class comes with a set factory methods (class methods) that returns a `ViewButton` with parameters set according to their `custom_id` (excluding link buttons).
-
-* `ViewButton.link(label: str, url: str)`
-  * `style`: `discord.ButtonStyle.link`
-  * `label`: `<label>`
-  * `url`: `<url>`
-* `ViewButton.back()`
-  * `style`: `discord.ButtonStyle.gray`
-  * `label`: "Back"
-  * `custom_id`: `ViewButton.ID_PREVIOUS_PAGE`
-* `ViewButton.next()`
-	* `style`: `discord.ButtonStyle.gray`
-	* `label`: "Next"
-	* `custom_id`: `ViewButton.ID_NEXT_PAGE`
-* `ViewButton.go_to_first_page()`
-	* `style`: `discord.ButtonStyle.gray`
-	* `label`: "First Page"
-	* `custom_id`: `ViewButton.ID_GO_TO_FIRST_PAGE`
-* `ViewButton.go_to_last_page()`
-	* `style`: `discord.ButtonStyle.gray`
-	* `label`: "Last Page"
-	* `custom_id`: `ViewButton.ID_GO_TO_LAST_PAGE`
-* `ViewButton.go_to_page()`
-	* `style`: `discord.ButtonStyle.gray`
-	* `label`: "Page Selection"
-	* `custom_id`: `ViewButton.ID_GO_TO_PAGE`
-* `ViewButton.end_session()`
-	* style: `discord.ButtonStyle.gray`
-	* label: "Close"
-	* custom_id: `ViewButton.ID_END_SESSION`
-* `ViewButton.all()`
-  * Returns a `list` of `ViewButton` in the following order
-  * `.go_to_first_page()` `.back()` `.next()` `.go_to_last_page()` `.go_to_page()` `.end_session()`
-* `ViewButton.all_with_emojis()`
-  * Returns a `list` of `ViewButton` with their `emoji` parameters already set in the following order
-  * `.go_to_first_page()` `.back()` `.next()` `.go_to_last_page()` `.go_to_page()` `.end_session()`
-* `ViewButton.generate_skip(label: str, action: str, amount: int)`
-  * `style`: `discord.ButtonStyle.gray`
-  * `label`: `<label>`
-  * `custom_id`: `ViewButton.ID_SKIP`
-  * `skip`: `ViewButton.Skip(<action>, <amount>)`
-
-```py
-menu = ViewMenu(ctx, ...)
-menu.add_page(...)
-menu.add_page(...)
-
-menu.add_button(ViewButton.back())
-menu.add_button(ViewButton.next())
-
-await menu.start()
-```
----
-### ViewButton Events
-You can set a `ViewButton` to be disabled or removed when it has been pressed a certain amount of times
-
-```
-class ViewButton.Event(event_type: str, value: int)
-```
-
-#### Parameters for ViewButton.Event
-* `event_type` (`str`) The action to take. Can either be "disable" or "remove"
-* `value` (`int`) The amount set for the specified event. Must be >= 1. If value is <= 0, it is implicitly set to 1
-
-Example:
-```py
-menu = ViewMenu(ctx, ...)
-
-# disable a button after 5 clicks
-button_1 = ViewButton(..., event=ViewButton.Event('disable', 5))
-menu.add_button(button_1)
-
-# remove a button after 10 clicks
-button_2 = ViewButton(..., event=ViewButton.Event('remove', 10))
-menu.add_button(button_2)
-```
-> **NOTE:** Not valid for link buttons. Also not ideal for buttons with a `custom_id` of `ViewButton.ID_END_SESSION`
----
-### ViewMenu Relays
-Menu relays are functions that are called anytime a button that is apart of a menu is pressed. It is considered as an extension of a `ViewButton` with an ID of `ViewButton.ID_CALLER`. Unlike caller buttons which provides no details about the interactions on the menu, relays do.
-* Associated methods
-  * `ViewMenu.set_relay(func: Callable[[NamedTuple], None], *, only: Optional[List[ViewButton]]=None)`
-  * `ViewMenu.remove_relay()`
-
-When creating a function for your relay, that function must contain a single positional argument. When a button is pressed, a `RelayPayload` object (a named tuple) is passed to that function. The attributes of `RelayPayload` are:
-* `member` (`discord.Member`) The person who pressed the button
-* `button` (`ViewButton`) The button that was pressed
-
-Example:
-```py
-async def enter_giveaway(payload):
-    member = payload.member
-    channel = payload.button.menu.message.channel
-    await channel.send(f"{member.mention}, you've entered the giveaway!")
-
-menu = ViewMenu(ctx, ...)
-menu.set_relay(enter_giveaway)
-```
-The `set_relay` method comes with the `only` parameter. If that parameter is `None`, all buttons that are pressed will be relayed (except link buttons because they don't send interaction events). You can provide a `list` of buttons to that parameter so only button presses from those specified buttons will be relayed.
-```py
-def example(payload):
-    ...
-
-menu = ViewMenu(ctx, ...)
-
-back_button = ViewButton.back()
-next_button = ViewButton.next()
-
-menu.set_relay(example, only=[back_button])
-```
-
----
-### Starting/Stopping the ViewMenu
-* Associated methods
-  * `await ViewMenu.start(*, send_to=None, reply=False)`
-  * `await ViewMenu.stop(*, delete_menu_message=False, remove_buttons=False, disable_buttons=False)`
-
-When starting the menu, you have the option to send the menu to a certain channel. Parameter `send_to` is the channel you'd like to send the menu to. You can set `send_to` as the channel name (`str`), channel ID (`int`), or channel object (`discord.TextChannel` / `discord.Thread`). Example:
-```py
-menu = ViewMenu(...)
-# channel name
-await menu.start(send_to='bot-commands')
-
-# channel ID
-await menu.start(send_to=1234567890123456)
-
-# channel object
-channel = guild.get_channel(1234567890123456)
-await menu.start(send_to=channel)
-
-# there's no need to specify send_to unless you want the menu to be sent to a different channel
-# from the one you're sending the initial message/using the command in. the menu can be started
-# in the current channel by omitting the send_to parameter
-await menu.start()
-```
-> **NOTE:** `send_to` is not valid if a menu was started in DM's
-
-Only one option is available when stopping the menu. If you have multiple parameters as `True`, only one will execute
-- `delete_menu_message` > `disable_buttons`
-- `disable_buttons` > `remove_buttons`
----
-
-### Full Example
-Here is a basic implementation of `ViewMenu` that you can copy & paste for a quick demonstration.
-```py
-import asyncio
-import discord
-from discord.ext import commands
-from reactionmenu import ViewMenu, ViewButton
-
-bot = commands.Bot(command_prefix='!', intents=discord.Intents.all())
-
-async def start_bot():
-    async with bot:
-        await bot.start('...')
-
-@bot.command()
-async def example(ctx):
-    menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
-    
-    for member in ctx.guild.members:
-        if member.avatar:
-            embed = discord.Embed(description=f'Joined {member.joined_at.strftime("%b. %d, %Y")}')
-            embed.set_author(name=member.name, icon_url=member.avatar.url)
-            menu.add_page(embed)
-    
-    menu.add_button(ViewButton.back())
-    menu.add_button(ViewButton.next())
-    menu.add_button(ViewButton.end_session())
-    
-    await menu.start()
-
-asyncio.run(start_bot())
-```
-</details>
+Metadata-Version: 2.1
+Name: reactionmenu
+Version: 3.1.4
+Summary: A library to create a discord.py 2.0+ paginator. Supports pagination with buttons, reactions, and category selection using selects.
+Author: Defxult
+License: MIT
+Project-URL: Homepage, https://github.com/Defxult/reactionmenu
+Project-URL: Changelog, https://github.com/Defxult/reactionmenu/blob/main/CHANGELOG.md
+Keywords: buttons,buttons paginator,buttons menu,discord,discord.py,discord.py 2.0,d.py,components,components paginator,components menu,discord components,discord components menu,discord buttons,discord buttons paginator,discord buttons menu,discord paginator,discord pagination,discord reaction menu,discord reactions,discord embed,discord menu,discord interactions,embed menu,embed reaction menu,embed paginator,interactions,interactions menu,interactions paginator,menus,paginator,pagination,pagination menu,reaction menu
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![logo](https://cdn.discordapp.com/attachments/655186216060321816/820162226316378162/discord.jpg)
+<div align="center">
+
+[![Downloads](https://pepy.tech/badge/reactionmenu)](https://pepy.tech/project/reactionmenu) 
+[![Downloads](https://pepy.tech/badge/reactionmenu/month)](https://pepy.tech/project/reactionmenu)
+[![Downloads](https://pepy.tech/badge/reactionmenu/week)](https://pepy.tech/project/reactionmenu)
+
+![python_version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
+</div>
+
+## How to install
+You can install the latest [PyPI](https://pypi.org/project/reactionmenu/) version of the library by doing:
+```
+$ pip install reactionmenu
+```
+Or the development version:
+```
+$ pip install git+https://github.com/Defxult/reactionmenu
+```
+
+## Intents
+Minimum intents needed
+```py
+bot = commands.Bot(..., intents=discord.Intents(messages=True, guilds=True, reactions=True, members=True))
+```
+---
+## ReactionMenu
+
+```
+class reactionmenu.ReactionMenu(method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs)
+```
+
+A `ReactionMenu` is a menu that uses emojis which are either custom guild emojis or a normal emoji to control the pagination process. If you're not looking for any of the fancy features and just want something simple, this is the one to use.
+
+![showcase](https://cdn.discordapp.com/attachments/655186216060321816/819885696176226314/showcase.gif)
+
+<details>
+  <summary><b>Click to show ReactionMenu documentation</b></summary>
+
+### How to import
+```py
+from reactionmenu import ReactionMenu, ReactionButton
+```
+This library comes with several methods and options in order to make a discord reaction menu simple. Once you have imported the proper classes, you will initialize the constructor like so:
+```py
+menu = ReactionMenu(method, menu_type=ReactionMenu.TypeEmbed)
+```
+
+
+### Parameters of the ReactionMenu constructor
+* `method` (`Union[discord.ext.commands.Context, discord.Interaction]`) A context or interaction object
+* `menu_type` (`MenuType`) The configuration of the menu
+  * `ReactionMenu.TypeEmbed`, a normal embed pagination menu
+  * `ReactionMenu.TypeEmbedDynamic`, an embed pagination menu with dynamic data
+  * `ReactionMenu.TypeText`, a text only pagination menu
+
+
+### Kwargs of the ReactionMenu constructor
+| Name | Type | Default Value | Used for | Info 
+-------|------|---------------|----------|------
+| `wrap_in_codeblock` | `str` | `None` | `ReactionMenu.TypeEmbedDynamic` | The discord codeblock language identifier to wrap your data in. Example: `ReactionMenu(ctx, ..., wrap_in_codeblock='py')`
+| `custom_embed` | `discord.Embed` | `None` | `ReactionMenu.TypeEmbedDynamic` | Embed object to use when adding data with `ReactionMenu.add_row()`. Used for styling purposes
+| `delete_on_timeout` | `bool` | `False` | `All menu types` | Delete the menu when it times out
+| `clear_reactions_after` | `bool` | `True` | `All menu types` | delete all reactions after the menu times out
+| `navigation_speed` | `str` | `ReactionMenu.NORMAL` | `All menu types` | Sets if the user needs to wait for the reaction to be removed by the bot before "turning" the page. Setting the speed to `ReactionMenu.FAST` makes it so that there is no need to wait (reactions are not removed on each press) and can navigate lengthy menu's more quickly
+| `only_roles` | `List[discord.Role]` | `None` | `All menu types` | If set, only members with any of the given roles are allowed to control the menu. The menu owner can always control the menu
+| `timeout` | `Union[int, float, None]` | `60.0` | `All menu types` | The timer for when the menu times out. Can be `None` for no timeout
+| `show_page_director` | `bool` | `True` | `All menu types` | Shown at the bottom of each embed page. "Page 1/20"
+| `name` | `str` | `None` | `All menu types` | A name you can set for the menu
+| `style` | `str` | `"Page $/&"` | `All menu types` | A custom page director style you can select. "$" represents the current page, "&" represents the total amount of pages. Example: `ReactionMenu(ctx, ..., style='On $ out of &')`
+| `all_can_click` | `bool` | `False` | `All menu types` | Sets if everyone is allowed to control when pages are 'turned' when buttons are clicked
+| `delete_interactions` | `bool` | `True` | `All menu types` | Delete the prompt message by the bot and response message by the user when asked what page they would like to go to when using `ReactionButton.Type.GO_TO_PAGE`
+| `rows_requested` | `int` | `None` | `ReactionMenu.TypeEmbedDynamic` | The amount of information per `ReactionMenu.add_row()` you would like applied to each embed page
+| `remove_extra_emojis` | `bool` | `False` | `All menu types` | If `True`, all emojis (reactions) added to the menu message that were not originally added to the menu will be removed
+---
+
+### Pages for ReactionMenu
+Depending on the `menu_type`, pages can either be a `str`, `discord.Embed`, or a combination of `content` and `files` ([example below](#stacked-pages))
+* If the `menu_type` is `ReactionMenu.TypeEmbed`, use embeds
+* If the `menu_type` is `ReactionMenu.TypeText` (text only menu) or `ReactionMenu.TypeEmbedDynamic` (embed only menu), use strings.
+* Associated methods
+  * `ReactionMenu.add_page(embed: discord.Embed=MISSING, content: Optional[str]=None, files: Optional[Sequence[discord.File]]=None)`
+  * `ReactionMenu.add_pages(pages: Sequence[Union[discord.Embed, str]])`
+  * `ReactionMenu.add_row(data: str)`
+  * `ReactionMenu.remove_all_pages()`
+  * `ReactionMenu.clear_all_row_data()`
+  * `ReactionMenu.remove_page(page_number: int)`
+  * `ReactionMenu.set_main_pages(*embeds: Embed)`
+  * `ReactionMenu.set_last_pages(*embeds: Embed)`
+
+
+#### Adding Pages
+```py
+# ReactionMenu.TypeEmbed
+menu = ReactionMenu(method, menu_type=ReactionMenu.TypeEmbed)
+menu.add_page(summer_embed)
+menu.add_page(winter_embed)
+
+# ReactionMenu.TypeText
+menu = ReactionMenu(method, menu_type=ReactionMenu.TypeText)
+menu.add_page(content='Its so hot!')
+menu.add_page(content='Its so cold!')
+```
+
+#### ReactionMenu.TypeText
+A `TypeText` menu is a text based pagination menu. No embeds are involved in the pagination process, only plain text is used.
+
+![showcase-text](https://cdn.discordapp.com/attachments/655186216060321816/929172629947027466/text_showcase.gif)
+
+#### Stacked Pages
+With `v3.1.0+`, you can paginate with more than just an embed or text. You can combine text, embeds, as well as files. But depending on the `menu_type` the combination can be restricted. Here is an example of a menu with a `menu_type` of `TypeEmbed` that is stacked.
+
+```py
+# You can use regular commands as well
+@bot.tree.command(description="These are stacked pages", guild=discord.Object(id=...))
+async def stacked(interaction: discord.Interaction):
+    menu = ReactionMenu(interaction, menu_type=ReactionMenu.TypeEmbed)
+
+    menu.add_page(discord.Embed(title="My Embed"), content="This content is stacked on top of a file", files=[discord.File("stacked.py")])
+    menu.add_page(discord.Embed(title="Hey Wumpos, can you say hi to the person reading this? 😃"))
+    menu.add_page(discord.Embed(title="Hi, I'm Wumpos!"), files=[discord.File("wumpos.gif")])
+    
+    menu.add_button(ReactionButton.back())
+    menu.add_button(ReactionButton.next())
+    
+    await menu.start()
+```
+![stacked](https://cdn.discordapp.com/attachments/655186216060321816/955966821268332554/stacked.gif)
+
+Since the `menu_type` is `TypeEmbed`, there always has to be an embed on each page. If the `menu_type` was `TypeText`, embeds aren't allowed and you will be restricted to only using the `files` parameter.
+
+#### ReactionMenu.TypeEmbedDynamic
+A dynamic menu is used when you do not know how much information will be applied to the menu. For example, if you were to request information from a database, that information can always change. You query something and you might get 1,500 results back, and the next maybe only 800. A dynamic menu pieces all this information together for you and adds it to an embed page by rows of data. `ReactionMenu.add_row()` is best used in some sort of `Iterable` where everything can be looped through, but only add the amount of data you want to the menu page.
+> **NOTE:** In a dynamic menu, all added data is placed in the description section of an embed. If you choose to use a `custom_embed`, all text in the description will be overridden with the data you add
+* Associated methods
+    * `ReactionMenu.add_row(data: str)`
+    * `ReactionMenu.clear_all_row_data()`
+    * `ReactionMenu.set_main_pages(*embeds: Embed)`
+    * `ReactionMenu.set_last_pages(*embeds: Embed)`
+* The kwargs specifically made for a dynamic menu are:
+    * `rows_requested` - The amount of rows you would like on each embed page before making a new page
+        * `ReactionMenu(..., rows_requested=5)`
+    * `custom_embed` - An embed you have created to use as the embed pages. Used for your menu aesthetic
+        * `ReactionMenu(..., custom_embed=red_embed)`
+    * `wrap_in_codeblock` - The language identifier when wrapping your data in a discord codeblock. 
+        * `ReactionMenu(..., wrap_in_codeblock='py')`
+
+##### Adding Rows/data
+```py
+menu = ReactionMenu(ctx, menu_type=ReactionMenu.TypeEmbedDynamic, rows_requested=5)
+
+for data in database.request('SELECT * FROM customers'):
+    menu.add_row(data)
+```
+##### Deleting Data
+You can remove all the data you've added to a menu by using `menu.clear_all_row_data()`
+
+##### Main/Last Pages
+When using a dynamic menu, the only embed pages you see are from the data you've added. But if you would like to show more pages other than just the data, you can use methods `ReactionMenu.set_main_pages()` and `ReactionMenu.set_last_pages()`. Setting the main page(s), the embeds you set will be the first embeds that are shown when the menu starts. Setting the last page(s) are the last embeds shown
+```py
+menu.set_main_pages(welcome_embed, announcement_embed)
+
+for data in get_information():
+    menu.add_row(data)
+
+menu.set_last_pages(additional_info_embed)
+# NOTE: setting main/last pages can be set in any order
+```
+
+### ReactionButtons and ButtonTypes
+Buttons/button types are used when you want to add a reaction to the menu that does a certain function. Buttons and button types work together to achieve the desired action.
+```
+class reactionmenu.ReactionButton(*, emoji: str, linked_to: ButtonType, **kwargs)
+```
+### Parameters of the ReactionButton constructor
+* `emoji` (`str`) The emoji you would like to use as the reaction
+* `linked_to` (`ReactionButton.Type`) When the reaction is pressed, this is what determines what it will do
+
+### Kwargs of the ReactionButton constructor
+| Name | Type | Default Value | Used for
+|------|------|---------------|----------
+| `embed` | `discord.Embed` | `None` | When the reaction is pressed, go to the specified embed
+| `name` | `str` | `None` | The name of the button
+| `details` | [info below](#reactionbuttons-with-reactionbuttontypecaller) | `None` | Assigns the function and it's arguments to call when a `ReactionButton` with `ReactionButton.Type.CALLER` is pressed
+| `event` | `ReactionButton.Event` | `None` | Determine when a button should be removed depending on how many times it has been pressed
+| `skip` | `ReactionButton.Skip` | `None` | Set the action and the amount of pages to skip when using a `linked_to` of `ReactionButton.Type.SKIP`. For example using this button type, setting the action to "+" and the amount 3. If you are on "Page 1/20", pressing that button will bring you to "Page 4/20"
+
+### Attributes for ReactionButton
+| Property | Return Type | Info
+|----------|-------------|------
+| `clicked_by` | `Set[discord.Member]` | The members who clicked the button
+| `total_clicks` | `int` | Amount of clicks from the button
+| `last_clicked` | `Optional[datetime.datetime]` | The time in UTC for when the button was last clicked
+| `menu` | `Optional[ReactionMenu]` | The menu the button is attached to
+
+* Associated methods
+    * `ReactionMenu.add_button(button: ReactionButton)`
+    * `ReactionMenu.remove_all_buttons()`
+    * `ReactionMenu.remove_button(button: ReactionButton)`
+    * `ReactionMenu.get_button(identity: Union[str, int], *, search_by='name')`
+    * `ReactionButton.set_caller_details(func: Callable[..., None], *args, **kwargs)`
+
+
+### All ButtonTypes
+| Type | Info |
+|-------|------|
+| `ReactionButton.Type.NEXT_PAGE` | Go to the next page in the menu session
+| `ReactionButton.Type.PREVIOUS_PAGE` | Go to the previous page in the menu session
+| `ReactionButton.Type.GO_TO_FIRST_PAGE` | Go to the first page in the menu session
+| `ReactionButton.Type.GO_TO_LAST_PAGE` | Go to the last page in the menu session
+| `ReactionButton.Type.GO_TO_PAGE` | Prompts you to type in the page you'd like to go to
+| `ReactionButton.Type.END_SESSION` | Stops the session and deletes the menu message
+| `ReactionButton.Type.CUSTOM_EMBED` | Used separately from the navigation buttons. Once pressed, go to the specified embed 
+| `ReactionButton.Type.CALLER` | Used when specifying the function to call and it's arguments when the button is pressed
+| `ReactionButton.Type.SKIP` | Used to paginate through multiple pages in a single button press
+
+
+### Adding Buttons
+You can add buttons (reactions) to the menu using a `ReactionButton`. Below are examples on how to use each `ButtonType`. 
+> **NOTE:** ReactionButtons with `ReactionButton.Type.CALLER` are a little different, so there is a dedicated section explaining how they work and how to implement them further below
+
+```py
+menu = ReactionMenu(...)
+
+# first and last pages
+fpb = ReactionButton(emoji='⏪', linked_to=ReactionButton.Type.GO_TO_FIRST_PAGE)
+lpb = ReactionButton(emoji='⏩', linked_to=ReactionButton.Type.GO_TO_LAST_PAGE)
+
+# go to page
+gtpb = ReactionButton(emoji='🔢', linked_to=ReactionButton.Type.GO_TO_PAGE)
+
+# end session
+esb = ReactionButton(emoji='⏹️', linked_to=ReactionButton.Type.END_SESSION)
+
+# custom embed
+ceb = ReactionButton(emoji='😎', linked_to=ReactionButton.Type.CUSTOM_EMBED, embed=discord.Embed(title='Hello'))
+
+# skip button
+sb = ReactionButton(emoji='5️⃣', linked_to=ReactionButton.Type.SKIP, skip=ReactionButton.Skip(action='+', amount=5))
+
+menu.add_button(fpb)
+...
+```
+### Deleting Buttons
+Remove all buttons with `menu.remove_all_buttons()`. You can also remove an individual button using its name if you have it set, or the button object itself with `menu.remove_button()`
+
+### ReactionButtons with ReactionButton.Type.CALLER
+`ReactionButton.Type.CALLER` buttons are used to implement your own functionality into the menu. Maybe you want to add a button that creates a text channel, sends a message, or add something to a database, whatever it may be. In order to work with `ReactionButton.Type.CALLER`, use the class method below.
+
+* `ReactionButton.set_caller_details(func: Callable[..., None], *args, **kwargs)`
+  
+This class method is used to setup a function and it's arguments that are later called when the button is pressed. The `ReactionButton` constructor has the kwarg `details`, and that's what you'll use with `.set_caller_details()` to assign the values needed. Some examples are below on how to properly implement `ReactionButton.Type.CALLER`
+
+```py
+@bot.command()
+async def user(ctx, name, *, message):
+    await ctx.send(f"Hi {name}! {message}. We're glad you're here!")
+
+def car(year, make, model):
+    print(f"I have a {year} {make} {model}")
+
+ub = ReactionButton(emoji='👋', linked_to=ReactionButton.Type.CALLER, details=ReactionButton.set_caller_details(user, ctx, 'Defxult', message='Welcome to the server'))
+cb = ReactionButton(emoji='🚗', linked_to=ReactionButton.Type.CALLER, details=ReactionButton.set_caller_details(car, 2021, 'Ford', 'Mustang'))
+```
+> **NOTE:** The function you pass in should not return anything. Calling functions with `ReactionButton.Type.CALLER` does not store or handle anything returned by that function
+---
+
+### ReactionButton Methods
+The `ReactionButton` class comes with a set factory methods (class methods) that returns a `ReactionButton` with parameters set according to their `linked_to`.
+
+* `ReactionButton.back()`
+  * `emoji`: "◀️"
+  * `linked_to`: `ReactionButton.Type.PREVIOUS_PAGE`
+* `ReactionButton.next()`
+	* `emoji`: "▶️"
+	* `linked_to`: `ReactionButton.Type.NEXT_PAGE`
+* `ReactionButton.go_to_first_page()`
+	* `emoji`: "⏪"
+	* `linked_to`: `ReactionButton.Type.GO_TO_FIRST_PAGE`
+* `ReactionButton.go_to_last_page()`
+	* `emoji`: "⏩"
+	* `linked_to`: `ReactionButton.Type.GO_TO_LAST_PAGE`
+* `ReactionButton.go_to_page()`
+	* `emoji`: "🔢"
+	* `linked_to`: `ReactionButton.Type.GO_TO_PAGE`
+* `ReactionButton.end_session()`
+	* `emoji`: "⏹️"
+	* `linked_to`: `ReactionButton.Type.END_SESSION`
+* `ReactionButton.all()`
+  * Returns a `list` of `ReactionButton` in the following order
+  * `.go_to_first_page()` `.back()` `.next()` `.go_to_last_page()` `.go_to_page()` `.end_session()`
+* `ReactionButton.generate_skip(emoji: str, action: str, amount: int)`
+  * `emoji`: `<emoji>`
+  * `linked_to`: `ReactionButton.Type.SKIP`
+  * `skip`: `ReactionButton.Skip(<action>, <amount>)`
+
+---
+### Setting Limits
+If you'd like, you can limit the amount of reaction menus that can be active at the same time *per* "guild", "member", or "channel" 
+* Associated CLASS Methods
+    * `ReactionMenu.set_sessions_limit(limit: int, per='guild', message='Too many active menus. Wait for other menus to be finished.')` 
+    * `ReactionMenu.remove_limit()`
+
+Example:
+```py
+@bot.command()
+async def limit(ctx):
+    ReactionMenu.set_sessions_limit(3, per='member', message='Sessions are limited to 3 per member')
+```
+
+With the above example, only 3 menus can be active at once for each member, and if they try to create more before their other menu's are finished, they will get an error message saying "Sessions are limited to 3 per member".
+
+### ReactionButton Events
+You can set a `ReactionButton` to be removed when it has been pressed a certain amount of times
+
+```
+class ReactionButton.Event(event_type: str, value: int)
+```
+
+#### Parameters for ReactionButton.Event
+* `event_type` (`str`) The action to take. The only available option is "remove"
+* `value` (`int`) The amount set for the specified event. Must be >= 1. If value is <= 0, it is implicitly set to 1
+
+Example:
+```py
+menu = ReactionMenu(ctx, ...)
+
+# remove a button after 10 clicks
+button = ReactionButton(..., event=ReactionButton.Event('remove', 10))
+menu.add_button(button)
+```
+> **NOTE:** Not ideal for buttons with a `linked_to` of `ReactionButton.Type.END_SESSION`
+---
+### ReactionMenu Relays
+Menu relays are functions that are called anytime a button that is apart of a menu is pressed. It is considered as an extension of a `ReactionButton` with a `linked_to` of `ReactionButton.Type.CALLER`. Unlike caller buttons which provides no details about the interactions on the menu, relays do.
+* Associated methods
+  * `ReactionMenu.set_relay(func: Callable[[NamedTuple], None], *, only: Optional[List[ReactionButton]]=None)`
+  * `ReactionMenu.remove_relay()`
+
+When creating a function for your relay, that function must contain a single positional argument. When a button is pressed, a `RelayPayload` object (a named tuple) is passed to that function. The attributes of `RelayPayload` are:
+* `member` (`discord.Member`) The person who pressed the button
+* `button` (`ReactionButton`) The button that was pressed
+
+Example:
+```py
+async def enter_giveaway(payload):
+    member = payload.member
+    channel = payload.button.menu.message.channel
+    await channel.send(f"{member.mention}, you've entered the giveaway!")
+
+menu = ReactionMenu(ctx, ...)
+menu.set_relay(enter_giveaway)
+```
+The `set_relay` method comes with the `only` parameter. If that parameter is `None`, all buttons that are pressed will be relayed. You can provide a `list` of buttons to that parameter so only button presses from those specified buttons will be relayed.
+```py
+def example(payload):
+    ...
+
+menu = ReactionMenu(ctx, ...)
+
+back_button = ReactionButton.back()
+next_button = ReactionButton.next()
+
+menu.set_relay(example, only=[back_button])
+```
+
+---
+### Starting/Stopping the ReactionMenu
+* Associated methods
+  * `await ReactionMenu.start(*, send_to=None, reply=False)`
+  * `await ReactionMenu.stop(*, delete_menu_message=False, clear_reactions=False)`
+
+When starting the menu, you have the option to send the menu to a certain channel. Parameter `send_to` is the channel you'd like to send the menu to. You can set `send_to` as the channel name (`str`), channel ID (`int`), or channel object (`discord.TextChannel` / `discord.Thread`). Example:
+```py
+menu = ReactionMenu(...)
+# channel name
+await menu.start(send_to='bot-commands')
+
+# channel ID
+await menu.start(send_to=1234567890123456)
+
+# channel object
+channel = guild.get_channel(1234567890123456)
+await menu.start(send_to=channel)
+
+# there's no need to specify send_to unless you want the menu to be sent to a different channel
+# from the one you're sending the initial message/using the command in. the menu can be started
+# in the current channel by omitting the send_to parameter
+await menu.start()
+```
+> **NOTE:** `send_to` is not valid if a menu was started in DM's
+
+### Full Example
+Here is a basic implementation of `ReactionMenu` that you can copy & paste for a quick demonstration.
+```py
+import asyncio
+import discord
+from discord.ext import commands
+from reactionmenu import ReactionMenu, ReactionButton
+
+bot = commands.Bot(command_prefix='!', intents=discord.Intents.all())
+
+async def start_bot():
+    async with bot:
+        await bot.start('...')
+
+@bot.command()
+async def example(ctx):
+    menu = ReactionMenu(ctx, menu_type=ReactionMenu.TypeEmbed)
+    
+    for member in ctx.guild.members:
+        if member.avatar:
+            embed = discord.Embed(description=f'Joined {member.joined_at.strftime("%b. %d, %Y")}')
+            embed.set_author(name=member.name, icon_url=member.avatar.url)
+            menu.add_page(embed)
+    
+    menu.add_button(ReactionButton.back())
+    menu.add_button(ReactionButton.next())
+    menu.add_button(ReactionButton.end_session())
+    
+    await menu.start()
+
+asyncio.run(start_bot())
+```
+</details>
+
+
+
+
+
+
+
+
+
+
+---
+
+
+
+
+
+
+
+
+
+
+## ViewMenu
+```
+class reactionmenu.ViewMenu(method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs)
+```
+
+A `ViewMenu` is a menu that uses discords Buttons feature. With buttons, you can enable and disable them, set a certain color for them with emojis, have buttons that send hidden messages, and add hyperlinks. This library offers a broader range of functionalities such as who pressed the button, how many times it was pressed and more. It uses views (`discord.ui.View`) to implement the Buttons functionality, but uses some of its own methods in order to make a Button pagination menu simple.
+
+![image](https://cdn.discordapp.com/attachments/655186216060321816/855818139450081280/buttons_showcase_reduced.gif)
+
+<details>
+  <summary><b>Click to show ViewMenu documentation</b></summary>
+
+
+### How to import
+```py
+from reactionmenu import ViewMenu, ViewButton
+```
+---
+
+### Parameters of the ViewMenu constructor
+* `method` (`Union[discord.ext.commands.Context, discord.Interaction]`) A context or interaction object
+* `menu_type` (`MenuType`) The configuration of the menu
+  * `ViewMenu.TypeEmbed`, a normal embed pagination menu
+  * `ViewMenu.TypeEmbedDynamic`, an embed pagination menu with dynamic data
+  * `ViewMenu.TypeText`, a text only pagination menu
+
+---
+### Kwargs of the ViewMenu constructor
+| Name | Type | Default Value | Used for | Info 
+-------|------|---------------|----------|------
+| `wrap_in_codeblock` | `str` | `None` | `ViewMenu.TypeEmbedDynamic` | The discord codeblock language identifier to wrap your data in. Example: `ViewMenu(ctx, ..., wrap_in_codeblock='py')`
+| `custom_embed` | `discord.Embed` | `None` | `ViewMenu.TypeEmbedDynamic` | Embed object to use when adding data with `ViewMenu.add_row()`. Used for styling purposes
+| `delete_on_timeout` | `bool` | `False` | `All menu types` | Delete the menu when it times out
+| `disable_items_on_timeout` | `bool` | `True` | `All menu types` | Disable the items on the menu when the menu times out
+| `remove_items_on_timeout` | `bool` | `False` | `All menu types` | Remove the items on the menu when the menu times out
+| `only_roles` | `List[discord.Role]` | `None` | `All menu types` | If set, only members with any of the given roles are allowed to control the menu. The menu owner can always control the menu
+| `timeout` | `Union[int, float, None]` | `60.0` | `All menu types` | The timer for when the menu times out. Can be `None` for no timeout
+| `show_page_director` | `bool` | `True` | `All menu types` | Shown at the bottom of each embed page. "Page 1/20"
+| `name` | `str` | `None` | `All menu types` | A name you can set for the menu
+| `style` | `str` | `"Page $/&"` | `All menu types` | A custom page director style you can select. "$" represents the current page, "&" represents the total amount of pages. Example: `ViewMenu(ctx, ..., style='On $ out of &')`
+| `all_can_click` | `bool` | `False` | `All menu types` | Sets if everyone is allowed to control when pages are 'turned' when buttons are clicked
+| `delete_interactions` | `bool` | `True` | `All menu types` | Delete the prompt message by the bot and response message by the user when asked what page they would like to go to when using `ViewButton.ID_GO_TO_PAGE`
+| `rows_requested` | `int` | `None` | `ViewMenu.TypeEmbedDynamic` | The amount of information per `ViewMenu.add_row()` you would like applied to each embed page
+---
+
+### Pages for ViewMenu
+Depending on the `menu_type`, pages can either be a `str`, `discord.Embed`, or a combination of `content` or `files` ([example below](#stacked-pages-1))
+* If the `menu_type` is `ViewMenu.TypeEmbed`, use embeds
+* If the `menu_type` is `ViewMenu.TypeText` (text only menu) or `ViewMenu.TypeEmbedDynamic` (embed only menu), use strings.
+* Associated methods
+  * `ViewMenu.add_page(embed: discord.Embed=MISSING, content: Optional[str]=None, files: Optional[Sequence[discord.File]]=None)`
+  * `ViewMenu.add_pages(pages: Sequence[Union[discord.Embed, str]])`
+  * `ViewMenu.add_row(data: str)`
+  * `ViewMenu.remove_all_pages()`
+  * `ViewMenu.clear_all_row_data()`
+  * `ViewMenu.remove_page(page_number: int)`
+  * `ViewMenu.set_main_pages(*embeds: Embed)`
+  * `ViewMenu.set_last_pages(*embeds: Embed)`
+
+#### Adding Pages
+```py
+# ViewMenu.TypeEmbed
+menu = ViewMenu(method, menu_type=ViewMenu.TypeEmbed)
+menu.add_page(summer_embed)
+menu.add_page(winter_embed)
+
+# ViewMenu.TypeText
+menu = ViewMenu(method, menu_type=ViewMenu.TypeText)
+menu.add_page(content='Its so hot!')
+menu.add_page(content='Its so cold!')
+```
+
+#### ViewMenu.TypeText
+A `TypeText` menu is a text based pagination menu. No embeds are involved in the pagination process, only plain text is used.
+
+![text_view_showcase](https://cdn.discordapp.com/attachments/655186216060321816/929744985656549386/text_view_showcase.gif)
+
+#### Stacked Pages
+With `v3.1.0+`, you can paginate with more than just an embed or text. You can combine text, embeds, as well as files. But depending on the `menu_type` the combination can be restricted. Here is an example of a menu with a `menu_type` of `TypeEmbed` that is stacked.
+
+```py
+# You can use regular commands as well
+@bot.tree.command(description="These are stacked pages", guild=discord.Object(id=...))
+async def stacked(interaction: discord.Interaction):
+    menu = ViewMenu(interaction, menu_type=ViewMenu.TypeEmbed)
+
+    menu.add_page(discord.Embed(title="My Embed"), content="This content is stacked on top of a file", files=[discord.File("stacked.py")])
+    menu.add_page(discord.Embed(title="Hey Wumpos, can you say hi to the person reading this? 😃"))
+    menu.add_page(discord.Embed(title="Hi, I'm Wumpos!"), files=[discord.File("wumpos.gif")])
+    
+    menu.add_button(ViewButton.back())
+    menu.add_button(ViewButton.next())
+    
+    await menu.start()
+```
+![stacked_view](https://cdn.discordapp.com/attachments/655186216060321816/955983620038860910/stacked_view.gif)
+
+Since the `menu_type` is `TypeEmbed`, there always has to be an embed on each page. If the `menu_type` was `TypeText`, embeds aren't allowed and you will be restricted to only using the `files` parameter.
+
+#### ViewMenu.TypeEmbedDynamic
+A dynamic menu is used when you do not know how much information will be applied to the menu. For example, if you were to request information from a database, that information can always change. You query something and you might get 1,500 results back, and the next maybe only 800. A dynamic menu pieces all this information together for you and adds it to an embed page by rows of data. `ViewMenu.add_row()` is best used in some sort of `Iterable` where everything can be looped through, but only add the amount of data you want to the menu page.
+> **NOTE:** In a dynamic menu, all added data is placed in the description section of an embed. If you choose to use a `custom_embed`, all text in the description will be overridden with the data you add
+* Associated methods
+    * `ViewMenu.add_row(data: str)`
+    * `ViewMenu.clear_all_row_data()`
+    * `ViewMenu.set_main_pages(*embeds: Embed)`
+    * `ViewMenu.set_last_pages(*embeds: Embed)`
+* The kwargs specifically made for a dynamic menu are:
+    * `rows_requested` - The amount of rows you would like on each embed page before making a new page
+        * `ViewMenu(..., rows_requested=5)`
+    * `custom_embed` - An embed you have created to use as the embed pages. Used for your menu aesthetic
+        * `ViewMenu(..., custom_embed=red_embed)`
+    * `wrap_in_codeblock` - The language identifier when wrapping your data in a discord codeblock. 
+        * `ViewMenu(..., wrap_in_codeblock='py')`
+
+##### Adding Rows/data
+```py
+menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbedDynamic, rows_requested=5)
+
+for data in database.request('SELECT * FROM customers'):
+    menu.add_row(data)
+```
+##### Deleting Data
+You can remove all the data you've added to a menu by using `menu.clear_all_row_data()`
+
+##### Main/Last Pages
+When using a dynamic menu, the only embed pages you see are from the data you've added. But if you would like to show more pages other than just the data, you can use methods `ViewMenu.set_main_pages()` and `ViewMenu.set_last_pages()`. Setting the main page(s), the embeds you set will be the first embeds that are shown when the menu starts. Setting the last page(s) are the last embeds shown
+```py
+menu.set_main_pages(welcome_embed, announcement_embed)
+
+for data in get_information():
+    menu.add_row(data)
+
+menu.set_last_pages(additional_info_embed)
+# NOTE: setting main/last pages can be set in any order
+```
+
+### Buttons for ViewMenu
+Buttons are what you use to interact with the menu. Unlike reactions, they look cleaner, provides less rate limit issues, and offer more in terms of interactions. Enable and disable buttons, use markdown hyperlinks in it's messages, and even send hidden messages.
+
+![discord_buttons](https://discord.com/assets/7bb017ce52cfd6575e21c058feb3883b.png)
+
+
+* Associated methods
+  * `ViewMenu.add_button(button: ViewButton)`
+  * `ViewMenu.disable_all_buttons()`
+  * `ViewMenu.disable_button(button: ViewButton)`
+  * `ViewMenu.enable_all_buttons()`
+  * `ViewMenu.enable_button(button: ViewButton)`
+  * `ViewMenu.get_button(identity: str, *, search_by='label')`
+  * `ViewMenu.remove_all_buttons()`
+  * `ViewMenu.remove_button(button: ViewButton)`
+  * `await ViewMenu.refresh_menu_items()`
+
+#### ViewButton
+```
+class reactionmenu.ViewButton(*, style=discord.ButtonStyle.secondary, label=None, disabled=False, custom_id=None, url=None, emoji=None, followup=None, event=None, **kwargs)
+```
+
+A `ViewButton` is a class that represents the discord button. It is a subclass of `discord.ui.Button`.
+
+The following are the rules set by Discord for Buttons:
+* Link buttons don't send interactions to the Discord App, so link button statistics (it's properties) are not tracked
+* Non-link buttons **must** have a `custom_id`, and cannot have a `url`
+* Link buttons **must** have a `url`, and cannot have a `custom_id`
+* There cannot be more than 25 buttons per message
+---
+#### Parameters of the ViewButton constructor
+* `style` (`discord.ButtonStyle`) The button style
+* `label` (`str`) The text on the button
+* `custom_id` (`str`) An ID to determine what action that button should take. Available IDs:
+  * `ViewButton.ID_NEXT_PAGE`
+  * `ViewButton.ID_PREVIOUS_PAGE`
+  * `ViewButton.ID_GO_TO_FIRST_PAGE` 
+  * `ViewButton.ID_GO_TO_LAST_PAGE`
+  * `ViewButton.ID_GO_TO_PAGE`
+  * `ViewButton.ID_END_SESSION`
+  * `ViewButton.ID_CALLER`
+  * `ViewButton.ID_SEND_MESSAGE`
+  * `ViewButton.ID_CUSTOM_EMBED`
+  * `ViewButton.ID_SKIP`
+* `emoji` (`Union[str, discord.PartialEmoji]`) Emoji used for the button
+  * `ViewButton(..., emoji='😄')` 
+  * `ViewButton(..., emoji='<:miscTwitter:705423192818450453>')`
+  * `ViewButton(..., emoji='\U000027a1')`
+  * `ViewButton(..., emoji='\N{winking face}')`
+* `url` (`str`) URL for a button with style `discord.ButtonStyle.link`
+* `disabled` (`bool`) If the button should be disabled
+* `followup` (`ViewButton.Followup`) The message sent after the button is pressed. Only available for buttons that have a `custom_id` of `ViewButton.ID_CALLER` or `ViewButton.ID_SEND_MESSAGE`. `ViewButton.Followup` is a class that has parameters similar to `discord.abc.Messageable.send()`, and is used to control if a message is ephemeral, contains a file, embed, tts, etc...
+* `event` (`ViewButton.Event`) Set a button to be disabled or removed when it has been pressed a certain amount of times
+
+#### Kwargs of the ViewButton constructor
+| Name | Type | Default Value | Used for
+|------|------|---------------|----------
+| `name` | `str` | `None` | The name of the button
+| `skip` | `ViewButton.Skip` | `None` | Set the action and the amount of pages to skip when using a `custom_id` of `ViewButton.ID_SKIP`. For example, setting the action to "+" and the amount 3. If you are on "Page 1/20", pressing that button will bring you to "Page 4/20"
+| `persist` | `bool` | `False` | Prevents link buttons from being disabled/removed when the menu times out or is stopped so they can remain clickable
+
+#### Attributes for ViewButton
+| Property | Return Type | Info
+|----------|-------------|------
+| `clicked_by` | `Set[discord.Member]` | The members who clicked the button
+| `total_clicks` | `int` | Amount of clicks from the button
+| `last_clicked` | `Optional[datetime.datetime]` | The time in UTC for when the button was last clicked
+| `menu` | `Optional[ViewMenu]` | The menu the button is attached to
+
+#### Adding a ViewButton
+```py
+from reactionmenu import ViewMenu, ViewButton
+
+menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
+
+# Link button
+link_button = ViewButton(style=discord.ButtonStyle.link, emoji='🌍', label='Link to Google', url='https://google.com')
+menu.add_button(link_button)
+
+# Skip button
+skip = ViewButton(style=discord.ButtonStyle.primary, label='+5', custom_id=ViewButton.ID_SKIP, skip=ViewButton.Skip(action='+', amount=5))
+menu.add_button(skip)
+
+# ViewButton.ID_PREVIOUS_PAGE
+back_button = ViewButton(style=discord.ButtonStyle.primary, label='Back', custom_id=ViewButton.ID_PREVIOUS_PAGE)
+menu.add_button(back_button)
+
+# ViewButton.ID_NEXT_PAGE
+next_button = ViewButton(style=discord.ButtonStyle.secondary, label='Next', custom_id=ViewButton.ID_NEXT_PAGE)
+menu.add_button(next_button)
+
+# All other ViewButton are created the same way as the last 2 EXCEPT
+# 1 - ViewButton.ID_CALLER
+# 2 - ViewButton.ID_SEND_MESSAGE
+# 3 - ViewButton.ID_CUSTOM_EMBED
+
+
+# ViewButton.ID_CALLER
+def say_hello(name: str):
+    print('Hello', name)
+
+call_followup = ViewButton.Followup(details=ViewButton.Followup.set_caller_details(say_hello, 'John'))
+menu.add_button(ViewButton(label='Say hi', custom_id=ViewButton.ID_CALLER, followup=call_followup))
+
+# ViewButton.ID_SEND_MESSAGE
+msg_followup = ViewButton.Followup('This message is hidden!', ephemeral=True)
+menu.add_button(ViewButton(style=discord.ButtonStyle.green, label='Message', custom_id=ViewButton.ID_SEND_MESSAGE, followup=msg_followup))
+
+# ViewButton.ID_CUSTOM_EMBED
+custom_embed_button = ViewButton(style=discord.ButtonStyle.blurple, label='Social Media Info', custom_id=ViewButton.ID_CUSTOM_EMBED, followup=ViewButton.Followup(embed=discord.Embed(...)))
+```
+---
+> **NOTE:** When it comes to buttons with a `custom_id` of `ViewButton.ID_CALLER`, `ViewButton.ID_SEND_MESSAGE`, `ViewButton.ID_CUSTOM_EMBED`, or link buttons, you can add as many as you'd like as long as in total it's 25 buttons or less. For all other button ID's, each menu can only have one.
+
+### Using Selects
+Selects are used when you'd like to categorize information in your menu. Selects can only be used when the menu's `menu_type` is `TypeEmbed`. You should keep in mind that discords limitations on how many menu UI items (rows) can be applied to each message.
+
+![select_showcase](https://cdn.discordapp.com/attachments/655186216060321816/971361708121653268/select_showcase.gif)
+
+* Associated Methods
+  * `ViewMenu.add_select(select: ViewSelect)`
+  * `ViewMenu.remove_select(select: ViewSelect)`
+  * `ViewMenu.remove_all_selects()`
+  * `ViewMenu.disable_select(select: ViewSelect)`
+  * `ViewMenu.disable_all_selects()`
+  * `ViewMenu.enable_select(select: ViewSelect)`
+  * `ViewMenu.enable_all_selects()`
+  * `ViewMenu.get_select(title: Union[str, None])`
+
+Example:
+```py
+from reactionmenu import ViewMenu, ViewSelect, Page
+
+menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
+menu.add_page(discord.Embed(title="A showcase of console video games", color=discord.Color.blurple()))
+
+menu.add_select(ViewSelect(title="Console Video Games", options={
+    discord.SelectOption(label="PlayStation", emoji="<:PlayStation:549638412538478602>") : [
+        Page(embed=discord.Embed(title="Ratchet & Clank", description=..., color=discord.Color.yellow()).set_image(url=...)),
+        Page(embed=discord.Embed(title="God of War", description=..., color=discord.Color.blue()).set_image(url=...))
+    ],
+    discord.SelectOption(label="Xbox", emoji="<:Xbox:501880493285834752>") : [
+        Page(embed=discord.Embed(title="Halo Infinite", description=..., color=discord.Color.green()).set_image(url=...)),
+        Page(embed=discord.Embed(title="Gears of War 4", description=..., color=discord.Color.red()).set_image(url=...))
+    ]
+}))
+
+menu.add_button(ViewButton.back())
+menu.add_button(ViewButton.next())
+await menu.start()
+```
+
+#### Go to page navigation
+You can use this type of select when you'd like to use the UI to select a page to go to.
+
+![goto_showcase](https://cdn.discordapp.com/attachments/655186216060321816/973629631905300501/Discord_6SP5AjoOOM.gif)
+
+* Associated methods
+  * `ViewMenu.add_go_to_select(goto: ViewSelect.GoTo)`
+  * `ViewMenu.enable_go_to_select(goto: ViewSelect.GoTo)`
+  * `ViewMenu.enable_all_go_to_selects()`
+  * `ViewMenu.disable_go_to_select(goto: ViewSelect.GoTo)`
+  * `ViewMenu.disable_all_go_to_selects()`
+  * `ViewMenu.remove_go_to_select(goto: ViewSelect.GoTo)`
+  * `ViewMenu.remove_all_go_to_selects()`
+
+The `page_numbers` parameter for `ViewSelect.GoTo` can be used with 3 different types
+
+1. `List[int]` If set to a list of integers, those specified values are the only options that are available when the select is clicked
+   1. `page_numbers=[1, 5, 10]`
+2. `Dict[int, Union[str, discord.Emoji, discord.PartialEmoji]]` You can use this type if you'd like to utilize emojis in your select
+   1. `page_numbers={1 : "🗯️", 2 : "📺"}`
+3. `ellipsis` You can set a *literal* ellipsis to have the library automatically assign all page numbers to the amount of pages that you've added to the menu. This can come in handy if you have 25 pages or less
+   1. `page_numbers=...`
+> **NOTE**: Setting the `page_numbers` parameter to an ellipsis (...) only works as intended if you've added the go to select AFTER you've added pages to the menu
+
+```py
+@bot.command()
+async def navigate(ctx):
+    menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
+
+    menu.add_page(discord.Embed(title="Twitter").set_image(url="..."))
+    menu.add_page(discord.Embed(title="YouTube").set_image(url="..."))
+    menu.add_page(discord.Embed(title="Discord").set_image(url="..."))
+    # ...
+    
+    menu.add_go_to_select(ViewSelect.GoTo(title="Go to page...", page_numbers=...))
+
+    menu.add_button(ViewButton.back())
+    menu.add_button(ViewButton.next())
+
+    await menu.start()
+```
+
+### Updating ViewButton and Pages
+* Associated methods
+  * `await ViewMenu.refresh_menu_items()`
+  * `await ViewMenu.update(*, new_pages: Union[List[Union[Embed, str]], None], new_buttons: Union[List[ViewButton], None])`
+
+When the menu is running, you can update the pages or buttons on the menu. Using `ViewMenu.update()`, you can replace the pages and buttons. Using `ViewMenu.refresh_menu_items()` updates the buttons you have changed.
+
+#### Updating a Button
+```py
+@bot.command()
+async def menu(ctx):
+    menu = ViewMenu(..., name='test')
+    link_button = ViewButton(..., label='Link')
+    
+    menu.add_button(link_button)
+    menu.add_page(...)
+
+    await menu.start()
+
+
+@bot.command()
+async def disable(ctx):
+    menu = ViewMenu.get_session('test')
+    link_button = menu[0].get_button('Link', search_by='label')
+    
+    menu.disable_button(link_button)
+    await menu.refresh_menu_items()
+```
+If the buttons are not refreshed with `ViewMenu.refresh_menu_items()`, the menu will not be updated when changing a button.
+
+#### Updating Pages and Buttons
+Method `ViewMenu.update(...)` is used when you want to replace all or a few of the buttons on the menu. 
+```py
+menu = ViewMenu(...)
+
+# in a different .command()
+await menu.update(new_pages=[hello_embed, goodbye_embed], new_buttons=[link_button, next_button])
+```
+
+> **NOTE**: When using `ViewMenu.update(...)`, there is no need to use `ViewMenu.refresh_menu_items()` because they are updated during the update call. 
+
+---
+#### ViewButton Methods
+The `ViewButton` class comes with a set factory methods (class methods) that returns a `ViewButton` with parameters set according to their `custom_id` (excluding link buttons).
+
+* `ViewButton.link(label: str, url: str)`
+  * `style`: `discord.ButtonStyle.link`
+  * `label`: `<label>`
+  * `url`: `<url>`
+* `ViewButton.back()`
+  * `style`: `discord.ButtonStyle.gray`
+  * `label`: "Back"
+  * `custom_id`: `ViewButton.ID_PREVIOUS_PAGE`
+* `ViewButton.next()`
+	* `style`: `discord.ButtonStyle.gray`
+	* `label`: "Next"
+	* `custom_id`: `ViewButton.ID_NEXT_PAGE`
+* `ViewButton.go_to_first_page()`
+	* `style`: `discord.ButtonStyle.gray`
+	* `label`: "First Page"
+	* `custom_id`: `ViewButton.ID_GO_TO_FIRST_PAGE`
+* `ViewButton.go_to_last_page()`
+	* `style`: `discord.ButtonStyle.gray`
+	* `label`: "Last Page"
+	* `custom_id`: `ViewButton.ID_GO_TO_LAST_PAGE`
+* `ViewButton.go_to_page()`
+	* `style`: `discord.ButtonStyle.gray`
+	* `label`: "Page Selection"
+	* `custom_id`: `ViewButton.ID_GO_TO_PAGE`
+* `ViewButton.end_session()`
+	* style: `discord.ButtonStyle.gray`
+	* label: "Close"
+	* custom_id: `ViewButton.ID_END_SESSION`
+* `ViewButton.all()`
+  * Returns a `list` of `ViewButton` in the following order
+  * `.go_to_first_page()` `.back()` `.next()` `.go_to_last_page()` `.go_to_page()` `.end_session()`
+* `ViewButton.all_with_emojis()`
+  * Returns a `list` of `ViewButton` with their `emoji` parameters already set in the following order
+  * `.go_to_first_page()` `.back()` `.next()` `.go_to_last_page()` `.go_to_page()` `.end_session()`
+* `ViewButton.generate_skip(label: str, action: str, amount: int)`
+  * `style`: `discord.ButtonStyle.gray`
+  * `label`: `<label>`
+  * `custom_id`: `ViewButton.ID_SKIP`
+  * `skip`: `ViewButton.Skip(<action>, <amount>)`
+
+```py
+menu = ViewMenu(ctx, ...)
+menu.add_page(...)
+menu.add_page(...)
+
+menu.add_button(ViewButton.back())
+menu.add_button(ViewButton.next())
+
+await menu.start()
+```
+---
+### ViewButton Events
+You can set a `ViewButton` to be disabled or removed when it has been pressed a certain amount of times
+
+```
+class ViewButton.Event(event_type: str, value: int)
+```
+
+#### Parameters for ViewButton.Event
+* `event_type` (`str`) The action to take. Can either be "disable" or "remove"
+* `value` (`int`) The amount set for the specified event. Must be >= 1. If value is <= 0, it is implicitly set to 1
+
+Example:
+```py
+menu = ViewMenu(ctx, ...)
+
+# disable a button after 5 clicks
+button_1 = ViewButton(..., event=ViewButton.Event('disable', 5))
+menu.add_button(button_1)
+
+# remove a button after 10 clicks
+button_2 = ViewButton(..., event=ViewButton.Event('remove', 10))
+menu.add_button(button_2)
+```
+> **NOTE:** Not valid for link buttons. Also not ideal for buttons with a `custom_id` of `ViewButton.ID_END_SESSION`
+---
+### ViewMenu Relays
+Menu relays are functions that are called anytime a button that is apart of a menu is pressed. It is considered as an extension of a `ViewButton` with an ID of `ViewButton.ID_CALLER`. Unlike caller buttons which provides no details about the interactions on the menu, relays do.
+* Associated methods
+  * `ViewMenu.set_relay(func: Callable[[NamedTuple], None], *, only: Optional[List[ViewButton]]=None)`
+  * `ViewMenu.remove_relay()`
+
+When creating a function for your relay, that function must contain a single positional argument. When a button is pressed, a `RelayPayload` object (a named tuple) is passed to that function. The attributes of `RelayPayload` are:
+* `member` (`discord.Member`) The person who pressed the button
+* `button` (`ViewButton`) The button that was pressed
+
+Example:
+```py
+async def enter_giveaway(payload):
+    member = payload.member
+    channel = payload.button.menu.message.channel
+    await channel.send(f"{member.mention}, you've entered the giveaway!")
+
+menu = ViewMenu(ctx, ...)
+menu.set_relay(enter_giveaway)
+```
+The `set_relay` method comes with the `only` parameter. If that parameter is `None`, all buttons that are pressed will be relayed (except link buttons because they don't send interaction events). You can provide a `list` of buttons to that parameter so only button presses from those specified buttons will be relayed.
+```py
+def example(payload):
+    ...
+
+menu = ViewMenu(ctx, ...)
+
+back_button = ViewButton.back()
+next_button = ViewButton.next()
+
+menu.set_relay(example, only=[back_button])
+```
+
+---
+### Starting/Stopping the ViewMenu
+* Associated methods
+  * `await ViewMenu.start(*, send_to=None, reply=False)`
+  * `await ViewMenu.stop(*, delete_menu_message=False, remove_buttons=False, disable_buttons=False)`
+
+When starting the menu, you have the option to send the menu to a certain channel. Parameter `send_to` is the channel you'd like to send the menu to. You can set `send_to` as the channel name (`str`), channel ID (`int`), or channel object (`discord.TextChannel` / `discord.Thread`). Example:
+```py
+menu = ViewMenu(...)
+# channel name
+await menu.start(send_to='bot-commands')
+
+# channel ID
+await menu.start(send_to=1234567890123456)
+
+# channel object
+channel = guild.get_channel(1234567890123456)
+await menu.start(send_to=channel)
+
+# there's no need to specify send_to unless you want the menu to be sent to a different channel
+# from the one you're sending the initial message/using the command in. the menu can be started
+# in the current channel by omitting the send_to parameter
+await menu.start()
+```
+> **NOTE:** `send_to` is not valid if a menu was started in DM's
+
+Only one option is available when stopping the menu. If you have multiple parameters as `True`, only one will execute
+- `delete_menu_message` > `disable_buttons`
+- `disable_buttons` > `remove_buttons`
+---
+
+### Full Example
+Here is a basic implementation of `ViewMenu` that you can copy & paste for a quick demonstration.
+```py
+import asyncio
+import discord
+from discord.ext import commands
+from reactionmenu import ViewMenu, ViewButton
+
+bot = commands.Bot(command_prefix='!', intents=discord.Intents.all())
+
+async def start_bot():
+    async with bot:
+        await bot.start('...')
+
+@bot.command()
+async def example(ctx):
+    menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
+    
+    for member in ctx.guild.members:
+        if member.avatar:
+            embed = discord.Embed(description=f'Joined {member.joined_at.strftime("%b. %d, %Y")}')
+            embed.set_author(name=member.name, icon_url=member.avatar.url)
+            menu.add_page(embed)
+    
+    menu.add_button(ViewButton.back())
+    menu.add_button(ViewButton.next())
+    menu.add_button(ViewButton.end_session())
+    
+    await menu.start()
+
+asyncio.run(start_bot())
+```
+</details>
```

### Comparing `reactionmenu-3.1.3/reactionmenu/abc.py` & `reactionmenu-3.1.4/reactionmenu/abc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1418 +1,1427 @@
-"""
-MIT License
-
-Copyright (c) 2021-present Defxult#8269
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
-DEALINGS IN THE SOFTWARE.
-"""
-
-from __future__ import annotations
-
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    ClassVar,
-    Final,
-    Generic,
-    Iterable,
-    List,
-    Literal,
-    Optional,
-    Set,
-    Tuple,
-    TypeVar,
-    Union,
-    overload
-)
-
-if TYPE_CHECKING:
-    from datetime import datetime
-    from typing_extensions import Self
-
-import abc
-import asyncio
-import collections
-import inspect
-import re
-import warnings
-from collections.abc import Sequence
-from enum import Enum, auto
-from typing import NamedTuple, Union
-
-import discord
-from discord.ext.commands import Context
-from discord.utils import MISSING
-
-from .decorators import ensure_not_primed
-from .errors import *
-
-# Constants
-_DYNAMIC_EMBED_LIMIT: Final[int] = 4096
-_DEFAULT_STYLE: Final[str] = 'Page $/&'
-DEFAULT_BUTTONS = None
-DEFAULT = MISSING
-
-GB = TypeVar('GB', bound='_BaseButton')
-M = TypeVar('M', bound='_BaseMenu')
-
-class Page:
-    """Represents a single "page" in the pagination process
-    
-        .. added:: v3.1.0
-    """
-    __slots__ = ("content", "embed", "files", "_go_to")
-    
-    def __init__(self, *, content: Optional[str]=None, embed: Optional[discord.Embed]=MISSING, files: Optional[List[discord.File]]=MISSING) -> None:
-        self.content = content
-        self.embed = embed
-        self.files = files
-        self._go_to: Optional[int] = None
-    
-    def __repr__(self) -> str:
-        return f"<Page {' '.join([f'{attr_name}={getattr(self, attr_name)!r}' for attr_name in self.__class__.__slots__ if type(getattr(self, attr_name)) not in (type(None), type(MISSING))])}>"
-    
-    def _shallow(self) -> Self:
-        from copy import copy
-        return copy(self)
-
-class PaginationEmojis:
-    """A set of basic emojis for your convenience to use for your buttons emoji
-    - ◀️ as `BACK_BUTTON`
-    - ▶️ as `NEXT_BUTTON`
-    - ⏪ as `FIRST_PAGE`
-    - ⏩ as `LAST_PAGE`
-    - 🔢 as `GO_TO_PAGE`
-    - ⏹️ as `END_SESSION`
-    """
-    BACK_BUTTON: ClassVar[str] = '◀️'
-    NEXT_BUTTON: ClassVar[str] = '▶️'
-    FIRST_PAGE: ClassVar[str]  = '⏪'
-    LAST_PAGE: ClassVar[str]   = '⏩'
-    GO_TO_PAGE: ClassVar[str]  = '🔢'
-    END_SESSION: ClassVar[str] = '⏹️'
-
-class _PageController:
-    def __init__(self, pages: List[Page]) -> None:
-        self.ALL_PAGES: Final[List[Page]] = pages
-        self.index = 0
-
-    @property
-    def current_page(self) -> Page:
-        return self.ALL_PAGES[self.index]
-    
-    @property
-    def total_pages(self) -> int:
-        """Return the total amount of pages registered to the menu"""
-        return len(self.ALL_PAGES) - 1
-    
-    def validate_index(self) -> Page:
-        """If the index is out of bounds, assign the appropriate values so the pagination process can continue and return the associated page"""
-        try:
-            _ = self.ALL_PAGES[self.index]
-        except IndexError:
-            if self.index > self.total_pages:
-                self.index = 0
-            
-            elif self.index < 0:
-                self.index = self.total_pages
-        finally:
-            return self.ALL_PAGES[self.index]
-    
-    def skip_loop(self, action: str, amount: int) -> None:
-        """Using `self.index += amount` does not work because this library is used to operating on a +-1 basis. This loop
-        provides a simple way to still operate on the +-1 standard.
-        """
-        while amount != 0:
-            if action == '+':
-                self.index += 1
-            elif action == '-':
-                self.index -= 1
-            
-            self.validate_index()
-            amount -= 1
-    
-    def skip(self, skip: _BaseButton.Skip) -> Page:
-        """Return the page that the skip value was set to"""
-        self.skip_loop(skip.action, skip.amount)
-        return self.validate_index()
-
-    def next(self) -> Page:
-        """Return the next page in the pagination process"""
-        self.index += 1
-        return self.validate_index()
-    
-    def prev(self) -> Page:
-        """Return the previous page in the pagination process"""
-        self.index -= 1
-        return self.validate_index()
-    
-    def first_page(self) -> Page:
-        """Return the first page in the pagination process"""
-        self.index = 0
-        return self.ALL_PAGES[self.index]
-
-    def last_page(self) -> Page:
-        """Return the last page in the pagination process"""
-        self.index = self.total_pages
-        return self.ALL_PAGES[self.index]
-
-class _MenuType(Enum):
-    TypeEmbed = auto()
-    TypeEmbedDynamic = auto()
-    TypeText = auto()
-
-MenuType = _MenuType
-
-class _LimitDetails(NamedTuple):
-    limit: int
-    per: str
-    message: str
-    set_by_user: bool = False
-
-    @classmethod
-    def default(cls) -> Self:
-        return cls(0, "", "")
-
-class _BaseButton(Generic[GB], metaclass=abc.ABCMeta):
-
-    Emojis: ClassVar[PaginationEmojis] = PaginationEmojis()
-
-    def __init__(self, name: str, event: Optional[_BaseButton.Event], skip: _BaseButton.Skip):
-        self.name: str = name
-        self.event: Optional[_BaseButton.Event] = event
-        self.skip: _BaseButton.Skip = skip
-        self.__clicked_by = set()
-        self.__total_clicks = 0
-        self.__last_clicked: Optional[datetime] = None
-    
-    @property
-    @abc.abstractmethod
-    def menu(self):
-        raise NotImplementedError
-    
-    @property
-    def clicked_by(self) -> Set[discord.Member]:
-        """
-        Returns
-        -------
-        Set[:class:`discord.Member`]: The members who clicked the button
-        """
-        return self.__clicked_by
-    
-    @property
-    def total_clicks(self) -> int:
-        """
-        Returns
-        -------
-        :class:`int`: The amount of clicks on the button
-        """
-        return self.__total_clicks
-
-    @property
-    def last_clicked(self) -> Optional[datetime]:
-        """
-        Returns
-        -------
-        Optional[:class:`datetime.datetime`]: The time in UTC for when the button was last clicked. Can be :class:`None` if the button has not been clicked
-        """
-        return self.__last_clicked
-
-    def _update_statistics(self, user: Union[discord.Member, discord.User]) -> None:
-        self.__clicked_by.add(user)
-        self.__total_clicks += 1
-        self.__last_clicked = discord.utils.utcnow()
-
-    class Skip:
-        """Initialize a skip button with the appropriate values
-        
-        Parameters
-        ----------
-        action: :class:`str`
-            Whether to go forward in the pagination process ("+") or backwards ("-")
-        
-        amount: :class:`int`
-            The amount of pages to skip. Must be >= 1. If value is <= 0, it is implicitly set to 2
-        """
-        def __init__(self, action: Literal['+', '-'], amount: int):
-            if amount <= 0: amount = 2
-            if action in ('+', '-'):
-                self.action = action
-                self.amount = amount
-            else:
-                raise MenuException('The action given was not recognized. Expected "+" or "-"')
-
-    class Event:
-        """Set a button to be disabled or removed when it has been pressed a certain amount of times. If the button is a :class:`ReactionButton`, only the "remove" event is available
-        
-        Parameters
-        ----------
-        event: :class:`str`
-            The action to take. Can either be "disable" or "remove"
-        
-        value: :class:`int`
-            The amount set for the specified event. Must be >= 1. If value is <= 0, it is implicitly set to 1"""
-        
-        _DISABLE = 'disable'
-        _REMOVE = 'remove'
-
-        def __init__(self, event_type: Literal['disable', 'remove'], value: int):
-            if value <= 0: value = 1
-            event_type = str(event_type).lower() # type: ignore
-            cls = self.__class__
-            
-            if event_type in (cls._DISABLE, cls._REMOVE):
-                self.event_type = event_type
-                self.value = value
-            else:
-                raise MenuException('The value for parameter "event_type" was not recognized')
-
-class _BaseMenu(metaclass=abc.ABCMeta):
-    TypeEmbed: Final[_MenuType] = _MenuType.TypeEmbed
-    TypeEmbedDynamic: Final[_MenuType] = _MenuType.TypeEmbedDynamic
-    TypeText: Final[_MenuType] = _MenuType.TypeText
-
-    _sessions_limit_details = _LimitDetails.default()
-    _active_sessions: List[Self] # initialized in child classes
-
-    def __init__(self, method: Union[Context, discord.Interaction], /, menu_type: _MenuType, **kwargs):
-        self._method = method
-        self._menu_type = menu_type
-
-        self._msg: Union[discord.Message, discord.InteractionMessage] # initialized in child classes
-        self._pc:_PageController # initialized in child classes
-        self._is_running = False
-        self._stop_initiated = False
-        self._page_director_separator = ":"
-
-        # dynamic session
-        self._main_page_contents = collections.deque()
-        self._last_page_contents = collections.deque()
-        self._dynamic_data_builder: List[str] = []
-        self.wrap_in_codeblock: Optional[str] = kwargs.get('wrap_in_codeblock')
-        self.rows_requested: int = kwargs.get('rows_requested', 0)
-        self.custom_embed: Optional[discord.Embed] = kwargs.get('custom_embed')
-
-        self._relay_info: Optional[NamedTuple] = None
-        self._on_timeout_details: Optional[Callable[[_BaseMenu], None]] = None
-        self._menu_timed_out = False
-        self._bypass_primed = False # used in :meth:`update()`
-        self._pages: List[Page] = []
-        self._on_close_event = asyncio.Event() # used for :meth:`wait_until_close()`
-
-        # kwargs
-        self.delete_on_timeout: bool = kwargs.get('delete_on_timeout', False)
-        self.only_roles: Optional[List[discord.Role]] = kwargs.get('only_roles')
-        self.show_page_director: bool = kwargs.get('show_page_director', True)
-        self.name: Optional[str] = kwargs.get('name')
-        self.style: Optional[str] = kwargs.get('style', _DEFAULT_STYLE)
-        self.all_can_click: bool = kwargs.get('all_can_click', False)
-        self.delete_interactions: bool = kwargs.get('delete_interactions', True)
-        self.allowed_mentions: discord.AllowedMentions = kwargs.get('allowed_mentions', discord.AllowedMentions(everyone=False, users=True, roles=False, replied_user=True))
-    
-    @abc.abstractmethod
-    def _handle_event(self):
-        raise NotImplementedError
-    
-    @abc.abstractmethod
-    def remove_all_buttons(self):
-        raise NotImplementedError
-    
-    @abc.abstractmethod
-    def get_button(self):
-        raise NotImplementedError
-    
-    @abc.abstractmethod
-    def remove_button(self):
-        raise NotImplementedError
-    
-    @abc.abstractmethod
-    def add_button(self):
-        raise NotImplementedError
-    
-    @abc.abstractmethod
-    def add_buttons(self):
-        raise NotImplementedError
-    
-    @abc.abstractmethod
-    def _override_dm_settings(self):
-        raise NotImplementedError
-    
-    @abc.abstractmethod
-    def stop(self):
-        raise NotImplementedError
-    
-    @abc.abstractmethod
-    async def start(self):
-        raise NotImplementedError
-    
-    # ABC class methods
-    
-    @abc.abstractclassmethod
-    async def quick_start(cls):
-        raise NotImplementedError
-    
-    @staticmethod
-    def separate(values: Sequence[Any]) -> Tuple[List[discord.Embed], List[str]]:
-        """|static method|
-        
-        Sorts all embeds and strings into a single tuple
-
-        Parameters
-        ----------
-        values: Sequence[`Any`]
-            The values to separate
-        
-        Returns
-        -------
-        Tuple[List[:class:`discord.Embed`], List[:class:`str`]]
-        
-        Example
-        -------
-        >>> embeds, strings = .separate([...])
-        """
-        all_embeds = list(filter(lambda item: isinstance(item, discord.Embed), values))
-        all_strings = list(filter(lambda item: isinstance(item, str), values))
-        return (all_embeds, all_strings)
-    
-    @staticmethod
-    def all_embeds(values: Sequence[Any]) -> bool:
-        """|static method|
-        
-        Tests to see if all items in the sequence are of type :class:`discord.Embed`
-        
-        Parameters
-        ----------
-        values: Sequence[`Any`]
-            The values to test
-        
-        Returns
-        -------
-        :class:`bool`: Can return `False` if the sequence is empty
-        """
-        return all([isinstance(item, discord.Embed) for item in values]) if values else False
-    
-    @staticmethod
-    def _sort_buttons(buttons: List[GB]) -> List[GB]:
-        return sorted(buttons, key=lambda btn: btn.total_clicks, reverse=True)
-    
-    @staticmethod
-    def all_strings(values: Sequence[Any]) -> bool:
-        """|static method|
-        
-        Tests to see if all items in the sequence are of type :class:`str`
-        
-        Parameters
-        ----------
-        values: Sequence[`Any`]
-            The values to test
-        
-        Returns
-        -------
-        :class:`bool`: Can return `False` if the sequence is empty
-        """
-        return all([isinstance(item, str) for item in values]) if values else False
-    
-    @staticmethod #* Don't make this an instance method. It would be better as one, but it's main intended use is for :meth:`_check` in "views_menu.py"
-    def _extract_proper_user(method: Union[Context, discord.Interaction]) -> Union[discord.Member, discord.User]:
-        """|static method| Get the proper :class:`discord.User` / :class:`discord.Member` from the attribute depending on the instance
-
-            .. added v3.1.0
-        """
-        return method.author if isinstance(method, Context) else method.user
-    
-    @classmethod
-    def _quick_check(cls, pages: Sequence[Union[discord.Embed, str]]) -> _MenuType:
-        """|class method| Verification for :meth:`quick_start()`
-        
-            .. added v3.1.0
-        """
-        if cls.all_embeds(pages):  return cls.TypeEmbed
-        if cls.all_strings(pages): return cls.TypeText
-        raise IncorrectType(f'All items in the sequence were not of type discord.Embed or str')
-    
-    @classmethod
-    def _all_menu_types(cls) -> Tuple[_MenuType, _MenuType, _MenuType]:
-        return (cls.TypeEmbed, cls.TypeEmbedDynamic, cls.TypeText)
-    
-    @classmethod
-    def remove_limit(cls) -> None:
-        """|class method|
-        
-        Remove the limits currently set for menu's
-        """
-        cls._sessions_limit_details = _LimitDetails.default()
-    
-    @classmethod
-    def get_all_dm_sessions(cls) -> List[Self]:
-        """|class method|
-        
-        Retrieve all active DM menu sessions
-        
-        Returns
-        -------
-        A :class:`list` of active DM menu sessions that are currently running. Can be an empty list if there are no active DM sessions
-        """
-        return [session for session in cls._active_sessions if session._msg.guild is None] # type: ignore
-    
-    @classmethod
-    def get_all_sessions(cls) -> List[Self]:
-        """|class method|
-        
-        Retrieve all active menu sessions
-        
-        Returns
-        -------
-        A :class:`list` of menu sessions that are currently running. Can be an empty list if there are no active sessions
-        """
-        return cls._active_sessions
-    
-    @classmethod
-    def get_session(cls, name: str) -> List[Self]:
-        """|class method|
-        
-        Get a menu instance by it's name
-        
-        Parameters
-        ----------
-        name: :class:`str`
-            The name of the menu to return
-        
-        Returns
-        -------
-        A :class:`list` of menu sessions that are currently running that match the supplied :param:`name`. Can be an empty list if there are no active sessions that matched the :param:`name`
-        """
-        name = str(name)
-        return [session for session in cls._active_sessions if session.name == name]
-    
-    @classmethod
-    def get_sessions_count(cls) -> int:
-        """|class method|
-        
-        Returns the number of active sessions
-        
-        Returns
-        -------
-        :class:`int`: The amount of menu sessions that are active
-        """
-        return len(cls._active_sessions)
-    
-    @classmethod
-    def set_sessions_limit(cls, limit: int, per: Literal['channel', 'guild', 'member']='guild', message: str='Too many active menus. Wait for other menus to be finished.') -> None:
-        """|class method|
-        
-        Sets the amount of menu sessions that can be active at the same time per guild, channel, or member. This applies to both :class:`ReactionMenu` & :class:`ViewMenu`
-
-        Parameters
-        ----------
-        limit: :class:`int`
-            The amount of menu sessions allowed
-        
-        per: :class:`str`
-            How menu sessions should be limited. Options: "channel", "guild", or "member"
-        
-        message: :class:`str`
-            Message that will be sent informing users about the menu limit when the limit is reached. Can be :class:`None` for no message
-                    
-        Raises
-        ------
-        - `IncorrectType`: The :param:`limit` parameter was not of type :class:`int`
-        - `MenuException`: The value of :param:`per` was not valid or the limit was not greater than or equal to one
-        """
-        if not isinstance(limit, int):
-            raise IncorrectType(f'Parameter "limit" expected int, got {limit.__class__.__name__}')
-        else:
-            if limit <= 0:
-                raise MenuException('The session limit must be greater than or equal to one')
-            
-            per = str(per).lower() # type: ignore
-            if per not in ('guild', 'channel', 'member'):
-                raise MenuException('Parameter value of "per" was not recognized. Expected: "channel", "guild", or "member"')
-
-            cls._sessions_limit_details = _LimitDetails(limit, per, message, set_by_user=True)
-    
-    @classmethod
-    async def stop_session(cls, name: str, include_all: bool=False) -> None:
-        """|coro class method|
-        
-        Stop a specific menu with the supplied name
-        
-        Parameters
-        ----------
-        name: :class:`str`
-            The menus name
-        
-        include_all: :class:`bool`
-            If set to `True`, it stops all menu sessions with the supplied :param:`name`. If `False`, stops only the most recently started menu with the supplied :param:`name`
-        
-        Raises
-        ------
-        - `MenuException`: The session with the supplied name was not found
-        """
-        name = str(name)
-
-        async def determine_include_all(sessions_to_stop: List[Self]) -> None:
-            """|coro| Ensures if :param:`include_all` is `True`, all sessions with the specified name will be stopped"""
-            if sessions_to_stop:
-                if include_all:
-                    for session in sessions_to_stop:
-                        await session.stop()
-                else:
-                    await sessions_to_stop[-1].stop()
-            else:
-                MESSAGE = f'Menu with name {name!r} was not found in the list of active {cls.__name__} sessions'
-                raise MenuException(MESSAGE)
-
-        matched_sessions = [session for session in cls._active_sessions if name == session.name]
-        await determine_include_all(matched_sessions)
-    
-    @classmethod
-    async def stop_all_sessions(cls) -> None:
-        """|coro class method|
-
-        Stops all menu sessions that are currently running
-        """
-        while cls._active_sessions:
-            session = cls._active_sessions[0]
-            await session.stop()
-    
-    @classmethod
-    def get_menu_from_message(cls, message_id: int, /) -> Optional[Self]:
-        """|class method|
-
-        Return the menu object associated with the message with the given ID
-
-        Parameters
-        ----------
-        message_id: :class:`int`
-            The `discord.Message.id` from the menu message
-
-        Returns
-        -------
-        The menu object. Can be :class:`None` if the menu was not found in the list of active menu sessions
-        """
-        for menu in cls._active_sessions:
-            if menu._msg.id == message_id: # type: ignore
-                return menu
-        return None
-
-    @property
-    def rows(self) -> Optional[List[str]]:
-        """
-        Returns
-        -------
-        Optional[List[:class:`str`]]: All rows that's been added to the menu. Can return `None` if the menu has not started or the `menu_type` is not `TypeEmbedDynamic`
-        
-            .. added: v3.1.0
-        """
-        return None if self._is_running is False or self._menu_type != _MenuType.TypeEmbedDynamic else self._dynamic_data_builder.copy()
-    
-    @property
-    def menu_type(self) -> str:
-        """
-        Returns
-        -------
-        :class:`str`: The `menu_type` you set via the constructor. This will either be `TypeEmbed`, `TypeEmbedDynamic`, or `TypeText`
-
-            .. added:: v3.1.0
-        """
-        return self._menu_type.name
-    
-    @property
-    def last_viewed(self) -> Optional[Page]:
-        """
-        Returns
-        -------
-        Optional[:class:`Page`]: The last page that was viewed in the pagination process. Can be :class:`None` if the menu has not been started
-        """
-        return self._pc.current_page._shallow() if self._pc is not None else None
-    
-    @property
-    def owner(self) -> Union[discord.Member, discord.User]:
-        """
-        Returns
-        -------
-        Union[:class:`discord.Member`, :class:`discord.User`]: The owner of the menu (the person that started the menu). If the menu was started in a DM, this will return :class:`discord.User`
-        """
-        return self._extract_proper_user(self._method)
-    
-    @property
-    def total_pages(self) -> int:
-        """
-        Returns
-        -------
-        :class:`int`: The amount of pages that have been added to the menu. If the `menu_type` is :attr:`TypeEmbedDynamic`, the amount of pages is not known until AFTER the menu has started. 
-        If attempted to retrieve the value before a dynamic menu has started, this will return a value of -1
-        """
-        if self._menu_type == _BaseMenu.TypeEmbedDynamic:
-            return len(self._pages) if self._is_running else -1
-        else:
-            return len(self._pages)
-    
-    @property
-    def pages(self) -> Optional[List[Page]]:
-        """
-        Returns
-        -------
-        Optional[List[:class:`Page`]]: The pages currently applied to the menu. Can return :class:`None` if there are no pages
-        
-        Note: If the `menu_type` is :attr:`TypeEmbedDynamic`, the pages aren't known until after the menu has started
-        """
-        return self._pages.copy() if self._pages else None # Return a copy so the core list of pages cannot be manipulated
-
-    @property
-    def message(self) -> Optional[Union[discord.Message, discord.InteractionMessage]]:
-        """
-        Returns
-        -------
-        Optional[Union[:class:`discord.Message`, :class:`discord.InteractionMessage`]]: The menu's message object. Can be :class:`None` if the menu has not been started
-        """
-        return self._msg
-    
-    @property
-    def is_running(self) -> bool:
-        """
-        Returns
-        -------
-        :class:`bool`: `True` if the menu is currently running, `False` otherwise
-        """
-        return self._is_running
-    
-    @property
-    def in_dms(self) -> bool:
-        """
-        Returns
-        -------
-        :class:`bool`: If the menu was started in a DM
-        """
-        return self._method.guild is None
-    
-    def _chunks(self, list_: List[str], n: int) -> Iterable:
-        """Yield successive n-sized chunks from list. Core component of a dynamic menu"""
-        for i in range(0, len(list_), n):
-            yield list_[i:i + n]
-    
-    async def _build_dynamic_pages(self, send_to, view: Optional[discord.ui.View]=None, payload: Optional[dict]=None) -> None:
-        """|coro| Compile all the information that was given via :meth:`add_row`"""
-        for data_clump in self._chunks(self._dynamic_data_builder, self.rows_requested):
-            joined_data = '\n'.join(data_clump)
-            if len(joined_data) <= _DYNAMIC_EMBED_LIMIT:
-                possible_block = f"```{self.wrap_in_codeblock}\n{joined_data}```"
-                embed = discord.Embed() if self.custom_embed is None else self.custom_embed.copy()
-                embed.description = joined_data if not self.wrap_in_codeblock else possible_block
-                self._pages.append(Page(embed=embed))
-            else:
-                raise DescriptionOversized('With the amount of data that was received, the embed description is over discords size limit. Lower the amount of "rows_requested" to solve this problem')
-        else:
-            def convert_to_page(main_last: Iterable[discord.Embed]) -> List[Page]:
-                """Initializing the :class:`deque` only supports :class:`discord.Embed`. This converts those embed objects to the supported :class:`Page` type for proper pagination
-                
-                    .. added:: v3.1.0
-                """
-                return [Page(embed=item) for item in main_last]
-            
-            # set the main/last pages if any
-            if any([self._main_page_contents, self._last_page_contents]):
-                
-                # convert to :class:`deque`
-                self._pages = collections.deque(self._pages) # type: ignore (only temporary to use extend methods of :class:`deque`)
-                
-                if self._main_page_contents:
-                    self._main_page_contents.reverse()
-                    self._pages.extendleft(convert_to_page(self._main_page_contents))
-                
-                if self._last_page_contents:
-                    self._pages.extend(convert_to_page(self._last_page_contents))
-            
-            # convert back to `list`
-            self._pages = list(self._pages)
-
-            self._refresh_page_director_info(_BaseMenu.TypeEmbedDynamic, self._pages)
-            cls = self.__class__
-
-            # make sure data has been added to create at least 1 page
-            if not self._pages: raise NoPages(f'You cannot start a {cls.__name__} when no data has been added')
-            
-            payload['embed'] = self._pages[0].embed # type: ignore / - / reassign the first page to show to director information
-            
-            if view is None:
-                await self._handle_send_to(send_to, payload) # type: ignore
-            else:
-                await self._handle_send_to(send_to, payload) # type: ignore ("embed=" can still be `None`)
-    
-    def _display_timeout_warning(self, error: Exception) -> None:
-        """Simply displays a warning message to the user notifying them an error has occurred in the function they have set for when the menu times out"""
-        warnings.formatwarning = lambda msg, *args, **kwargs: f'{msg}'
-        warnings.warn(inspect.cleandoc(
-            f"""
-            UserWarning: The function you have set in method {self.__class__.__name__}.set_on_timeout() raised an error
-            -> {error.__class__.__name__}: {error}
-            
-            This error has been ignored so the menu timeout process can complete
-            """
-        ))
-    
-    async def _handle_on_timeout(self) -> None:
-        """|coro| Call the function the user has set for when the menu times out"""
-        if self._on_timeout_details and self._menu_timed_out:
-            func = self._on_timeout_details
-            
-            # call the timeout function but ignore any and all exceptions that may occur during the function timeout call.
-            # the most important thing here is to ensure the menu is gracefully stopped while displaying a formatted
-            # error message to the user
-            try:
-                if asyncio.iscoroutinefunction(func):
-                    await func(self) # type: ignore (`iscoroutinefunction` will still return `False` if func is `None` (i want that to happen))
-                else: func(self)
-            except Exception as error:
-                self._display_timeout_warning(error)
-    
-    def _determine_kwargs(self, page: Page) -> dict:
-        """Determine the `inter.response.edit_message()` and :meth:`_msg.edit()` kwargs for the pagination process. Used in :meth:`ViewMenu._paginate()` and :meth:`ReactionMenu._paginate()`"""
-        
-        # create a copy of the files if they are set because once paginated, they are only visible once
-        maybe_new_files = [discord.File(f.filename) for f in page.files] if page.files else [] # type: ignore
-        
-        kwargs = {
-            "content" : page.content, # `content` will always be present because even with TypeEmbed menu's, pagination with the addition of text is possible
-            "allowed_mentions" : self.allowed_mentions,
-            "attachments" : maybe_new_files, # the `edit_message` method for this has an "attachment" kwarg instead of a "files" parameter
-            "allowed_mentions" : self.allowed_mentions
-        }
-
-        # only add the "embed" key if its an embed type menu
-        if self._menu_type in (_BaseMenu.TypeEmbed, _BaseMenu.TypeEmbedDynamic):
-            kwargs["embed"] = page.embed
-        return kwargs
-    
-    def _refresh_page_director_info(self, type_: _MenuType, pages: List[Page]) -> None:
-        """Sets the page count at the bottom of embeds/text if set
-        
-        Parameters
-        ----------
-        type_: :class:`_MenuType`
-            Either :attr:`_BaseMenu.TypeEmbed`, :attr:`_BaseMenu.TypeEmbedDynamic` or :attr:`_BaseMenu.TypeText`
-        
-        pages: List[:class:`Page`]
-            The pagination contents
-        """
-        if self.show_page_director:
-            if type_ not in (_BaseMenu.TypeEmbed, _BaseMenu.TypeEmbedDynamic, _BaseMenu.TypeText):
-                raise Exception('Needs to be of type _BaseMenu.TypeEmbed, _BaseMenu.TypeEmbedDynamic or _BaseMenu.TypeText') 
-            
-            page_number = 1
-
-            if type_ in (_BaseMenu.TypeEmbed, _BaseMenu.TypeEmbedDynamic):
-                page_number = 1
-                OUTOF: Final[int] = len(pages)
-                all_embeds = [p.embed for p in pages]
-                for embed in all_embeds:
-                    embed.set_footer(text=f'{self._maybe_new_style(page_number, OUTOF)}{self._page_director_separator if embed.footer.text else ""} {embed.footer.text if embed.footer.text else ""}', icon_url=embed.footer.icon_url) # type: ignore
-                    page_number += 1
-            else:
-                # TypeText Only
-
-                CODEBLOCK = re.compile(r'(`{3})(.*?)(`{3})', flags=re.DOTALL)
-                CODEBLOCK_DATA_AFTER = re.compile(r'(`{3})(.*?)(`{3}).+', flags=re.DOTALL)
-                for idx in range(len(pages)):
-                    page: Page = pages[idx]
-                    page_info = self._maybe_new_style(page_number, len(pages))
-                    
-                    # the main purpose of the re is to decide if only 1 or 2 '\n' should be used. with codeblocks, at the end of the block there is already a new line, so there's no need to add an extra one except in
-                    # the case where there is more information after the codeblock
-                    
-                    # Note: with codeblocks, i already tried the f doc string version of this and it doesnt work because there is a spacing issue with page_info. using a normal f string with \n works as intended
-                    # f doc string version: https://github.com/Defxult/reactionmenu/blob/eb88af3a2a6dd468f7bcff38214eb77bc91b241e/reactionmenu/text.py#L288
-                    
-                    if re.search(CODEBLOCK, page.content): # type: ignore
-                        if re.search(CODEBLOCK_DATA_AFTER, page.content): # type: ignore
-                            page.content = f'{page.content}\n\n{page_info}'
-                        else:
-                            page.content = f'{page.content}\n{page_info}'
-                    else:
-                        page.content = f'{page.content}\n\n{page_info}'
-                    page_number += 1
-    
-    async def _handle_session_limits(self) -> bool:
-        """|coro| Determine if the menu session is currently limited, if so, send the error message and return `False` indicating that further code execution (starting the menu) should be cancelled
-        
-            .. note::
-                This method is only called if `_LimitDetails.set_by_user` has been set externally (by the public method)
-        """
-        cls = self.__class__
-        details = cls._sessions_limit_details
-        can_proceed = True
-
-        # if the menu is in a DM, handle it separately
-        if self.in_dms:
-            dm_sessions = cls.get_all_dm_sessions()
-            if dm_sessions:
-                user_dm_sessions = [session for session in dm_sessions if session.owner.id == self._extract_proper_user(self._method).id]
-                if len(user_dm_sessions) >= details.limit:
-                    can_proceed = False
-        else:
-            if details.per == 'guild':
-                guild_sessions = [session for session in cls._active_sessions if session.message.guild is not None] # type: ignore
-                if len(guild_sessions) >= details.limit:
-                    can_proceed = False
-            
-            elif details.per == 'member':
-                member_sessions = [session for session in cls._active_sessions if session.owner.id == self._extract_proper_user(self._method).id]
-                if len(member_sessions) >= details.limit:
-                    can_proceed = False
-            
-            elif details.per == 'channel':
-                channel_sessions = [session for session in cls._active_sessions if session.message.channel.id == self._method.channel.id] # type: ignore
-                if len(channel_sessions) >= details.limit:
-                    can_proceed = False
-        
-        if can_proceed:
-            return True
-        else:
-            await self._method.channel.send(details.message) # type: ignore
-            return False
-    
-    def _maybe_new_style(self, counter: int, total_pages: int) -> str: 
-        """Sets custom page director styles"""
-        if self.style:
-            if self.style.count('$') == 1 and self.style.count('&') == 1:
-                temp = self.style # copy it to a new variable so its not being changed in every call
-                temp = temp.replace('$', str(counter))
-                temp = temp.replace('&', str(total_pages))
-                return temp
-            else:
-                raise ImproperStyleFormat
-        else:
-            return f'Page {counter}/{total_pages}'
-    
-    async def _contact_relay(self, member: Union[discord.Member, discord.User], button: GB) -> None: # type: ignore
-        """|coro| Dispatch the information to the relay function if a relay has been set"""
-        if self._relay_info:
-            func: Callable = self._relay_info.func # type: ignore
-            only = self._relay_info.only # type: ignore
-            RelayPayload = collections.namedtuple('RelayPayload', ['member', 'button'])
-            payload = RelayPayload(member=member, button=button)
-
-            # before the information is relayed, ensure the relay function contains a single positional argument
-            spec = inspect.getfullargspec(func)
-            if all([
-                len(spec.args) == 1,
-                not spec.varargs,
-                not spec.varkw,
-                not spec.defaults,
-                not spec.kwonlyargs,
-                not spec.kwonlydefaults
-            ]):
-                async def call() -> None:
-                    """|coro| Dispatch the information to the relay function. If any errors occur during the call, report it to the user"""
-                    try:
-                        if asyncio.iscoroutinefunction(func):
-                            await func(payload)
-                        else:
-                            func(payload)
-                    except Exception as error:
-                        error_msg = inspect.cleandoc(
-                            f"""When dispatching the information to your relay function ("{func.__name__}"), that function raised an error during it's execution
-                            -> {error.__class__.__name__}: {error}
-                            """
-                        )
-                        raise MenuException(error_msg)
-
-                if only:
-                    if button in only:
-                        await call()
-                else:
-                    await call()
-            else:
-                raise MenuException('When setting a relay, the relay function must have exactly one positional argument')
-    
-    def _handle_reply_kwargs(self, send_to, reply: bool) -> dict:
-        """Used to determine the mentions for the `reply` parameter in :meth:`.start()`"""
-        if isinstance(send_to, (discord.TextChannel, discord.VoiceChannel, discord.Thread)) and send_to == self._method.channel:
-            send_to = None
-        return {
-            'reference' : self._method.message if all([send_to is None, reply is True]) else None,
-            'mention_author' : self.allowed_mentions.replied_user
-        }
-    
-    async def _handle_send_to(self, send_to: Union[str, int, discord.TextChannel, discord.VoiceChannel, discord.Thread, None], menu_payload: dict) -> None:
-        """|coro| For the :param:`send_to` kwarg in :meth:`Menu.start()`. Determine what channel the menu should start in"""
-        if isinstance(self._method, Context):
-
-            async def register_message(channel: discord.abc.Messageable) -> None:
-                """|coro| Set :attr:`_msg` to the :class:`discord.Message` that the menu is operating from"""
-                self._msg = await channel.send(**menu_payload) # type: ignore
-            
-            if self.in_dms:
-                await register_message(self._method.channel)
-            else:
-                if send_to is None:
-                    await register_message(self._method.channel)
-                else:
-                    if not isinstance(send_to, (str, int, discord.TextChannel, discord.VoiceChannel, discord.Thread)):
-                        raise IncorrectType(f'Parameter "send_to" expected str, int, discord.TextChannel, discord.VoiceChannel, or discord.Thread, got {send_to.__class__.__name__}')
-                    else:
-                        class_name = self.__class__.__name__                    # converted to list because its a sequence proxy
-                        all_messageable_channels = self._method.guild.text_channels + list(self._method.guild.threads) + self._method.guild.voice_channels # type: ignore
-                        
-                        # before we continue, check if there are any duplicate named text channels or threads/no matching names found if a str was provided
-                        if isinstance(send_to, str):
-                            matched_channels = [ch for ch in all_messageable_channels if ch.name == send_to]
-                            if len(matched_channels) == 0:
-                                raise MenuException(f'When using parameter "send_to" in {class_name}.start(), there were no channels/threads with the name {send_to!r}')
-                            
-                            elif len(matched_channels) >= 2:
-                                raise MenuException(f'When using parameter "send_to" in {class_name}.start(), there were {len(matched_channels)} channels/threads with the name {send_to!r}. With multiple channels/threads having the same name, the intended channel is unknown')
-                        
-                        for channel in all_messageable_channels:
-                            if isinstance(send_to, str):
-                                if channel.name == send_to:
-                                    await register_message(channel)
-                                    break
-                            
-                            elif isinstance(send_to, int):
-                                if channel.id == send_to:
-                                    await register_message(channel)
-                                    break
-                            
-                            # it should be a discord.TextChannel, discord.VoiceChannel, or discord.Thread
-                            else:
-                                if channel == send_to:
-                                    await register_message(channel)
-                                    break
-
-                        else:
-                            raise MenuException(f'When using parameter "send_to" in {class_name}.start(), the channel {send_to} was not found')
-        
-        elif isinstance(self._method, discord.Interaction):
-            if self._method.response.is_done():
-                await self._method.followup.send(**menu_payload)
-            else:
-                await self._method.response.send_message(**menu_payload)
-            self._msg = await self._method.original_response()
-        
-        else:
-            raise IncorrectType('Parameter "method" was not of the correct type')
-
-    def randomize_embed_colors(self) -> None:
-        """Randomize the color of all the embeds that have been added to the menu
-        
-        Raises
-        ------
-        - `MenuException`: The `menu_type` was not of `TypeEmbed`
-        
-            .. added:: v3.1.0
-        """
-        if self._menu_type == _BaseMenu.TypeEmbed:
-            for page in self._pages:
-                if page.embed:
-                    page.embed.color = discord.Color.random()
-        else:
-            raise MenuException("Randomizing embed colors can only be used when the menu_type is TypeEmbed")
-    
-    def set_page_director_style(self, style_id: int, separator: str=DEFAULT) -> None:
-        """Set how the page numbers dictating what page you are on (in the footer of an embed/regular message) are displayed
-
-        Parameters
-        ----------
-        style_id: :class:`int`
-            Varying formats of how the page director can be presented. The following ID's are available:
-
-            - `1` = Page 1/10
-            - `2` = Page 1 out of 10
-            - `3` = 1 out of 10
-            - `4` = 1 • 10
-            - `5` = 1 » 10
-            - `6` = 1 | 10
-            - `7` = 1 : 10
-            - `8` = 1 - 10
-            - `9` = 1 / 10
-            - `10` = 1 🔹 10
-            - `11` = 1 🔸 10
-        
-        separator: :class:`str`
-            The separator between the page director and any text you may have in the embed footer. The default separator is ":". It should be noted that whichever separator you assign,
-            if you wish to have spacing between the page director and the separator, you must place the space inside the string yourself as such: " :"
-        
-        Raises
-        ------
-        - `MenuException`: The :param:`style_id` value was not valid 
-        """
-        if separator:
-            self._page_director_separator = str(separator)
-        
-        if style_id == 1:   self.style = _DEFAULT_STYLE
-        elif style_id == 2: self.style = 'Page $ out of &'
-        elif style_id == 3: self.style = '$ out of &'
-        elif style_id == 4: self.style = '$ • &'
-        elif style_id == 5: self.style = '$ » &'
-        elif style_id == 6: self.style = '$ | &'
-        elif style_id == 7: self.style = '$ : &'
-        elif style_id == 8: self.style = '$ - &'
-        elif style_id == 9: self.style = '$ / &'
-        elif style_id == 10: self.style = '$ 🔹 &'
-        elif style_id == 11: self.style = '$ 🔸 &'
-        else:
-            raise MenuException(f'Parameter "style_id" expected a number 1-11, got {style_id!r}')
-    
-    async def wait_until_closed(self) -> None:
-        """|coro|
-        
-        Waits until the menu session ends using `.stop()` or when the menu times out. This should not be used inside relays
-        
-            .. added:: v3.0.1
-        """
-        await self._on_close_event.wait()
-    
-    @ensure_not_primed
-    def add_from_messages(self, messages: Sequence[discord.Message]) -> None:
-        """Add pages to the menu using the message object itself
-        
-        Parameters
-        ----------
-        messages: Sequence[:class:`discord.Message`]
-            A sequence of discord message objects
-        
-        Raises
-        ------
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        - `MenuSettingsMismatch`: The messages provided did not have the correct values. For example, the `menu_type` was set to `TypeEmbed`, but the messages you've provided only contains text. If the `menu_type` is `TypeEmbed`, only messages with embeds should be provided
-        - `IncorrectType`: All messages were not of type :class:`discord.Message`
-        """
-        if all([isinstance(msg, discord.Message) for msg in messages]):
-            if self._menu_type == _BaseMenu.TypeEmbed:
-                embeds: List[discord.Embed] = []
-                for m in messages:
-                    if m.embeds:
-                        embeds.extend(m.embeds)
-                if embeds:
-                    self.add_pages(embeds)
-                else:
-                    raise MenuSettingsMismatch(f'The menu is set to {self._menu_type.name} but no embeds were found in the messages provided')
-            
-            elif self._menu_type == _BaseMenu.TypeText:
-                content: List[str] = []
-                for m in messages:
-                    if m.content:
-                        content.append(m.content)
-                if content:
-                    self.add_pages(content)
-                else:
-                    raise MenuSettingsMismatch(f'The menu is set to {self._menu_type.name} but no text (discord.Message.content) was found in the messages provided')
-        else:
-            raise IncorrectType('All messages were not of type discord.Message')
-    
-    @ensure_not_primed
-    async def add_from_ids(self, messageable: discord.abc.Messageable, message_ids: Sequence[int]) -> None:
-        """|coro|
-        
-        Add pages to the menu using the IDs of messages. This only grabs embeds (if the `menu_type` is :attr:`TypeEmbed`) or the content (if the `menu_type` is :attr:`TypeText`) from the message
-        
-        Parameters
-        ----------
-        messageable: :class:`discord.abc.Messageable`
-            A discord :class:`Messageable` object (:class:`discord.TextChannel`, :class:`commands.Context`, etc.)
-        
-        message_ids: Sequence[:class:`int`]
-            The messages to fetch
-
-        Raises
-        ------
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        - `MenuSettingsMismatch`: The message IDs provided did not have the correct values when fetched. For example, the `menu_type` was set to `TypeEmbed`, but the messages you've provided for the library to fetch only contains text. If the `menu_type` is `TypeEmbed`, only messages with embeds should be provided
-        - `MenuException`: An error occurred when attempting to fetch a message or not all :param:`message_ids` were of type int
-        """
-        if all([isinstance(ID, int) for ID in message_ids]):
-            to_paginate: List[discord.Message] = []            
-            for msg_id in message_ids:
-                try:
-                    fetched_message = await messageable.fetch_message(msg_id)
-                    to_paginate.append(fetched_message)
-                except (discord.NotFound, discord.Forbidden, discord.HTTPException) as error:
-                    raise MenuException(f'An error occurred when attempting to retrieve message with the ID {msg_id}: {error}')
-            
-            if self._menu_type == _BaseMenu.TypeEmbed:
-                embeds_to_paginate: List[discord.Embed] = []
-                for msg in to_paginate:
-                    if msg.embeds:
-                        embeds_to_paginate.extend(msg.embeds)
-                if embeds_to_paginate:
-                    for embed in embeds_to_paginate:
-                        self.add_page(embed)
-                else:
-                    raise MenuSettingsMismatch(f'The menu is set to {self._menu_type.name} but no embeds were found in the messages provided')
-            
-            elif self._menu_type == _BaseMenu.TypeText:
-                content_to_paginate: List[str] = []
-                for msg in to_paginate:
-                    if msg.content:
-                        content_to_paginate.append(msg.content)
-                if content_to_paginate:
-                    for content in content_to_paginate:
-                        self.add_page(content=content)
-                else:
-                    raise MenuSettingsMismatch(f'The menu is set to {self._menu_type.name} but no text (discord.Message.content) was found in the messages provided')
-        else:
-            raise MenuException('Not all message IDs were of type int')
-    
-    @ensure_not_primed
-    def clear_all_row_data(self) -> None:
-        """Delete all the data thats been added using :meth:`add_row()`
-        
-        Raises
-        ------
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        - `MenuSettingsMismatch`: This method was called but the menus `menu_type` was not :attr:`TypeEmbedDynamic`
-        """
-        if self._menu_type == _BaseMenu.TypeEmbedDynamic:
-            self._dynamic_data_builder.clear()
-        else:
-            raise MenuSettingsMismatch('Cannot clear all row data when the menu_type is not set as TypeEmbedDynamic')
-    
-    @ensure_not_primed
-    def add_row(self, data: str) -> None:
-        """Add text to the embed page by rows of data
-        
-        Parameters
-        ----------
-        data: :class:`str`
-            The data to add
-        
-        Raises
-        ------
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        - `MenuSettingsMismatch`: This method was called but the menus `menu_type` was not :attr:`TypeEmbedDynamic`
-        - `MissingSetting`: The kwarg "rows_requested" (int) has not been set for the menu
-        """
-        if self._menu_type == _BaseMenu.TypeEmbedDynamic:
-            if self.rows_requested:
-                self._dynamic_data_builder.append(str(data))
-            else:
-                raise MissingSetting('The kwarg "rows_requested" (int) has not been set for the menu')
-        else:
-            raise MenuSettingsMismatch('add_row() can only be used with a menu_type of TypeEmbedDynamic')
-    
-    @ensure_not_primed
-    def set_main_pages(self, *embeds: discord.Embed) -> None:
-        """On a menu with a `menu_type` of :attr:`TypeEmbedDynamic`, set the pages you would like to show first. These embeds will be shown before the embeds that contain your data
-        
-        Parameters
-        ----------
-        *embeds: :class:`discord.Embed`
-            An argument list of :class:`discord.Embed` objects
-        
-        Raises
-        ------
-        - `MenuSettingsMismatch`: Tried to use method on a menu that was not of `menu_type` :attr:`TypeEmbedDynamic`
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        - `MenuException`: The "embeds" parameter was empty. At least one value is needed
-        - `IncorrectType`: All values in the argument list were not of type :class:`discord.Embed`
-        """
-        if not embeds: raise MenuException('The argument list when setting main pages was empty')
-        if not all([isinstance(e, discord.Embed) for e in embeds]): raise IncorrectType('All values in the argument list when setting main pages were not of type discord.Embed')
-        if self._menu_type != _BaseMenu.TypeEmbedDynamic: raise MenuSettingsMismatch('Method set_main_pages is only available for menus with menu_type TypeEmbedDynamic')
-        
-        # if they've set any values, remove it. Each set should be from the call and should not stack
-        self._main_page_contents.clear()
-        
-        for embed in embeds:
-            self._main_page_contents.append(embed)
-
-    @ensure_not_primed
-    def set_last_pages(self, *embeds: discord.Embed) -> None:
-        """On a menu with a `menu_type` of :attr:`TypeEmbedDynamic`, set the pages you would like to show last. These embeds will be shown after the embeds that contain your data
-        
-        Parameters
-        ----------
-        *embeds: :class:`discord.Embed`
-            An argument list of :class:`discord.Embed` objects
-        
-        Raises
-        ------
-        - `MenuSettingsMismatch`: Tried to use method on a menu that was not of `menu_type` :attr:`TypeEmbedDynamic`
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        - `MenuException`: The "embeds" parameter was empty. At least one value is needed
-        - `IncorrectType`: All values in the argument list were not of type :class:`discord.Embed`
-        """
-        if not embeds: raise MenuException('The argument list when setting last pages was empty')
-        if not all([isinstance(e, discord.Embed) for e in embeds]): raise IncorrectType('All values in the argument list when setting last pages were not of type discord.Embed')
-        if self._menu_type != _BaseMenu.TypeEmbedDynamic: raise MenuSettingsMismatch('Method set_last_pages is only available for menus with menu_type TypeEmbedDynamic')
-        
-        # if they've set any values, remove it. Each set should be from the call and should not stack
-        self._last_page_contents.clear()
-        
-        for embed in embeds:
-            self._last_page_contents.append(embed)
-    
-    @ensure_not_primed
-    def add_page(self, embed: Optional[discord.Embed]=MISSING, content: Optional[str]=None, files: Optional[List[discord.File]]=MISSING) -> None:
-        """Add a page to the menu
-
-        Parameters
-        ----------
-        embed: Optional[:class:`discord.Embed`]
-            The embed of the page
-        
-        content: Optional[:class:`str`]
-            The text that appears above an embed in a message
-        
-        files: Optional[Sequence[:class:`discord.File`]]
-            Files you'd like to attach to the page
-        
-        Raises
-        ------
-        - `MenuException`: Attempted to add a page with no parameters
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        - `MenuSettingsMismatch`: The page being added does not match the menus `menu_type` 
-        
-            .. changes::
-                v3.1.0
-                    Added parameter content
-                    Added parameter embed
-                    Added parameter files
-                    Removed parameter "page"
-        """
-        if all([content is None, embed is None, files is None]):
-            raise MenuException("When adding a page, at lease one parameter must be set")
-        
-        cls = self.__class__
-        if self._menu_type == cls.TypeEmbed:
-            if isinstance(embed, discord.Embed):
-                self._pages.append(Page(content=content, embed=embed, files=files))
-            else:
-                raise MenuSettingsMismatch(f'When adding a page with a menu_type of TypeEmbed, the "embed" parameter cannot be None')
-        
-        elif self._menu_type == cls.TypeText:
-            if content:
-                self._pages.append(Page(content=str(content), files=files))
-            else:
-                raise MenuSettingsMismatch(f'When adding a page with a menu_type of TypeText, the "content" parameter cannot be None')
-        
-        else:
-            raise MenuSettingsMismatch('add_page method cannot be used with the current menu_type')
-    
-    @overload
-    def add_pages(self, pages: Sequence[discord.Embed]) -> None:
-        ...
-    
-    @overload
-    def add_pages(self, pages: Sequence[str]) -> None:
-        ...
-
-    @ensure_not_primed
-    def add_pages(self, pages: Sequence[Union[discord.Embed, str]]) -> None:
-        """Add multiple pages to the menu at once
-        
-        Parameters
-        ----------
-        pages: Sequence[Union[:class:`discord.Embed`, :class:`str`]]
-            The pages to add. Can only be used when the menus `menu_type` is :attr:`TypeEmbed` (adding a :class:`discord.Embed`)
-            or :attr:`TypeText` (adding a :class:`str`)
-        
-        Raises
-        ------
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        - `MenuSettingsMismatch`: The page being added does not match the menus `menu_type` 
-        """
-        for embed_or_str in pages:
-            if isinstance(embed_or_str, str):
-                self.add_page(content=embed_or_str)
-            else:
-                self.add_page(embed_or_str) # type: ignore
-    
-    @ensure_not_primed
-    def remove_all_pages(self) -> None:
-        """Remove all pages from the menu
-        
-        Raises
-        ------
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        """
-        self._pages.clear()
-    
-    @ensure_not_primed
-    def remove_page(self, page_number: int) -> None:
-        """Remove a page from the menu
-        
-        Parameters
-        ----------
-        page_number: :class:`int`
-            The page to remove
-        
-        Raises
-        ------
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        - `InvalidPage`: The page associated with the given page number was not valid
-        """
-        if self._pages:
-            if page_number > 0 and page_number <= len(self._pages):
-                page_to_delete = page_number - 1
-                del self._pages[page_to_delete]
-            else:
-                raise InvalidPage(f'Page number invalid. Must be from 1 - {len(self._pages)}')
-    
-    def set_on_timeout(self, func: Callable[[M], None]) -> None:
-        """Set the function to be called when the menu times out
-
-        Parameters
-        ----------
-        func: Callable[[:type:`M`]], :class:`None`]
-            The function object that will be called when the menu times out. The function should contain a single positional argument
-            and should not return anything. The argument passed to that function is an instance of the menu.
-        
-        Raises
-        ------
-        - `IncorrectType`: Parameter "func" was not a callable object
-        """
-        if not callable(func): raise IncorrectType('Parameter "func" must be callable')
-        self._on_timeout_details = func # type: ignore
-    
-    def remove_on_timeout(self) -> None:
-        """Remove the timeout call to the function you have set when the menu times out"""
-        self._on_timeout_details = None
-    
-    def set_relay(self, func: Callable[[NamedTuple], None], *, only: Optional[List[GB]]=None) -> None:
-        """Set a function to be called with a given set of information when a button is pressed on the menu. The information passed is `RelayPayload`, a named tuple.
-        The named tuple contains the following attributes:
-
-        - `member`: The :class:`discord.Member` object of the person who pressed the button. Could be :class:`discord.User` if the menu was started in a DM
-        - `button`: Depending on the menu instance, the :class:`ReactionButton` or :class:`ViewButton` object of the button that was pressed
-
-        Parameters
-        ----------
-        func: Callable[[:class:`NamedTuple`], :class:`None`]
-            The function should only contain a single positional argument. Command functions (`@bot.command()`) not supported
-        
-        only: Optional[List[:generic:`GB`]]
-            A list of buttons (`GB`) associated with the current menu instance. If the menu instance is :class:`ReactionMenu`, this should be a list of :class:`ReactionButton`
-            and vice-versa for :class:`ViewMenu` instances. If this is :class:`None`, all buttons on the menu will be relayed. If set, only button presses from those specified buttons will be relayed
-        
-        Raises
-        ------
-        - `IncorrectType`: The :param:`func` argument provided was not callable
-        """
-        if callable(func):
-            RelayInfo = collections.namedtuple('RelayInfo', ['func', 'only'])
-            self._relay_info = RelayInfo(func=func, only=only)
-        else:
-            raise IncorrectType('When setting the relay, argument "func" must be callable')
-    
-    def remove_relay(self) -> None:
-        """Remove the relay that's been set"""
-        self._relay_info = None
+"""
+MIT License
+
+Copyright (c) 2021-present Defxult#8269
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    ClassVar,
+    Final,
+    Generic,
+    Iterable,
+    List,
+    Literal,
+    Optional,
+    Set,
+    Tuple,
+    TypeVar,
+    Union,
+    overload
+)
+
+if TYPE_CHECKING:
+    from datetime import datetime
+    from typing_extensions import Self
+
+import abc
+import asyncio
+import collections
+import inspect
+import re
+import warnings
+from collections.abc import Sequence
+from enum import Enum, auto
+from typing import NamedTuple, Union
+
+import discord
+from discord.ext.commands import Context
+from discord.utils import MISSING
+
+from .decorators import ensure_not_primed
+from .errors import *
+
+# Constants
+_DYNAMIC_EMBED_LIMIT: Final[int] = 4096
+_DEFAULT_STYLE: Final[str] = 'Page $/&'
+DEFAULT_BUTTONS = None
+DEFAULT = MISSING
+
+GB = TypeVar('GB', bound='_BaseButton')
+M = TypeVar('M', bound='_BaseMenu')
+
+class Page:
+    """Represents a single "page" in the pagination process
+    
+        .. added:: v3.1.0
+    """
+    __slots__ = ("content", "embed", "files", "_go_to")
+    
+    def __init__(self, *, content: Optional[str]=None, embed: Optional[discord.Embed]=MISSING, files: Optional[List[discord.File]]=MISSING) -> None:
+        self.content = content
+        self.embed = embed
+        self.files = files
+        self._go_to: Optional[int] = None
+    
+    def __repr__(self) -> str:
+        return f"<Page {' '.join([f'{attr_name}={getattr(self, attr_name)!r}' for attr_name in self.__class__.__slots__ if type(getattr(self, attr_name)) not in (type(None), type(MISSING))])}>"
+    
+    def _shallow(self) -> Self:
+        from copy import copy
+        return copy(self)
+
+class PaginationEmojis:
+    """A set of basic emojis for your convenience to use for your buttons emoji
+    - ◀️ as `BACK_BUTTON`
+    - ▶️ as `NEXT_BUTTON`
+    - ⏪ as `FIRST_PAGE`
+    - ⏩ as `LAST_PAGE`
+    - 🔢 as `GO_TO_PAGE`
+    - ⏹️ as `END_SESSION`
+    """
+    BACK_BUTTON: ClassVar[str] = '◀️'
+    NEXT_BUTTON: ClassVar[str] = '▶️'
+    FIRST_PAGE: ClassVar[str]  = '⏪'
+    LAST_PAGE: ClassVar[str]   = '⏩'
+    GO_TO_PAGE: ClassVar[str]  = '🔢'
+    END_SESSION: ClassVar[str] = '⏹️'
+
+class _PageController:
+    def __init__(self, pages: List[Page]) -> None:
+        self.ALL_PAGES: Final[List[Page]] = pages
+        self.index = 0
+
+    @property
+    def current_page(self) -> Page:
+        return self.ALL_PAGES[self.index]
+    
+    @property
+    def total_pages(self) -> int:
+        """Return the total amount of pages registered to the menu"""
+        return len(self.ALL_PAGES) - 1
+    
+    def validate_index(self) -> Page:
+        """If the index is out of bounds, assign the appropriate values so the pagination process can continue and return the associated page"""
+        try:
+            _ = self.ALL_PAGES[self.index]
+        except IndexError:
+            if self.index > self.total_pages:
+                self.index = 0
+            
+            elif self.index < 0:
+                self.index = self.total_pages
+        finally:
+            return self.ALL_PAGES[self.index]
+    
+    def skip_loop(self, action: str, amount: int) -> None:
+        """Using `self.index += amount` does not work because this library is used to operating on a +-1 basis. This loop
+        provides a simple way to still operate on the +-1 standard.
+        """
+        while amount != 0:
+            if action == '+':
+                self.index += 1
+            elif action == '-':
+                self.index -= 1
+            
+            self.validate_index()
+            amount -= 1
+    
+    def skip(self, skip: _BaseButton.Skip) -> Page:
+        """Return the page that the skip value was set to"""
+        self.skip_loop(skip.action, skip.amount)
+        return self.validate_index()
+
+    def next(self) -> Page:
+        """Return the next page in the pagination process"""
+        self.index += 1
+        return self.validate_index()
+    
+    def prev(self) -> Page:
+        """Return the previous page in the pagination process"""
+        self.index -= 1
+        return self.validate_index()
+    
+    def first_page(self) -> Page:
+        """Return the first page in the pagination process"""
+        self.index = 0
+        return self.ALL_PAGES[self.index]
+
+    def last_page(self) -> Page:
+        """Return the last page in the pagination process"""
+        self.index = self.total_pages
+        return self.ALL_PAGES[self.index]
+
+class _MenuType(Enum):
+    TypeEmbed = auto()
+    TypeEmbedDynamic = auto()
+    TypeText = auto()
+
+MenuType = _MenuType
+
+class _LimitDetails(NamedTuple):
+    limit: int
+    per: str
+    message: str
+    set_by_user: bool = False
+
+    @classmethod
+    def default(cls) -> Self:
+        return cls(0, "", "")
+
+class _BaseButton(Generic[GB], metaclass=abc.ABCMeta):
+
+    Emojis: ClassVar[PaginationEmojis] = PaginationEmojis()
+
+    def __init__(self, name: str, event: Optional[_BaseButton.Event], skip: _BaseButton.Skip):
+        self.name: str = name
+        self.event: Optional[_BaseButton.Event] = event
+        self.skip: _BaseButton.Skip = skip
+        self.__clicked_by = set()
+        self.__total_clicks = 0
+        self.__last_clicked: Optional[datetime] = None
+    
+    @property
+    @abc.abstractmethod
+    def menu(self):
+        raise NotImplementedError
+    
+    @property
+    def clicked_by(self) -> Set[discord.Member]:
+        """
+        Returns
+        -------
+        Set[:class:`discord.Member`]: The members who clicked the button
+        """
+        return self.__clicked_by
+    
+    @property
+    def total_clicks(self) -> int:
+        """
+        Returns
+        -------
+        :class:`int`: The amount of clicks on the button
+        """
+        return self.__total_clicks
+
+    @property
+    def last_clicked(self) -> Optional[datetime]:
+        """
+        Returns
+        -------
+        Optional[:class:`datetime.datetime`]: The time in UTC for when the button was last clicked. Can be :class:`None` if the button has not been clicked
+        """
+        return self.__last_clicked
+
+    def _update_statistics(self, user: Union[discord.Member, discord.User]) -> None:
+        self.__clicked_by.add(user)
+        self.__total_clicks += 1
+        self.__last_clicked = discord.utils.utcnow()
+
+    class Skip:
+        """Initialize a skip button with the appropriate values
+        
+        Parameters
+        ----------
+        action: :class:`str`
+            Whether to go forward in the pagination process ("+") or backwards ("-")
+        
+        amount: :class:`int`
+            The amount of pages to skip. Must be >= 1. If value is <= 0, it is implicitly set to 2
+        """
+        def __init__(self, action: Literal['+', '-'], amount: int):
+            if amount <= 0: amount = 2
+            if action in ('+', '-'):
+                self.action = action
+                self.amount = amount
+            else:
+                raise MenuException('The action given was not recognized. Expected "+" or "-"')
+
+    class Event:
+        """Set a button to be disabled or removed when it has been pressed a certain amount of times. If the button is a :class:`ReactionButton`, only the "remove" event is available
+        
+        Parameters
+        ----------
+        event: :class:`str`
+            The action to take. Can either be "disable" or "remove"
+        
+        value: :class:`int`
+            The amount set for the specified event. Must be >= 1. If value is <= 0, it is implicitly set to 1"""
+        
+        _DISABLE = 'disable'
+        _REMOVE = 'remove'
+
+        def __init__(self, event_type: Literal['disable', 'remove'], value: int):
+            if value <= 0: value = 1
+            event_type = str(event_type).lower() # type: ignore
+            cls = self.__class__
+            
+            if event_type in (cls._DISABLE, cls._REMOVE):
+                self.event_type = event_type
+                self.value = value
+            else:
+                raise MenuException('The value for parameter "event_type" was not recognized')
+
+class _BaseMenu(metaclass=abc.ABCMeta):
+    TypeEmbed: Final[_MenuType] = _MenuType.TypeEmbed
+    TypeEmbedDynamic: Final[_MenuType] = _MenuType.TypeEmbedDynamic
+    TypeText: Final[_MenuType] = _MenuType.TypeText
+
+    _sessions_limit_details = _LimitDetails.default()
+    _active_sessions: List[Self] # initialized in child classes
+
+    def __init__(self, method: Union[Context, discord.Interaction], /, menu_type: _MenuType, **kwargs):
+        # `Context` has an `interaction` attribute. If that attribute is `None`,
+        # it's not an application command, if so, it's an application command so access
+        # and set the interaction attribute so a `ViewMenu` can be used.
+        if isinstance(method, Context) and method.interaction is None:
+            self._method = method
+        elif isinstance(method, Context) and method.interaction is not None:
+            self._method = method.interaction
+        else:
+            self._method = method # will be an interaction
+
+        self._menu_type = menu_type
+
+        self._msg: Union[discord.Message, discord.InteractionMessage] # initialized in child classes
+        self._pc:_PageController # initialized in child classes
+        self._is_running = False
+        self._stop_initiated = False
+        self._page_director_separator = ":"
+
+        # dynamic session
+        self._main_page_contents = collections.deque()
+        self._last_page_contents = collections.deque()
+        self._dynamic_data_builder: List[str] = []
+        self.wrap_in_codeblock: Optional[str] = kwargs.get('wrap_in_codeblock')
+        self.rows_requested: int = kwargs.get('rows_requested', 0)
+        self.custom_embed: Optional[discord.Embed] = kwargs.get('custom_embed')
+
+        self._relay_info: Optional[NamedTuple] = None
+        self._on_timeout_details: Optional[Callable[[_BaseMenu], None]] = None
+        self._menu_timed_out = False
+        self._bypass_primed = False # used in :meth:`update()`
+        self._pages: List[Page] = []
+        self._on_close_event = asyncio.Event() # used for :meth:`wait_until_close()`
+
+        # kwargs
+        self.delete_on_timeout: bool = kwargs.get('delete_on_timeout', False)
+        self.only_roles: Optional[List[discord.Role]] = kwargs.get('only_roles')
+        self.show_page_director: bool = kwargs.get('show_page_director', True)
+        self.name: Optional[str] = kwargs.get('name')
+        self.style: Optional[str] = kwargs.get('style', _DEFAULT_STYLE)
+        self.all_can_click: bool = kwargs.get('all_can_click', False)
+        self.delete_interactions: bool = kwargs.get('delete_interactions', True)
+        self.allowed_mentions: discord.AllowedMentions = kwargs.get('allowed_mentions', discord.AllowedMentions(everyone=False, users=True, roles=False, replied_user=True))
+    
+    @abc.abstractmethod
+    def _handle_event(self):
+        raise NotImplementedError
+    
+    @abc.abstractmethod
+    def remove_all_buttons(self):
+        raise NotImplementedError
+    
+    @abc.abstractmethod
+    def get_button(self):
+        raise NotImplementedError
+    
+    @abc.abstractmethod
+    def remove_button(self):
+        raise NotImplementedError
+    
+    @abc.abstractmethod
+    def add_button(self):
+        raise NotImplementedError
+    
+    @abc.abstractmethod
+    def add_buttons(self):
+        raise NotImplementedError
+    
+    @abc.abstractmethod
+    def _override_dm_settings(self):
+        raise NotImplementedError
+    
+    @abc.abstractmethod
+    def stop(self):
+        raise NotImplementedError
+    
+    @abc.abstractmethod
+    async def start(self):
+        raise NotImplementedError
+    
+    # ABC class methods
+    
+    @abc.abstractclassmethod
+    async def quick_start(cls):
+        raise NotImplementedError
+    
+    @staticmethod
+    def separate(values: Sequence[Any]) -> Tuple[List[discord.Embed], List[str]]:
+        """|static method|
+        
+        Sorts all embeds and strings into a single tuple
+
+        Parameters
+        ----------
+        values: Sequence[`Any`]
+            The values to separate
+        
+        Returns
+        -------
+        Tuple[List[:class:`discord.Embed`], List[:class:`str`]]
+        
+        Example
+        -------
+        >>> embeds, strings = .separate([...])
+        """
+        all_embeds = list(filter(lambda item: isinstance(item, discord.Embed), values))
+        all_strings = list(filter(lambda item: isinstance(item, str), values))
+        return (all_embeds, all_strings)
+    
+    @staticmethod
+    def all_embeds(values: Sequence[Any]) -> bool:
+        """|static method|
+        
+        Tests to see if all items in the sequence are of type :class:`discord.Embed`
+        
+        Parameters
+        ----------
+        values: Sequence[`Any`]
+            The values to test
+        
+        Returns
+        -------
+        :class:`bool`: Can return `False` if the sequence is empty
+        """
+        return all([isinstance(item, discord.Embed) for item in values]) if values else False
+    
+    @staticmethod
+    def _sort_buttons(buttons: List[GB]) -> List[GB]:
+        return sorted(buttons, key=lambda btn: btn.total_clicks, reverse=True)
+    
+    @staticmethod
+    def all_strings(values: Sequence[Any]) -> bool:
+        """|static method|
+        
+        Tests to see if all items in the sequence are of type :class:`str`
+        
+        Parameters
+        ----------
+        values: Sequence[`Any`]
+            The values to test
+        
+        Returns
+        -------
+        :class:`bool`: Can return `False` if the sequence is empty
+        """
+        return all([isinstance(item, str) for item in values]) if values else False
+    
+    @staticmethod #* Don't make this an instance method. It would be better as one, but it's main intended use is for :meth:`_check` in "views_menu.py"
+    def _extract_proper_user(method: Union[Context, discord.Interaction]) -> Union[discord.Member, discord.User]:
+        """|static method| Get the proper :class:`discord.User` / :class:`discord.Member` from the attribute depending on the instance
+
+            .. added v3.1.0
+        """
+        return method.author if isinstance(method, Context) else method.user
+    
+    @classmethod
+    def _quick_check(cls, pages: Sequence[Union[discord.Embed, str]]) -> _MenuType:
+        """|class method| Verification for :meth:`quick_start()`
+        
+            .. added v3.1.0
+        """
+        if cls.all_embeds(pages):  return cls.TypeEmbed
+        if cls.all_strings(pages): return cls.TypeText
+        raise IncorrectType(f'All items in the sequence were not of type discord.Embed or str')
+    
+    @classmethod
+    def _all_menu_types(cls) -> Tuple[_MenuType, _MenuType, _MenuType]:
+        return (cls.TypeEmbed, cls.TypeEmbedDynamic, cls.TypeText)
+    
+    @classmethod
+    def remove_limit(cls) -> None:
+        """|class method|
+        
+        Remove the limits currently set for menu's
+        """
+        cls._sessions_limit_details = _LimitDetails.default()
+    
+    @classmethod
+    def get_all_dm_sessions(cls) -> List[Self]:
+        """|class method|
+        
+        Retrieve all active DM menu sessions
+        
+        Returns
+        -------
+        A :class:`list` of active DM menu sessions that are currently running. Can be an empty list if there are no active DM sessions
+        """
+        return [session for session in cls._active_sessions if session._msg.guild is None] # type: ignore
+    
+    @classmethod
+    def get_all_sessions(cls) -> List[Self]:
+        """|class method|
+        
+        Retrieve all active menu sessions
+        
+        Returns
+        -------
+        A :class:`list` of menu sessions that are currently running. Can be an empty list if there are no active sessions
+        """
+        return cls._active_sessions
+    
+    @classmethod
+    def get_session(cls, name: str) -> List[Self]:
+        """|class method|
+        
+        Get a menu instance by it's name
+        
+        Parameters
+        ----------
+        name: :class:`str`
+            The name of the menu to return
+        
+        Returns
+        -------
+        A :class:`list` of menu sessions that are currently running that match the supplied :param:`name`. Can be an empty list if there are no active sessions that matched the :param:`name`
+        """
+        name = str(name)
+        return [session for session in cls._active_sessions if session.name == name]
+    
+    @classmethod
+    def get_sessions_count(cls) -> int:
+        """|class method|
+        
+        Returns the number of active sessions
+        
+        Returns
+        -------
+        :class:`int`: The amount of menu sessions that are active
+        """
+        return len(cls._active_sessions)
+    
+    @classmethod
+    def set_sessions_limit(cls, limit: int, per: Literal['channel', 'guild', 'member']='guild', message: str='Too many active menus. Wait for other menus to be finished.') -> None:
+        """|class method|
+        
+        Sets the amount of menu sessions that can be active at the same time per guild, channel, or member. This applies to both :class:`ReactionMenu` & :class:`ViewMenu`
+
+        Parameters
+        ----------
+        limit: :class:`int`
+            The amount of menu sessions allowed
+        
+        per: :class:`str`
+            How menu sessions should be limited. Options: "channel", "guild", or "member"
+        
+        message: :class:`str`
+            Message that will be sent informing users about the menu limit when the limit is reached. Can be :class:`None` for no message
+                    
+        Raises
+        ------
+        - `IncorrectType`: The :param:`limit` parameter was not of type :class:`int`
+        - `MenuException`: The value of :param:`per` was not valid or the limit was not greater than or equal to one
+        """
+        if not isinstance(limit, int):
+            raise IncorrectType(f'Parameter "limit" expected int, got {limit.__class__.__name__}')
+        else:
+            if limit <= 0:
+                raise MenuException('The session limit must be greater than or equal to one')
+            
+            per = str(per).lower() # type: ignore
+            if per not in ('guild', 'channel', 'member'):
+                raise MenuException('Parameter value of "per" was not recognized. Expected: "channel", "guild", or "member"')
+
+            cls._sessions_limit_details = _LimitDetails(limit, per, message, set_by_user=True)
+    
+    @classmethod
+    async def stop_session(cls, name: str, include_all: bool=False) -> None:
+        """|coro class method|
+        
+        Stop a specific menu with the supplied name
+        
+        Parameters
+        ----------
+        name: :class:`str`
+            The menus name
+        
+        include_all: :class:`bool`
+            If set to `True`, it stops all menu sessions with the supplied :param:`name`. If `False`, stops only the most recently started menu with the supplied :param:`name`
+        
+        Raises
+        ------
+        - `MenuException`: The session with the supplied name was not found
+        """
+        name = str(name)
+
+        async def determine_include_all(sessions_to_stop: List[Self]) -> None:
+            """|coro| Ensures if :param:`include_all` is `True`, all sessions with the specified name will be stopped"""
+            if sessions_to_stop:
+                if include_all:
+                    for session in sessions_to_stop:
+                        await session.stop()
+                else:
+                    await sessions_to_stop[-1].stop()
+            else:
+                MESSAGE = f'Menu with name {name!r} was not found in the list of active {cls.__name__} sessions'
+                raise MenuException(MESSAGE)
+
+        matched_sessions = [session for session in cls._active_sessions if name == session.name]
+        await determine_include_all(matched_sessions)
+    
+    @classmethod
+    async def stop_all_sessions(cls) -> None:
+        """|coro class method|
+
+        Stops all menu sessions that are currently running
+        """
+        while cls._active_sessions:
+            session = cls._active_sessions[0]
+            await session.stop()
+    
+    @classmethod
+    def get_menu_from_message(cls, message_id: int, /) -> Optional[Self]:
+        """|class method|
+
+        Return the menu object associated with the message with the given ID
+
+        Parameters
+        ----------
+        message_id: :class:`int`
+            The `discord.Message.id` from the menu message
+
+        Returns
+        -------
+        The menu object. Can be :class:`None` if the menu was not found in the list of active menu sessions
+        """
+        for menu in cls._active_sessions:
+            if menu._msg.id == message_id: # type: ignore
+                return menu
+        return None
+
+    @property
+    def rows(self) -> Optional[List[str]]:
+        """
+        Returns
+        -------
+        Optional[List[:class:`str`]]: All rows that's been added to the menu. Can return `None` if the menu has not started or the `menu_type` is not `TypeEmbedDynamic`
+        
+            .. added: v3.1.0
+        """
+        return None if self._is_running is False or self._menu_type != _MenuType.TypeEmbedDynamic else self._dynamic_data_builder.copy()
+    
+    @property
+    def menu_type(self) -> str:
+        """
+        Returns
+        -------
+        :class:`str`: The `menu_type` you set via the constructor. This will either be `TypeEmbed`, `TypeEmbedDynamic`, or `TypeText`
+
+            .. added:: v3.1.0
+        """
+        return self._menu_type.name
+    
+    @property
+    def last_viewed(self) -> Optional[Page]:
+        """
+        Returns
+        -------
+        Optional[:class:`Page`]: The last page that was viewed in the pagination process. Can be :class:`None` if the menu has not been started
+        """
+        return self._pc.current_page._shallow() if self._pc is not None else None
+    
+    @property
+    def owner(self) -> Union[discord.Member, discord.User]:
+        """
+        Returns
+        -------
+        Union[:class:`discord.Member`, :class:`discord.User`]: The owner of the menu (the person that started the menu). If the menu was started in a DM, this will return :class:`discord.User`
+        """
+        return self._extract_proper_user(self._method)
+    
+    @property
+    def total_pages(self) -> int:
+        """
+        Returns
+        -------
+        :class:`int`: The amount of pages that have been added to the menu. If the `menu_type` is :attr:`TypeEmbedDynamic`, the amount of pages is not known until AFTER the menu has started. 
+        If attempted to retrieve the value before a dynamic menu has started, this will return a value of -1
+        """
+        if self._menu_type == _BaseMenu.TypeEmbedDynamic:
+            return len(self._pages) if self._is_running else -1
+        else:
+            return len(self._pages)
+    
+    @property
+    def pages(self) -> Optional[List[Page]]:
+        """
+        Returns
+        -------
+        Optional[List[:class:`Page`]]: The pages currently applied to the menu. Can return :class:`None` if there are no pages
+        
+        Note: If the `menu_type` is :attr:`TypeEmbedDynamic`, the pages aren't known until after the menu has started
+        """
+        return self._pages.copy() if self._pages else None # Return a copy so the core list of pages cannot be manipulated
+
+    @property
+    def message(self) -> Optional[Union[discord.Message, discord.InteractionMessage]]:
+        """
+        Returns
+        -------
+        Optional[Union[:class:`discord.Message`, :class:`discord.InteractionMessage`]]: The menu's message object. Can be :class:`None` if the menu has not been started
+        """
+        return self._msg
+    
+    @property
+    def is_running(self) -> bool:
+        """
+        Returns
+        -------
+        :class:`bool`: `True` if the menu is currently running, `False` otherwise
+        """
+        return self._is_running
+    
+    @property
+    def in_dms(self) -> bool:
+        """
+        Returns
+        -------
+        :class:`bool`: If the menu was started in a DM
+        """
+        return self._method.guild is None
+    
+    def _chunks(self, list_: List[str], n: int) -> Iterable:
+        """Yield successive n-sized chunks from list. Core component of a dynamic menu"""
+        for i in range(0, len(list_), n):
+            yield list_[i:i + n]
+    
+    async def _build_dynamic_pages(self, send_to, view: Optional[discord.ui.View]=None, payload: Optional[dict]=None) -> None:
+        """|coro| Compile all the information that was given via :meth:`add_row`"""
+        for data_clump in self._chunks(self._dynamic_data_builder, self.rows_requested):
+            joined_data = '\n'.join(data_clump)
+            if len(joined_data) <= _DYNAMIC_EMBED_LIMIT:
+                possible_block = f"```{self.wrap_in_codeblock}\n{joined_data}```"
+                embed = discord.Embed() if self.custom_embed is None else self.custom_embed.copy()
+                embed.description = joined_data if not self.wrap_in_codeblock else possible_block
+                self._pages.append(Page(embed=embed))
+            else:
+                raise DescriptionOversized('With the amount of data that was received, the embed description is over discords size limit. Lower the amount of "rows_requested" to solve this problem')
+        else:
+            def convert_to_page(main_last: Iterable[discord.Embed]) -> List[Page]:
+                """Initializing the :class:`deque` only supports :class:`discord.Embed`. This converts those embed objects to the supported :class:`Page` type for proper pagination
+                
+                    .. added:: v3.1.0
+                """
+                return [Page(embed=item) for item in main_last]
+            
+            # set the main/last pages if any
+            if any([self._main_page_contents, self._last_page_contents]):
+                
+                # convert to :class:`deque`
+                self._pages = collections.deque(self._pages) # type: ignore (only temporary to use extend methods of :class:`deque`)
+                
+                if self._main_page_contents:
+                    self._main_page_contents.reverse()
+                    self._pages.extendleft(convert_to_page(self._main_page_contents))
+                
+                if self._last_page_contents:
+                    self._pages.extend(convert_to_page(self._last_page_contents))
+            
+            # convert back to `list`
+            self._pages = list(self._pages)
+
+            self._refresh_page_director_info(_BaseMenu.TypeEmbedDynamic, self._pages)
+            cls = self.__class__
+
+            # make sure data has been added to create at least 1 page
+            if not self._pages: raise NoPages(f'You cannot start a {cls.__name__} when no data has been added')
+            
+            payload['embed'] = self._pages[0].embed # type: ignore / - / reassign the first page to show to director information
+            
+            if view is None:
+                await self._handle_send_to(send_to, payload) # type: ignore
+            else:
+                await self._handle_send_to(send_to, payload) # type: ignore ("embed=" can still be `None`)
+    
+    def _display_timeout_warning(self, error: Exception) -> None:
+        """Simply displays a warning message to the user notifying them an error has occurred in the function they have set for when the menu times out"""
+        warnings.formatwarning = lambda msg, *args, **kwargs: f'{msg}'
+        warnings.warn(inspect.cleandoc(
+            f"""
+            UserWarning: The function you have set in method {self.__class__.__name__}.set_on_timeout() raised an error
+            -> {error.__class__.__name__}: {error}
+            
+            This error has been ignored so the menu timeout process can complete
+            """
+        ))
+    
+    async def _handle_on_timeout(self) -> None:
+        """|coro| Call the function the user has set for when the menu times out"""
+        if self._on_timeout_details and self._menu_timed_out:
+            func = self._on_timeout_details
+            
+            # call the timeout function but ignore any and all exceptions that may occur during the function timeout call.
+            # the most important thing here is to ensure the menu is gracefully stopped while displaying a formatted
+            # error message to the user
+            try:
+                if asyncio.iscoroutinefunction(func):
+                    await func(self) # type: ignore (`iscoroutinefunction` will still return `False` if func is `None` (i want that to happen))
+                else: func(self)
+            except Exception as error:
+                self._display_timeout_warning(error)
+    
+    def _determine_kwargs(self, page: Page) -> dict:
+        """Determine the `inter.response.edit_message()` and :meth:`_msg.edit()` kwargs for the pagination process. Used in :meth:`ViewMenu._paginate()` and :meth:`ReactionMenu._paginate()`"""
+        
+        # create a copy of the files if they are set because once paginated, they are only visible once
+        maybe_new_files = [discord.File(f.filename) for f in page.files] if page.files else [] # type: ignore
+        
+        kwargs = {
+            "content" : page.content, # `content` will always be present because even with TypeEmbed menu's, pagination with the addition of text is possible
+            "allowed_mentions" : self.allowed_mentions,
+            "attachments" : maybe_new_files, # the `edit_message` method for this has an "attachment" kwarg instead of a "files" parameter
+            "allowed_mentions" : self.allowed_mentions
+        }
+
+        # only add the "embed" key if its an embed type menu
+        if self._menu_type in (_BaseMenu.TypeEmbed, _BaseMenu.TypeEmbedDynamic):
+            kwargs["embed"] = page.embed
+        return kwargs
+    
+    def _refresh_page_director_info(self, type_: _MenuType, pages: List[Page]) -> None:
+        """Sets the page count at the bottom of embeds/text if set
+        
+        Parameters
+        ----------
+        type_: :class:`_MenuType`
+            Either :attr:`_BaseMenu.TypeEmbed`, :attr:`_BaseMenu.TypeEmbedDynamic` or :attr:`_BaseMenu.TypeText`
+        
+        pages: List[:class:`Page`]
+            The pagination contents
+        """
+        if self.show_page_director:
+            if type_ not in (_BaseMenu.TypeEmbed, _BaseMenu.TypeEmbedDynamic, _BaseMenu.TypeText):
+                raise Exception('Needs to be of type _BaseMenu.TypeEmbed, _BaseMenu.TypeEmbedDynamic or _BaseMenu.TypeText') 
+            
+            page_number = 1
+
+            if type_ in (_BaseMenu.TypeEmbed, _BaseMenu.TypeEmbedDynamic):
+                page_number = 1
+                OUTOF: Final[int] = len(pages)
+                all_embeds = [p.embed for p in pages]
+                for embed in all_embeds:
+                    embed.set_footer(text=f'{self._maybe_new_style(page_number, OUTOF)}{self._page_director_separator if embed.footer.text else ""} {embed.footer.text if embed.footer.text else ""}', icon_url=embed.footer.icon_url) # type: ignore
+                    page_number += 1
+            else:
+                # TypeText Only
+
+                CODEBLOCK = re.compile(r'(`{3})(.*?)(`{3})', flags=re.DOTALL)
+                CODEBLOCK_DATA_AFTER = re.compile(r'(`{3})(.*?)(`{3}).+', flags=re.DOTALL)
+                for idx in range(len(pages)):
+                    page: Page = pages[idx]
+                    page_info = self._maybe_new_style(page_number, len(pages))
+                    
+                    # the main purpose of the re is to decide if only 1 or 2 '\n' should be used. with codeblocks, at the end of the block there is already a new line, so there's no need to add an extra one except in
+                    # the case where there is more information after the codeblock
+                    
+                    # Note: with codeblocks, i already tried the f doc string version of this and it doesnt work because there is a spacing issue with page_info. using a normal f string with \n works as intended
+                    # f doc string version: https://github.com/Defxult/reactionmenu/blob/eb88af3a2a6dd468f7bcff38214eb77bc91b241e/reactionmenu/text.py#L288
+                    
+                    if re.search(CODEBLOCK, page.content): # type: ignore
+                        if re.search(CODEBLOCK_DATA_AFTER, page.content): # type: ignore
+                            page.content = f'{page.content}\n\n{page_info}'
+                        else:
+                            page.content = f'{page.content}\n{page_info}'
+                    else:
+                        page.content = f'{page.content}\n\n{page_info}'
+                    page_number += 1
+    
+    async def _handle_session_limits(self) -> bool:
+        """|coro| Determine if the menu session is currently limited, if so, send the error message and return `False` indicating that further code execution (starting the menu) should be cancelled
+        
+            .. note::
+                This method is only called if `_LimitDetails.set_by_user` has been set externally (by the public method)
+        """
+        cls = self.__class__
+        details = cls._sessions_limit_details
+        can_proceed = True
+
+        # if the menu is in a DM, handle it separately
+        if self.in_dms:
+            dm_sessions = cls.get_all_dm_sessions()
+            if dm_sessions:
+                user_dm_sessions = [session for session in dm_sessions if session.owner.id == self._extract_proper_user(self._method).id]
+                if len(user_dm_sessions) >= details.limit:
+                    can_proceed = False
+        else:
+            if details.per == 'guild':
+                guild_sessions = [session for session in cls._active_sessions if session.message.guild is not None] # type: ignore
+                if len(guild_sessions) >= details.limit:
+                    can_proceed = False
+            
+            elif details.per == 'member':
+                member_sessions = [session for session in cls._active_sessions if session.owner.id == self._extract_proper_user(self._method).id]
+                if len(member_sessions) >= details.limit:
+                    can_proceed = False
+            
+            elif details.per == 'channel':
+                channel_sessions = [session for session in cls._active_sessions if session.message.channel.id == self._method.channel.id] # type: ignore
+                if len(channel_sessions) >= details.limit:
+                    can_proceed = False
+        
+        if can_proceed:
+            return True
+        else:
+            await self._method.channel.send(details.message) # type: ignore
+            return False
+    
+    def _maybe_new_style(self, counter: int, total_pages: int) -> str: 
+        """Sets custom page director styles"""
+        if self.style:
+            if self.style.count('$') == 1 and self.style.count('&') == 1:
+                temp = self.style # copy it to a new variable so its not being changed in every call
+                temp = temp.replace('$', str(counter))
+                temp = temp.replace('&', str(total_pages))
+                return temp
+            else:
+                raise ImproperStyleFormat
+        else:
+            return f'Page {counter}/{total_pages}'
+    
+    async def _contact_relay(self, member: Union[discord.Member, discord.User], button: GB) -> None: # type: ignore
+        """|coro| Dispatch the information to the relay function if a relay has been set"""
+        if self._relay_info:
+            func: Callable = self._relay_info.func # type: ignore
+            only = self._relay_info.only # type: ignore
+            RelayPayload = collections.namedtuple('RelayPayload', ['member', 'button'])
+            payload = RelayPayload(member=member, button=button)
+
+            # before the information is relayed, ensure the relay function contains a single positional argument
+            spec = inspect.getfullargspec(func)
+            if all([
+                len(spec.args) == 1,
+                not spec.varargs,
+                not spec.varkw,
+                not spec.defaults,
+                not spec.kwonlyargs,
+                not spec.kwonlydefaults
+            ]):
+                async def call() -> None:
+                    """|coro| Dispatch the information to the relay function. If any errors occur during the call, report it to the user"""
+                    try:
+                        if asyncio.iscoroutinefunction(func):
+                            await func(payload)
+                        else:
+                            func(payload)
+                    except Exception as error:
+                        error_msg = inspect.cleandoc(
+                            f"""When dispatching the information to your relay function ("{func.__name__}"), that function raised an error during it's execution
+                            -> {error.__class__.__name__}: {error}
+                            """
+                        )
+                        raise MenuException(error_msg)
+
+                if only:
+                    if button in only:
+                        await call()
+                else:
+                    await call()
+            else:
+                raise MenuException('When setting a relay, the relay function must have exactly one positional argument')
+    
+    def _handle_reply_kwargs(self, send_to, reply: bool) -> dict:
+        """Used to determine the mentions for the `reply` parameter in :meth:`.start()`"""
+        if isinstance(send_to, (discord.TextChannel, discord.VoiceChannel, discord.Thread)) and send_to == self._method.channel:
+            send_to = None
+        return {
+            'reference' : self._method.message if all([send_to is None, reply is True]) else None,
+            'mention_author' : self.allowed_mentions.replied_user
+        }
+    
+    async def _handle_send_to(self, send_to: Union[str, int, discord.TextChannel, discord.VoiceChannel, discord.Thread, None], menu_payload: dict) -> None:
+        """|coro| For the :param:`send_to` kwarg in :meth:`Menu.start()`. Determine what channel the menu should start in"""
+        if isinstance(self._method, Context):
+
+            async def register_message(channel: discord.abc.Messageable) -> None:
+                """|coro| Set :attr:`_msg` to the :class:`discord.Message` that the menu is operating from"""
+                self._msg = await channel.send(**menu_payload) # type: ignore
+            
+            if self.in_dms:
+                await register_message(self._method.channel)
+            else:
+                if send_to is None:
+                    await register_message(self._method.channel)
+                else:
+                    if not isinstance(send_to, (str, int, discord.TextChannel, discord.VoiceChannel, discord.Thread)):
+                        raise IncorrectType(f'Parameter "send_to" expected str, int, discord.TextChannel, discord.VoiceChannel, or discord.Thread, got {send_to.__class__.__name__}')
+                    else:
+                        class_name = self.__class__.__name__                    # converted to list because its a sequence proxy
+                        all_messageable_channels = self._method.guild.text_channels + list(self._method.guild.threads) + self._method.guild.voice_channels # type: ignore
+                        
+                        # before we continue, check if there are any duplicate named text channels or threads/no matching names found if a str was provided
+                        if isinstance(send_to, str):
+                            matched_channels = [ch for ch in all_messageable_channels if ch.name == send_to]
+                            if len(matched_channels) == 0:
+                                raise MenuException(f'When using parameter "send_to" in {class_name}.start(), there were no channels/threads with the name {send_to!r}')
+                            
+                            elif len(matched_channels) >= 2:
+                                raise MenuException(f'When using parameter "send_to" in {class_name}.start(), there were {len(matched_channels)} channels/threads with the name {send_to!r}. With multiple channels/threads having the same name, the intended channel is unknown')
+                        
+                        for channel in all_messageable_channels:
+                            if isinstance(send_to, str):
+                                if channel.name == send_to:
+                                    await register_message(channel)
+                                    break
+                            
+                            elif isinstance(send_to, int):
+                                if channel.id == send_to:
+                                    await register_message(channel)
+                                    break
+                            
+                            # it should be a discord.TextChannel, discord.VoiceChannel, or discord.Thread
+                            else:
+                                if channel == send_to:
+                                    await register_message(channel)
+                                    break
+
+                        else:
+                            raise MenuException(f'When using parameter "send_to" in {class_name}.start(), the channel {send_to} was not found')
+        
+        elif isinstance(self._method, discord.Interaction):
+            if self._method.response.is_done():
+                await self._method.followup.send(**menu_payload)
+            else:
+                await self._method.response.send_message(**menu_payload)
+            self._msg = await self._method.original_response()
+        
+        else:
+            raise IncorrectType('Parameter "method" was not of the correct type')
+
+    def randomize_embed_colors(self) -> None:
+        """Randomize the color of all the embeds that have been added to the menu
+        
+        Raises
+        ------
+        - `MenuException`: The `menu_type` was not of `TypeEmbed`
+        
+            .. added:: v3.1.0
+        """
+        if self._menu_type == _BaseMenu.TypeEmbed:
+            for page in self._pages:
+                if page.embed:
+                    page.embed.color = discord.Color.random()
+        else:
+            raise MenuException("Randomizing embed colors can only be used when the menu_type is TypeEmbed")
+    
+    def set_page_director_style(self, style_id: int, separator: str=DEFAULT) -> None:
+        """Set how the page numbers dictating what page you are on (in the footer of an embed/regular message) are displayed
+
+        Parameters
+        ----------
+        style_id: :class:`int`
+            Varying formats of how the page director can be presented. The following ID's are available:
+
+            - `1` = Page 1/10
+            - `2` = Page 1 out of 10
+            - `3` = 1 out of 10
+            - `4` = 1 • 10
+            - `5` = 1 » 10
+            - `6` = 1 | 10
+            - `7` = 1 : 10
+            - `8` = 1 - 10
+            - `9` = 1 / 10
+            - `10` = 1 🔹 10
+            - `11` = 1 🔸 10
+        
+        separator: :class:`str`
+            The separator between the page director and any text you may have in the embed footer. The default separator is ":". It should be noted that whichever separator you assign,
+            if you wish to have spacing between the page director and the separator, you must place the space inside the string yourself as such: " :"
+        
+        Raises
+        ------
+        - `MenuException`: The :param:`style_id` value was not valid 
+        """
+        if separator:
+            self._page_director_separator = str(separator)
+        
+        if style_id == 1:   self.style = _DEFAULT_STYLE
+        elif style_id == 2: self.style = 'Page $ out of &'
+        elif style_id == 3: self.style = '$ out of &'
+        elif style_id == 4: self.style = '$ • &'
+        elif style_id == 5: self.style = '$ » &'
+        elif style_id == 6: self.style = '$ | &'
+        elif style_id == 7: self.style = '$ : &'
+        elif style_id == 8: self.style = '$ - &'
+        elif style_id == 9: self.style = '$ / &'
+        elif style_id == 10: self.style = '$ 🔹 &'
+        elif style_id == 11: self.style = '$ 🔸 &'
+        else:
+            raise MenuException(f'Parameter "style_id" expected a number 1-11, got {style_id!r}')
+    
+    async def wait_until_closed(self) -> None:
+        """|coro|
+        
+        Waits until the menu session ends using `.stop()` or when the menu times out. This should not be used inside relays
+        
+            .. added:: v3.0.1
+        """
+        await self._on_close_event.wait()
+    
+    @ensure_not_primed
+    def add_from_messages(self, messages: Sequence[discord.Message]) -> None:
+        """Add pages to the menu using the message object itself
+        
+        Parameters
+        ----------
+        messages: Sequence[:class:`discord.Message`]
+            A sequence of discord message objects
+        
+        Raises
+        ------
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        - `MenuSettingsMismatch`: The messages provided did not have the correct values. For example, the `menu_type` was set to `TypeEmbed`, but the messages you've provided only contains text. If the `menu_type` is `TypeEmbed`, only messages with embeds should be provided
+        - `IncorrectType`: All messages were not of type :class:`discord.Message`
+        """
+        if all([isinstance(msg, discord.Message) for msg in messages]):
+            if self._menu_type == _BaseMenu.TypeEmbed:
+                embeds: List[discord.Embed] = []
+                for m in messages:
+                    if m.embeds:
+                        embeds.extend(m.embeds)
+                if embeds:
+                    self.add_pages(embeds)
+                else:
+                    raise MenuSettingsMismatch(f'The menu is set to {self._menu_type.name} but no embeds were found in the messages provided')
+            
+            elif self._menu_type == _BaseMenu.TypeText:
+                content: List[str] = []
+                for m in messages:
+                    if m.content:
+                        content.append(m.content)
+                if content:
+                    self.add_pages(content)
+                else:
+                    raise MenuSettingsMismatch(f'The menu is set to {self._menu_type.name} but no text (discord.Message.content) was found in the messages provided')
+        else:
+            raise IncorrectType('All messages were not of type discord.Message')
+    
+    @ensure_not_primed
+    async def add_from_ids(self, messageable: discord.abc.Messageable, message_ids: Sequence[int]) -> None:
+        """|coro|
+        
+        Add pages to the menu using the IDs of messages. This only grabs embeds (if the `menu_type` is :attr:`TypeEmbed`) or the content (if the `menu_type` is :attr:`TypeText`) from the message
+        
+        Parameters
+        ----------
+        messageable: :class:`discord.abc.Messageable`
+            A discord :class:`Messageable` object (:class:`discord.TextChannel`, :class:`commands.Context`, etc.)
+        
+        message_ids: Sequence[:class:`int`]
+            The messages to fetch
+
+        Raises
+        ------
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        - `MenuSettingsMismatch`: The message IDs provided did not have the correct values when fetched. For example, the `menu_type` was set to `TypeEmbed`, but the messages you've provided for the library to fetch only contains text. If the `menu_type` is `TypeEmbed`, only messages with embeds should be provided
+        - `MenuException`: An error occurred when attempting to fetch a message or not all :param:`message_ids` were of type int
+        """
+        if all([isinstance(ID, int) for ID in message_ids]):
+            to_paginate: List[discord.Message] = []            
+            for msg_id in message_ids:
+                try:
+                    fetched_message = await messageable.fetch_message(msg_id)
+                    to_paginate.append(fetched_message)
+                except (discord.NotFound, discord.Forbidden, discord.HTTPException) as error:
+                    raise MenuException(f'An error occurred when attempting to retrieve message with the ID {msg_id}: {error}')
+            
+            if self._menu_type == _BaseMenu.TypeEmbed:
+                embeds_to_paginate: List[discord.Embed] = []
+                for msg in to_paginate:
+                    if msg.embeds:
+                        embeds_to_paginate.extend(msg.embeds)
+                if embeds_to_paginate:
+                    for embed in embeds_to_paginate:
+                        self.add_page(embed)
+                else:
+                    raise MenuSettingsMismatch(f'The menu is set to {self._menu_type.name} but no embeds were found in the messages provided')
+            
+            elif self._menu_type == _BaseMenu.TypeText:
+                content_to_paginate: List[str] = []
+                for msg in to_paginate:
+                    if msg.content:
+                        content_to_paginate.append(msg.content)
+                if content_to_paginate:
+                    for content in content_to_paginate:
+                        self.add_page(content=content)
+                else:
+                    raise MenuSettingsMismatch(f'The menu is set to {self._menu_type.name} but no text (discord.Message.content) was found in the messages provided')
+        else:
+            raise MenuException('Not all message IDs were of type int')
+    
+    @ensure_not_primed
+    def clear_all_row_data(self) -> None:
+        """Delete all the data thats been added using :meth:`add_row()`
+        
+        Raises
+        ------
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        - `MenuSettingsMismatch`: This method was called but the menus `menu_type` was not :attr:`TypeEmbedDynamic`
+        """
+        if self._menu_type == _BaseMenu.TypeEmbedDynamic:
+            self._dynamic_data_builder.clear()
+        else:
+            raise MenuSettingsMismatch('Cannot clear all row data when the menu_type is not set as TypeEmbedDynamic')
+    
+    @ensure_not_primed
+    def add_row(self, data: str) -> None:
+        """Add text to the embed page by rows of data
+        
+        Parameters
+        ----------
+        data: :class:`str`
+            The data to add
+        
+        Raises
+        ------
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        - `MenuSettingsMismatch`: This method was called but the menus `menu_type` was not :attr:`TypeEmbedDynamic`
+        - `MissingSetting`: The kwarg "rows_requested" (int) has not been set for the menu
+        """
+        if self._menu_type == _BaseMenu.TypeEmbedDynamic:
+            if self.rows_requested:
+                self._dynamic_data_builder.append(str(data))
+            else:
+                raise MissingSetting('The kwarg "rows_requested" (int) has not been set for the menu')
+        else:
+            raise MenuSettingsMismatch('add_row() can only be used with a menu_type of TypeEmbedDynamic')
+    
+    @ensure_not_primed
+    def set_main_pages(self, *embeds: discord.Embed) -> None:
+        """On a menu with a `menu_type` of :attr:`TypeEmbedDynamic`, set the pages you would like to show first. These embeds will be shown before the embeds that contain your data
+        
+        Parameters
+        ----------
+        *embeds: :class:`discord.Embed`
+            An argument list of :class:`discord.Embed` objects
+        
+        Raises
+        ------
+        - `MenuSettingsMismatch`: Tried to use method on a menu that was not of `menu_type` :attr:`TypeEmbedDynamic`
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        - `MenuException`: The "embeds" parameter was empty. At least one value is needed
+        - `IncorrectType`: All values in the argument list were not of type :class:`discord.Embed`
+        """
+        if not embeds: raise MenuException('The argument list when setting main pages was empty')
+        if not all([isinstance(e, discord.Embed) for e in embeds]): raise IncorrectType('All values in the argument list when setting main pages were not of type discord.Embed')
+        if self._menu_type != _BaseMenu.TypeEmbedDynamic: raise MenuSettingsMismatch('Method set_main_pages is only available for menus with menu_type TypeEmbedDynamic')
+        
+        # if they've set any values, remove it. Each set should be from the call and should not stack
+        self._main_page_contents.clear()
+        
+        for embed in embeds:
+            self._main_page_contents.append(embed)
+
+    @ensure_not_primed
+    def set_last_pages(self, *embeds: discord.Embed) -> None:
+        """On a menu with a `menu_type` of :attr:`TypeEmbedDynamic`, set the pages you would like to show last. These embeds will be shown after the embeds that contain your data
+        
+        Parameters
+        ----------
+        *embeds: :class:`discord.Embed`
+            An argument list of :class:`discord.Embed` objects
+        
+        Raises
+        ------
+        - `MenuSettingsMismatch`: Tried to use method on a menu that was not of `menu_type` :attr:`TypeEmbedDynamic`
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        - `MenuException`: The "embeds" parameter was empty. At least one value is needed
+        - `IncorrectType`: All values in the argument list were not of type :class:`discord.Embed`
+        """
+        if not embeds: raise MenuException('The argument list when setting last pages was empty')
+        if not all([isinstance(e, discord.Embed) for e in embeds]): raise IncorrectType('All values in the argument list when setting last pages were not of type discord.Embed')
+        if self._menu_type != _BaseMenu.TypeEmbedDynamic: raise MenuSettingsMismatch('Method set_last_pages is only available for menus with menu_type TypeEmbedDynamic')
+        
+        # if they've set any values, remove it. Each set should be from the call and should not stack
+        self._last_page_contents.clear()
+        
+        for embed in embeds:
+            self._last_page_contents.append(embed)
+    
+    @ensure_not_primed
+    def add_page(self, embed: Optional[discord.Embed]=MISSING, content: Optional[str]=None, files: Optional[List[discord.File]]=MISSING) -> None:
+        """Add a page to the menu
+
+        Parameters
+        ----------
+        embed: Optional[:class:`discord.Embed`]
+            The embed of the page
+        
+        content: Optional[:class:`str`]
+            The text that appears above an embed in a message
+        
+        files: Optional[Sequence[:class:`discord.File`]]
+            Files you'd like to attach to the page
+        
+        Raises
+        ------
+        - `MenuException`: Attempted to add a page with no parameters
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        - `MenuSettingsMismatch`: The page being added does not match the menus `menu_type` 
+        
+            .. changes::
+                v3.1.0
+                    Added parameter content
+                    Added parameter embed
+                    Added parameter files
+                    Removed parameter "page"
+        """
+        if all([content is None, embed is None, files is None]):
+            raise MenuException("When adding a page, at lease one parameter must be set")
+        
+        cls = self.__class__
+        if self._menu_type == cls.TypeEmbed:
+            if isinstance(embed, discord.Embed):
+                self._pages.append(Page(content=content, embed=embed, files=files))
+            else:
+                raise MenuSettingsMismatch(f'When adding a page with a menu_type of TypeEmbed, the "embed" parameter cannot be None')
+        
+        elif self._menu_type == cls.TypeText:
+            if content:
+                self._pages.append(Page(content=str(content), files=files))
+            else:
+                raise MenuSettingsMismatch(f'When adding a page with a menu_type of TypeText, the "content" parameter cannot be None')
+        
+        else:
+            raise MenuSettingsMismatch('add_page method cannot be used with the current menu_type')
+    
+    @overload
+    def add_pages(self, pages: Sequence[discord.Embed]) -> None:
+        ...
+    
+    @overload
+    def add_pages(self, pages: Sequence[str]) -> None:
+        ...
+
+    @ensure_not_primed
+    def add_pages(self, pages: Sequence[Union[discord.Embed, str]]) -> None:
+        """Add multiple pages to the menu at once
+        
+        Parameters
+        ----------
+        pages: Sequence[Union[:class:`discord.Embed`, :class:`str`]]
+            The pages to add. Can only be used when the menus `menu_type` is :attr:`TypeEmbed` (adding a :class:`discord.Embed`)
+            or :attr:`TypeText` (adding a :class:`str`)
+        
+        Raises
+        ------
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        - `MenuSettingsMismatch`: The page being added does not match the menus `menu_type` 
+        """
+        for embed_or_str in pages:
+            if isinstance(embed_or_str, str):
+                self.add_page(content=embed_or_str)
+            else:
+                self.add_page(embed_or_str) # type: ignore
+    
+    @ensure_not_primed
+    def remove_all_pages(self) -> None:
+        """Remove all pages from the menu
+        
+        Raises
+        ------
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        """
+        self._pages.clear()
+    
+    @ensure_not_primed
+    def remove_page(self, page_number: int) -> None:
+        """Remove a page from the menu
+        
+        Parameters
+        ----------
+        page_number: :class:`int`
+            The page to remove
+        
+        Raises
+        ------
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        - `InvalidPage`: The page associated with the given page number was not valid
+        """
+        if self._pages:
+            if page_number > 0 and page_number <= len(self._pages):
+                page_to_delete = page_number - 1
+                del self._pages[page_to_delete]
+            else:
+                raise InvalidPage(f'Page number invalid. Must be from 1 - {len(self._pages)}')
+    
+    def set_on_timeout(self, func: Callable[[M], None]) -> None:
+        """Set the function to be called when the menu times out
+
+        Parameters
+        ----------
+        func: Callable[[:type:`M`]], :class:`None`]
+            The function object that will be called when the menu times out. The function should contain a single positional argument
+            and should not return anything. The argument passed to that function is an instance of the menu.
+        
+        Raises
+        ------
+        - `IncorrectType`: Parameter "func" was not a callable object
+        """
+        if not callable(func): raise IncorrectType('Parameter "func" must be callable')
+        self._on_timeout_details = func # type: ignore
+    
+    def remove_on_timeout(self) -> None:
+        """Remove the timeout call to the function you have set when the menu times out"""
+        self._on_timeout_details = None
+    
+    def set_relay(self, func: Callable[[NamedTuple], None], *, only: Optional[List[GB]]=None) -> None:
+        """Set a function to be called with a given set of information when a button is pressed on the menu. The information passed is `RelayPayload`, a named tuple.
+        The named tuple contains the following attributes:
+
+        - `member`: The :class:`discord.Member` object of the person who pressed the button. Could be :class:`discord.User` if the menu was started in a DM
+        - `button`: Depending on the menu instance, the :class:`ReactionButton` or :class:`ViewButton` object of the button that was pressed
+
+        Parameters
+        ----------
+        func: Callable[[:class:`NamedTuple`], :class:`None`]
+            The function should only contain a single positional argument. Command functions (`@bot.command()`) not supported
+        
+        only: Optional[List[:generic:`GB`]]
+            A list of buttons (`GB`) associated with the current menu instance. If the menu instance is :class:`ReactionMenu`, this should be a list of :class:`ReactionButton`
+            and vice-versa for :class:`ViewMenu` instances. If this is :class:`None`, all buttons on the menu will be relayed. If set, only button presses from those specified buttons will be relayed
+        
+        Raises
+        ------
+        - `IncorrectType`: The :param:`func` argument provided was not callable
+        """
+        if callable(func):
+            RelayInfo = collections.namedtuple('RelayInfo', ['func', 'only'])
+            self._relay_info = RelayInfo(func=func, only=only)
+        else:
+            raise IncorrectType('When setting the relay, argument "func" must be callable')
+    
+    def remove_relay(self) -> None:
+        """Remove the relay that's been set"""
+        self._relay_info = None
```

### Comparing `reactionmenu-3.1.3/reactionmenu/buttons.py` & `reactionmenu-3.1.4/reactionmenu/buttons.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,667 +1,667 @@
-"""
-MIT License
-
-Copyright (c) 2021-present Defxult#8269
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
-DEALINGS IN THE SOFTWARE.
-"""
-
-from __future__ import annotations
-
-from typing import (
-	TYPE_CHECKING,
-	Any,
-	Callable,
-	Dict,
-	Final,
-	Iterable,
-	List,
-	Literal,
-	NamedTuple,
-	Optional,
-	Tuple,
-	Union
-)
-
-if TYPE_CHECKING:
-	from . import ViewMenu, ReactionButton, ReactionMenu
-
-import re
-from enum import auto, Enum
-
-import discord
-from discord.ext.commands import Command
-
-from .abc import _BaseButton, PaginationEmojis
-from .errors import IncorrectType
-
-
-class _Details(NamedTuple):
-	"""Used for buttons with a `custom_id` of `ID_CALLER`"""
-	func: Callable[..., None]
-	args: Iterable[Any]
-	kwargs: Dict[str, Any]
-
-Details = _Details
-
-class ViewButton(discord.ui.Button, _BaseButton):
-	"""A helper class for :class:`ViewMenu`. Represents a UI button.
-	
-	Parameters
-	----------
-	style: :class:`discord.ButtonStyle`
-		The style of the button
-	
-	label: Optional[:class:`str`]
-		The button label, if any
-	
-	disabled: :class:`bool`
-		Whether the button is disabled or not
-	
-	custom_id: Optional[:class:`str`]
-		The ID of the button that gets received during an interaction. If this button is for a URL, it does not have a custom ID
-	
-	url: Optional[:class:`str`]
-		The URL this button sends you to
-	
-	emoji: Optional[Union[:class:`str`, :class:`discord.PartialEmoji`]]
-		The emoji of the button, if available
-	
-	followup: Optional[:class:`ViewButton.Follow`]
-		Used with buttons with custom_id :attr:`ViewButton.ID_CALLER`, :attr:`ViewButton.ID_SEND_MESSAGE`, :attr:`ViewButton.ID_CUSTOM_EMBED`
-	
-	event: Optional[:class:`ViewButton.Event`]
-		Set the button to be disabled or removed when it has been pressed a certain amount of times
-	
-	Kwargs
-	------
-	name: :class:`str`
-		An optional name for the button. Can be set to retrieve it later via :meth:`ViewMenu.get_button()`
-	
-	skip: :class:`ViewButton.Skip`
-		Set the action and the amount of pages to skip when using a `custom_id` of `ViewButton.ID_SKIP`
-	
-	persist: :class:`bool`
-		Available only when using link buttons. This prevents link buttons from being disabled/removed when the menu times out or is stopped so they can remain clickable
-	
-		.. added v3.1.0
-			:param:`persist`
-	"""
-	ID_NEXT_PAGE: Final[str] = '0'
-	ID_PREVIOUS_PAGE: Final[str] = '1'
-	ID_GO_TO_FIRST_PAGE: Final[str] = '2'
-	ID_GO_TO_LAST_PAGE: Final[str] = '3'
-	ID_GO_TO_PAGE: Final[str] = '4'
-	ID_END_SESSION: Final[str] = '5'
-	ID_CALLER: Final[str] = '6'
-	ID_SEND_MESSAGE: Final[str] = '7'
-	ID_CUSTOM_EMBED: Final[str] = '8'
-	ID_SKIP: Final[str] = '9'
-
-	_RE_IDs = r'[0-9]|[0-9]_\d+'
-	_RE_UNIQUE_ID_SET = r'_\d+'
-
-	def __init__(
-		self,
-		*,
-		style: discord.ButtonStyle=discord.ButtonStyle.secondary,
-		label: Optional[str]=None,
-		disabled: bool=False,
-		custom_id: Optional[str]=None,
-		url: Optional[str]=None,
-		emoji: Optional[Union[str, discord.PartialEmoji]]=None,
-		followup: Optional[ViewButton.Followup]=None,
-		event: Optional[ViewButton.Event]=None,
-		**kwargs
-		):
-		super().__init__(style=style, label=label, disabled=disabled, custom_id=custom_id, url=url, emoji=emoji, row=None)
-		_BaseButton.__init__(self, name=kwargs.get('name'), event=event, skip=kwargs.get('skip')) # type: ignore
-		self.followup = followup
-		self.persist: bool = kwargs.get('persist', False)
-		
-		# abc
-		self._menu: Optional[ViewMenu] = None
-	
-	def __repr__(self):
-		total_clicks = '' if self.style == discord.ButtonStyle.link else f' total_clicks={self.total_clicks}'
-		is_link_button = True if self.style == discord.ButtonStyle.link else False
-		return f'<ViewButton label={self.label!r} custom_id={ViewButton._get_id_name_from_id(str(self.custom_id), is_link_button=is_link_button)} style={self.style} emoji={self.emoji!r} url={self.url} disabled={self.disabled}{total_clicks}>'
-
-	async def callback(self, interaction: discord.Interaction) -> None:
-		"""*INTERNAL USE ONLY* - The callback function from the button interaction. This should not be manually called"""
-		await self._menu._paginate(self, interaction) # type: ignore
-	
-	class Followup:
-		"""A class that represents the message sent using a :class:`ViewButton`. Contains parameters similar to method `discord.abc.Messageable.send`. Only to be used with :class:`ViewButton` kwarg "followup".
-		It is to be noted that this should not be used with :class:`ViewButton` with a "style" of `discord.ButtonStyle.link` because link buttons do not send interaction events.
-		
-		Parameters
-		----------
-		content: Optional[:class:`str`]
-			Message to send
-		
-		embed: Optional[:class:`discord.Embed`]
-			Embed to send. Can also bet set for buttons with a custom_id of :attr:`ViewButton.ID_CUSTOM_EMBED`
-		
-		file: Optional[:class:`discord.File`]
-			File to send. If the :class:`ViewButton` custom_id is :attr:`ViewButton.ID_SEND_MESSAGE`, the file will be ignored because of discord API limitations
-		
-		tts: :class:`bool`
-			If discord should read the message aloud. Not valid for `ephemeral` messages
-		
-		allowed_mentions: Optional[:class:`discord.AllowedMentions`]
-			Controls the mentions being processed in the menu message. Not valid for `ephemeral` messages
-		
-		delete_after: Optional[Union[:class:`int`, :class:`float`]]
-			Amount of time to wait before the message is deleted. Not valid for `ephemeral` messages
-		
-		ephemeral: :class:`bool`
-			If the message will be hidden from everyone except the person that pressed the button. This is only valid for a :class:`ViewButton` with custom_id :attr:`ViewButton.ID_SEND_MESSAGE`
-		
-		Kwargs
-		------
-		details: :meth:`ViewButton.Followup.set_caller_details()`
-			The information that will be used when a `ViewButton.ID_CALLER` button is pressed (defaults to :class:`None`)
-		"""
-		
-		__slots__ = ('content', 'embed', 'file', 'tts', 'allowed_mentions', 'delete_after', 'ephemeral', 'details')
-
-		def __repr__(self):
-			x = []
-			for val in self.__class__.__slots__:
-				temp = getattr(self, val)
-				if temp:
-					x.append(f'{val}={temp!r}')
-			
-			return f'<Followup {" ".join(x)}>'
-
-		def __init__(
-			self,
-			content: Optional[str]=None, 
-			*,
-			embed: Optional[discord.Embed]=None,
-			file: Optional[discord.File]=None,
-			tts: bool=False,
-			allowed_mentions: Optional[discord.AllowedMentions]=None,
-			delete_after: Optional[Union[int, float]]=None,
-			ephemeral: bool=False,
-			**kwargs
-			):
-			self.content = content
-			self.embed = embed
-			self.file = file
-			self.tts = tts
-			self.allowed_mentions = allowed_mentions
-			self.delete_after = delete_after
-			self.ephemeral = ephemeral
-			self.details: Optional[Details] = kwargs.get('details')
-		
-		def _to_dict(self) -> dict:
-			"""This is a :class:`ViewButton.Followup` method"""
-			new = {}
-			for i in self.__slots__:
-				new[i] = getattr(self, i)
-			return new
-		
-		@staticmethod
-		def set_caller_details(func: Callable[..., None], *args, **kwargs) -> Details:
-			"""|static method|
-			
-			Set the parameters for the function you set for a :class:`ViewButton` with the custom_id :attr:`ViewButton.ID_CALLER`
-			
-			Parameters
-			----------
-			func: Callable[..., :class:`None`]
-				The function object that will be called when the associated button is pressed
-			
-			*args: `Any`
-				An argument list that represents the parameters of that function
-			
-			**kwargs: `Any`
-				An argument list that represents the kwarg parameters of that function
-			
-			Returns
-			-------
-			:class:`Details`: The :class:`NamedTuple` containing the values needed to internally call the function you have set
-			
-			Raises
-			------
-			- `IncorrectType`: Parameter "func" was not a callable object
-			"""
-			if callable(func):
-				func = func.callback if isinstance(func, Command) else func
-				return Details(func=func, args=args, kwargs=kwargs)
-			else:
-				raise IncorrectType('Parameter "func" must be callable')
-
-	@classmethod
-	def _base_nav_buttons(cls) -> Tuple[str, str, str, str, str]:
-		return (cls.ID_PREVIOUS_PAGE, cls.ID_NEXT_PAGE, cls.ID_GO_TO_FIRST_PAGE, cls.ID_GO_TO_LAST_PAGE, cls.ID_GO_TO_PAGE)
-	
-	@classmethod
-	def _get_id_name_from_id(cls, id_: str, **kwargs) -> str:
-		# if its a CALLER, SEND_MESSAGE, or CUSTOM_EMBED id, convert to it's true representation, because when passed, it's form is "[ButtonID]_[unique ID]"
-		# see :meth:`_button_add_check` or :meth:`_maybe_custom_id` for details
-
-		is_link_button = kwargs.get('is_link_button', False)
-		if is_link_button:
-			return 'LINK_BUTTON'
-		
-		unique_id_set = re.compile(ViewButton._RE_UNIQUE_ID_SET)
-		if re.search(unique_id_set, id_):
-			id_ = re.sub(unique_id_set, '', id_)
-		
-		for key, val in cls.__dict__.items():
-			if id_ == val:
-				return f'ViewButton.{key}'
-		
-		assert False, "id name could not be found"
-	
-	@property
-	def menu(self) -> Optional[ViewMenu]:
-		"""
-		Returns
-		-------
-		Optional[:class:`ViewMenu`]: The menu instance this button is attached to. Could be :class:`None` if the button is not attached to a menu
-		"""
-		return self._menu
-	
-	@classmethod
-	def generate_skip(cls, label: str, action: Literal['+', '-'], amount: int) -> ViewButton:
-		"""|class method|
-		
-		A factory method that returns a :class:`ViewButton` with the following parameters set:
-		
-		- style: `discord.ButtonStyle.gray`
-		- label: `<label>`
-		- custom_id: :attr:`ViewButton.ID_SKIP`
-		- skip: `ViewButton.Skip(<action>, <amount>)`
-		"""
-		return cls(style=discord.ButtonStyle.gray, label=label, custom_id=cls.ID_SKIP, skip=cls.Skip(action, amount))
-	
-	@classmethod
-	def link(cls, label: str, url: str) -> ViewButton:
-		"""|class method|
-		
-		A factory method that returns a :class:`ViewButton` with the following parameters set:
-		
-		- style: `discord.ButtonStyle.link`
-		- label: `<label>`
-		- url: `<url>`
-		"""
-		return cls(style=discord.ButtonStyle.link, label=str(label), url=str(url))
-	
-	@classmethod
-	def back(cls) -> ViewButton:
-		"""|class method|
-		
-		A factory method that returns a :class:`ViewButton` with the following parameters set:
-		
-		- style: `discord.ButtonStyle.gray`
-		- label: "Back"
-		- custom_id: :attr:`ViewButton.ID_PREVIOUS_PAGE`
-		"""
-		return cls(style=discord.ButtonStyle.gray, label='Back', custom_id=cls.ID_PREVIOUS_PAGE)
-	
-	@classmethod
-	def next(cls) -> ViewButton:
-		"""|class method|
-		
-		A factory method that returns a :class:`ViewButton` with the following parameters set:
-		
-		- style: `discord.ButtonStyle.gray`
-		- label: "Next"
-		- custom_id: :attr:`ViewButton.ID_NEXT_PAGE`
-		"""
-		return cls(style=discord.ButtonStyle.gray, label='Next', custom_id=cls.ID_NEXT_PAGE)
-	
-	@classmethod
-	def go_to_first_page(cls) -> ViewButton:
-		"""|class method|
-		
-		A factory method that returns a :class:`ViewButton` with the following parameters set:
-		
-		- style: `discord.ButtonStyle.gray`
-		- label: "First Page"
-		- custom_id: :attr:`ViewButton.ID_GO_TO_FIRST_PAGE`
-		"""
-		return cls(style=discord.ButtonStyle.gray, label='First Page', custom_id=cls.ID_GO_TO_FIRST_PAGE)
-	
-	@classmethod
-	def go_to_last_page(cls) -> ViewButton:
-		"""|class method|
-		
-		A factory method that returns a :class:`ViewButton` with the following parameters set:
-		
-		- style: `discord.ButtonStyle.gray`
-		- label: "Last Page"
-		- custom_id: :attr:`ViewButton.ID_GO_TO_LAST_PAGE`
-		"""
-		return cls(style=discord.ButtonStyle.gray, label='Last Page', custom_id=cls.ID_GO_TO_LAST_PAGE)
-	
-	@classmethod
-	def go_to_page(cls) -> ViewButton:
-		"""|class method|
-		
-		A factory method that returns a :class:`ViewButton` with the following parameters set:
-		
-		- style: `discord.ButtonStyle.gray`
-		- label: "Page Selection"
-		- custom_id: :attr:`ViewButton.ID_GO_TO_PAGE`
-		"""
-		return cls(style=discord.ButtonStyle.gray, label='Page Selection', custom_id=cls.ID_GO_TO_PAGE)
-	
-	@classmethod
-	def end_session(cls) -> ViewButton:
-		"""|class method|
-		
-		A factory method that returns a :class:`ViewButton` with the following parameters set:
-		
-		- style: `discord.ButtonStyle.gray`
-		- label: "Close"
-		- custom_id: :attr:`ViewButton.ID_END_SESSION`
-		"""
-		return cls(style=discord.ButtonStyle.gray, label='Close', custom_id=cls.ID_END_SESSION)
-	
-	@classmethod
-	def all(cls) -> List[ViewButton]:
-		"""|class method|
-		
-		A factory method that returns a list of all base navigation buttons. The following buttons are returned with pre-set values:
-		
-		- Button 1
-			- style: `discord.ButtonStyle.gray`
-			- label: "First Page"
-			- custom_id: :attr:`ViewButton.ID_GO_TO_FIRST_PAGE`
-		- Button 2
-			- style: `discord.ButtonStyle.gray`
-			- label: "Back"
-			- custom_id: :attr:`ViewButton.ID_PREVIOUS_PAGE`
-		- Button 3
-			- style: `discord.ButtonStyle.gray`
-			- label: "Next"
-			- custom_id: :attr:`ViewButton.ID_NEXT_PAGE`
-		- Button 4
-			- style: `discord.ButtonStyle.gray`
-			- label: "Last Page"
-			- custom_id: :attr:`ViewButton.ID_GO_TO_LAST_PAGE`
-		- Button 5
-			- style: `discord.ButtonStyle.gray`
-			- label: "Page Selection"
-			- custom_id: :attr:`ViewButton.ID_GO_TO_PAGE`
-		- Button 6
-			- style: `discord.ButtonStyle.gray`
-			- label: "Close"
-			- custom_id: :attr:`ViewButton.ID_END_SESSION`
-
-		They are returned in that order
-		
-		Returns
-		-------
-		List[:class:`ViewButton`]
-		"""
-		return [cls.go_to_first_page(), cls.back(), cls.next(), cls.go_to_last_page(), cls.go_to_page(), cls.end_session()]
-	
-	@classmethod
-	def all_with_emojis(cls) -> List[ViewButton]:
-		"""|class method|
-		
-		A factory method that returns a list of all base navigation buttons with emojis assigned instead of labels. The following buttons are returned with pre-set values:
-		
-		- Button 1
-			- style: `discord.ButtonStyle.gray`
-			- emoji: ⏪
-			- custom_id: :attr:`ViewButton.ID_GO_TO_FIRST_PAGE`
-		- Button 2
-			- style: `discord.ButtonStyle.gray`
-			- emoji: ◀️
-			- custom_id: :attr:`ViewButton.ID_PREVIOUS_PAGE`
-		- Button 3
-			- style: `discord.ButtonStyle.gray`
-			- emoji: ▶️
-			- custom_id: :attr:`ViewButton.ID_NEXT_PAGE`
-		- Button 4
-			- style: `discord.ButtonStyle.gray`
-			- emoji: ⏩
-			- custom_id: :attr:`ViewButton.ID_GO_TO_LAST_PAGE`
-		- Button 5
-			- style: `discord.ButtonStyle.gray`
-			- emoji: 🔢
-			- custom_id: :attr:`ViewButton.ID_GO_TO_PAGE`
-		- Button 6
-			- style: `discord.ButtonStyle.gray`
-			- emoji: ⏹️
-			- custom_id: :attr:`ViewButton.ID_END_SESSION`
-
-		They are returned in that order
-		
-		Returns
-		-------
-		List[:class:`ViewButton`]
-
-			.. added:: v3.1.0
-		"""
-		return [
-			cls(style=discord.ButtonStyle.gray, emoji='⏪', custom_id=cls.ID_GO_TO_FIRST_PAGE),
-			cls(style=discord.ButtonStyle.gray, emoji='◀️', custom_id=cls.ID_PREVIOUS_PAGE),
-			cls(style=discord.ButtonStyle.gray, emoji='▶️', custom_id=cls.ID_NEXT_PAGE),
-			cls(style=discord.ButtonStyle.gray, emoji='⏩', custom_id=cls.ID_GO_TO_LAST_PAGE),
-			cls(style=discord.ButtonStyle.gray, emoji='🔢', custom_id=cls.ID_GO_TO_PAGE),
-			cls(style=discord.ButtonStyle.gray, emoji='⏹️', custom_id=cls.ID_END_SESSION)
-		]
-
-class ButtonType(Enum):
-	"""A helper class for :class:`ReactionMenu`. Determines the generic action a button can perform."""
-	NEXT_PAGE = auto()
-	PREVIOUS_PAGE = auto()
-	GO_TO_FIRST_PAGE = auto()
-	GO_TO_LAST_PAGE = auto()
-	GO_TO_PAGE = auto()
-	END_SESSION = auto()
-	CUSTOM_EMBED = auto()
-	CALLER = auto()
-	SKIP = auto()
-
-	@staticmethod
-	def _get_buttontype_name_from_type(type_: ButtonType) -> str:
-		"""|static method| Used to determine the `linked_to` type. Returns the full :class:`str` representation of that type"""
-		return f'{type_.__class__.__name__}.{type_.name}'
-
-class ReactionButton(_BaseButton):
-	"""A helper class for :class:`ReactionMenu`. Represents a reaction.
-	
-	Parameters
-	----------
-	emoji: :class:`str`
-		The discord reaction that will be used
-
-	linked_to: :class:`ReactionButton.Type`
-		A generic action a button can perform
-	
-	Kwargs
-	------
-	embed: :class:`discord.Embed`
-		Only used when :param:`linked_to` is set as :attr:`ReactionButton.Type.CUSTOM_EMBED`. This is the embed that can be selected separately from the menu (`TypeEmbed` menu's only)
-
-	name: :class:`str`
-		An optional name for the button. Can be set to retrieve it later via :meth:`ReactionMenu.get_button()`
-
-	details: :meth:`ReactionButton.set_caller_details()`
-		The class method used to set the function and it's arguments to be called when the button is pressed
-	
-	event: :class:`ReactionButton.Event`
-		Determine when a button should be removed depending on how many times it has been pressed
-
-	skip: :class:`ReactionButton.Skip`
-		Set the action and the amount of pages to skip when using a `linked_to` of `ReactionButton.Type.SKIP`
-	"""
-
-	Type = ButtonType
-
-	def __init__(self, *, emoji: str, linked_to: ReactionButton.Type, **kwargs):
-		super().__init__(name=kwargs.get('name'), event=kwargs.get('event'), skip=kwargs.get('skip')) # type: ignore
-		self.emoji = str(emoji)
-		self.linked_to = linked_to
-		
-		self.custom_embed: Optional[discord.Embed] = kwargs.get('embed')
-		self.details: Optional[Details] = kwargs.get('details')
-		
-		# abc
-		self._menu: Optional[ReactionMenu] = None
-	
-	def __str__(self):
-		return self.emoji
-	
-	def __repr__(self):
-		return f'<ReactionButton emoji={self.emoji!r} linked_to={ButtonType._get_buttontype_name_from_type(self.linked_to)} total_clicks={self.total_clicks} name={self.name!r}>'
-	
-	@property
-	def menu(self) -> Optional[ReactionMenu]:
-		"""
-		Returns
-		-------
-		Optional[:class:`ReactionMenu`]: The menu the button is currently operating under. Can be :class:`None` if the button is not registered to a menu
-		"""
-		return self._menu
-	
-	@staticmethod
-	def set_caller_details(func: Callable[..., None], *args, **kwargs) -> Details:
-		"""|static method|
-		
-		Set the parameters for the function you set for a :class:`ReactionButton` with a `linked_to` of :attr:`ReactionButton.Type.CALLER`
-
-		Parameters
-		----------
-		func: Callable[..., :class:`None`]
-			The function object that will be called when the associated button is pressed
-		
-		*args: `Any`
-			An argument list that represents the parameters of that function
-		
-		**kwargs: `Any`
-			An argument list that represents the kwarg parameters of that function
-		
-		Returns
-		-------
-		:class:`Details`: The :class:`NamedTuple` containing the values needed to internally call the function you have set
-		
-		Raises
-		------
-		- `IncorrectType`: Parameter "func" was not a callable object
-		"""
-		if callable(func):
-			func = func.callback if isinstance(func, Command) else func
-			return Details(func=func, args=args, kwargs=kwargs)
-		else:
-			raise IncorrectType('Parameter "func" must be callable')
-	
-	@classmethod
-	def generate_skip(cls, emoji: str, action: Literal['+', '-'], amount: int) -> ReactionButton:
-		"""|class method|
-		
-		A factory method that returns a :class:`ReactionButton` with the following parameters set:
-		
-		- emoji: `<emoji>`
-		- linked_to: :attr:`ReactionButton.Type.SKIP`
-		- skip: `ReactionButton.Skip(<action>, <amount>)`
-		"""
-		return cls(emoji=emoji, linked_to=cls.Type.SKIP, skip=cls.Skip(action, amount))
-	
-	@classmethod
-	def back(cls) -> ReactionButton:
-		"""|class method|
-		
-		A factory method that returns a :class:`ReactionButton` with the following parameters set:
-		
-		- emoji: ◀️
-		- linked_to: :attr:`ReactionButton.Type.PREVIOUS_PAGE`
-		"""
-		return cls(emoji=PaginationEmojis.BACK_BUTTON, linked_to=cls.Type.PREVIOUS_PAGE)
-	
-	@classmethod
-	def next(cls) -> ReactionButton:
-		"""|class method|
-		
-		A factory method that returns a :class:`ReactionButton` with the following parameters set:
-		
-		- emoji: ▶️
-		- linked_to: :attr:`ReactionButton.Type.NEXT_PAGE`
-		"""
-		return cls(emoji=PaginationEmojis.NEXT_BUTTON, linked_to=cls.Type.NEXT_PAGE)
-	
-	@classmethod
-	def go_to_first_page(cls) -> ReactionButton:
-		"""|class method|
-		
-		A factory method that returns a :class:`ReactionButton` with the following parameters set:
-		
-		- emoji: ⏪
-		- linked_to: :attr:`ReactionButton.Type.GO_TO_FIRST_PAGE`
-		"""
-		return cls(emoji=PaginationEmojis.FIRST_PAGE, linked_to=cls.Type.GO_TO_FIRST_PAGE)
-	
-	@classmethod
-	def go_to_last_page(cls) -> ReactionButton:
-		"""|class method|
-		
-		A factory method that returns a :class:`ReactionButton` with the following parameters set:
-		
-		- emoji: ⏩
-		- linked_to: :attr:`ReactionButton.Type.GO_TO_LAST_PAGE`
-		"""
-		return cls(emoji=PaginationEmojis.LAST_PAGE, linked_to=cls.Type.GO_TO_LAST_PAGE)
-	
-	@classmethod
-	def go_to_page(cls) -> ReactionButton:
-		"""|class method|
-		
-		A factory method that returns a :class:`ReactionButton` with the following parameters set:
-		
-		- emoji: 🔢
-		- linked_to: :attr:`ReactionButton.Type.GO_TO_PAGE`
-		"""
-		return cls(emoji=PaginationEmojis.GO_TO_PAGE, linked_to=cls.Type.GO_TO_PAGE)
-	
-	@classmethod
-	def end_session(cls) -> ReactionButton:
-		"""|class method|
-		
-		A factory method that returns a :class:`ReactionButton` with the following parameters set:
-		
-		- emoji: ⏹️
-		- linked_to: :attr:`ReactionButton.Type.END_SESSION`
-		"""
-		return cls(emoji=PaginationEmojis.END_SESSION, linked_to=cls.Type.END_SESSION)
-	
-	@classmethod
-	def all(cls) -> List[ReactionButton]:
-		"""|class method|
-		
-		A factory method that returns a `list` of all base navigation buttons. Base navigation buttons are :class:`ReactionButton` with a `linked_to` of:
-		
-		- :attr:`ReactionButton.Type.GO_TO_FIRST_PAGE`
-		- :attr:`ReactionButton.Type.PREVIOUS_PAGE`
-		- :attr:`ReactionButton.Type.NEXT_PAGE`
-		- :attr:`ReactionButton.Type.GO_TO_LAST_PAGE`
-		- :attr:`ReactionButton.Type.GO_TO_PAGE`
-		- :attr:`ReactionButton.Type.END_SESSION`
-
-		They are returned in that order
-		"""
-		return [cls.go_to_first_page(), cls.back(), cls.next(), cls.go_to_last_page(), cls.go_to_page(), cls.end_session()]
+"""
+MIT License
+
+Copyright (c) 2021-present Defxult#8269
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+from typing import (
+	TYPE_CHECKING,
+	Any,
+	Callable,
+	Dict,
+	Final,
+	Iterable,
+	List,
+	Literal,
+	NamedTuple,
+	Optional,
+	Tuple,
+	Union
+)
+
+if TYPE_CHECKING:
+	from . import ViewMenu, ReactionButton, ReactionMenu
+
+import re
+from enum import auto, Enum
+
+import discord
+from discord.ext.commands import Command
+
+from .abc import _BaseButton, PaginationEmojis
+from .errors import IncorrectType
+
+
+class _Details(NamedTuple):
+	"""Used for buttons with a `custom_id` of `ID_CALLER`"""
+	func: Callable[..., None]
+	args: Iterable[Any]
+	kwargs: Dict[str, Any]
+
+Details = _Details
+
+class ViewButton(discord.ui.Button, _BaseButton):
+	"""A helper class for :class:`ViewMenu`. Represents a UI button.
+	
+	Parameters
+	----------
+	style: :class:`discord.ButtonStyle`
+		The style of the button
+	
+	label: Optional[:class:`str`]
+		The button label, if any
+	
+	disabled: :class:`bool`
+		Whether the button is disabled or not
+	
+	custom_id: Optional[:class:`str`]
+		The ID of the button that gets received during an interaction. If this button is for a URL, it does not have a custom ID
+	
+	url: Optional[:class:`str`]
+		The URL this button sends you to
+	
+	emoji: Optional[Union[:class:`str`, :class:`discord.PartialEmoji`]]
+		The emoji of the button, if available
+	
+	followup: Optional[:class:`ViewButton.Follow`]
+		Used with buttons with custom_id :attr:`ViewButton.ID_CALLER`, :attr:`ViewButton.ID_SEND_MESSAGE`, :attr:`ViewButton.ID_CUSTOM_EMBED`
+	
+	event: Optional[:class:`ViewButton.Event`]
+		Set the button to be disabled or removed when it has been pressed a certain amount of times
+	
+	Kwargs
+	------
+	name: :class:`str`
+		An optional name for the button. Can be set to retrieve it later via :meth:`ViewMenu.get_button()`
+	
+	skip: :class:`ViewButton.Skip`
+		Set the action and the amount of pages to skip when using a `custom_id` of `ViewButton.ID_SKIP`
+	
+	persist: :class:`bool`
+		Available only when using link buttons. This prevents link buttons from being disabled/removed when the menu times out or is stopped so they can remain clickable
+	
+		.. added v3.1.0
+			:param:`persist`
+	"""
+	ID_NEXT_PAGE: Final[str] = '0'
+	ID_PREVIOUS_PAGE: Final[str] = '1'
+	ID_GO_TO_FIRST_PAGE: Final[str] = '2'
+	ID_GO_TO_LAST_PAGE: Final[str] = '3'
+	ID_GO_TO_PAGE: Final[str] = '4'
+	ID_END_SESSION: Final[str] = '5'
+	ID_CALLER: Final[str] = '6'
+	ID_SEND_MESSAGE: Final[str] = '7'
+	ID_CUSTOM_EMBED: Final[str] = '8'
+	ID_SKIP: Final[str] = '9'
+
+	_RE_IDs = r'[0-9]|[0-9]_\d+'
+	_RE_UNIQUE_ID_SET = r'_\d+'
+
+	def __init__(
+		self,
+		*,
+		style: discord.ButtonStyle=discord.ButtonStyle.secondary,
+		label: Optional[str]=None,
+		disabled: bool=False,
+		custom_id: Optional[str]=None,
+		url: Optional[str]=None,
+		emoji: Optional[Union[str, discord.PartialEmoji]]=None,
+		followup: Optional[ViewButton.Followup]=None,
+		event: Optional[ViewButton.Event]=None,
+		**kwargs
+		):
+		super().__init__(style=style, label=label, disabled=disabled, custom_id=custom_id, url=url, emoji=emoji, row=None)
+		_BaseButton.__init__(self, name=kwargs.get('name'), event=event, skip=kwargs.get('skip')) # type: ignore
+		self.followup = followup
+		self.persist: bool = kwargs.get('persist', False)
+		
+		# abc
+		self._menu: Optional[ViewMenu] = None
+	
+	def __repr__(self):
+		total_clicks = '' if self.style == discord.ButtonStyle.link else f' total_clicks={self.total_clicks}'
+		is_link_button = True if self.style == discord.ButtonStyle.link else False
+		return f'<ViewButton label={self.label!r} custom_id={ViewButton._get_id_name_from_id(str(self.custom_id), is_link_button=is_link_button)} style={self.style} emoji={self.emoji!r} url={self.url} disabled={self.disabled}{total_clicks}>'
+
+	async def callback(self, interaction: discord.Interaction) -> None:
+		"""*INTERNAL USE ONLY* - The callback function from the button interaction. This should not be manually called"""
+		await self._menu._paginate(self, interaction) # type: ignore
+	
+	class Followup:
+		"""A class that represents the message sent using a :class:`ViewButton`. Contains parameters similar to method `discord.abc.Messageable.send`. Only to be used with :class:`ViewButton` kwarg "followup".
+		It is to be noted that this should not be used with :class:`ViewButton` with a "style" of `discord.ButtonStyle.link` because link buttons do not send interaction events.
+		
+		Parameters
+		----------
+		content: Optional[:class:`str`]
+			Message to send
+		
+		embed: Optional[:class:`discord.Embed`]
+			Embed to send. Can also bet set for buttons with a custom_id of :attr:`ViewButton.ID_CUSTOM_EMBED`
+		
+		file: Optional[:class:`discord.File`]
+			File to send. If the :class:`ViewButton` custom_id is :attr:`ViewButton.ID_SEND_MESSAGE`, the file will be ignored because of discord API limitations
+		
+		tts: :class:`bool`
+			If discord should read the message aloud. Not valid for `ephemeral` messages
+		
+		allowed_mentions: Optional[:class:`discord.AllowedMentions`]
+			Controls the mentions being processed in the menu message. Not valid for `ephemeral` messages
+		
+		delete_after: Optional[Union[:class:`int`, :class:`float`]]
+			Amount of time to wait before the message is deleted. Not valid for `ephemeral` messages
+		
+		ephemeral: :class:`bool`
+			If the message will be hidden from everyone except the person that pressed the button. This is only valid for a :class:`ViewButton` with custom_id :attr:`ViewButton.ID_SEND_MESSAGE`
+		
+		Kwargs
+		------
+		details: :meth:`ViewButton.Followup.set_caller_details()`
+			The information that will be used when a `ViewButton.ID_CALLER` button is pressed (defaults to :class:`None`)
+		"""
+		
+		__slots__ = ('content', 'embed', 'file', 'tts', 'allowed_mentions', 'delete_after', 'ephemeral', 'details')
+
+		def __repr__(self):
+			x = []
+			for val in self.__class__.__slots__:
+				temp = getattr(self, val)
+				if temp:
+					x.append(f'{val}={temp!r}')
+			
+			return f'<Followup {" ".join(x)}>'
+
+		def __init__(
+			self,
+			content: Optional[str]=None, 
+			*,
+			embed: Optional[discord.Embed]=None,
+			file: Optional[discord.File]=None,
+			tts: bool=False,
+			allowed_mentions: Optional[discord.AllowedMentions]=None,
+			delete_after: Optional[Union[int, float]]=None,
+			ephemeral: bool=False,
+			**kwargs
+			):
+			self.content = content
+			self.embed = embed
+			self.file = file
+			self.tts = tts
+			self.allowed_mentions = allowed_mentions
+			self.delete_after = delete_after
+			self.ephemeral = ephemeral
+			self.details: Optional[Details] = kwargs.get('details')
+		
+		def _to_dict(self) -> dict:
+			"""This is a :class:`ViewButton.Followup` method"""
+			new = {}
+			for i in self.__slots__:
+				new[i] = getattr(self, i)
+			return new
+		
+		@staticmethod
+		def set_caller_details(func: Callable[..., None], *args, **kwargs) -> Details:
+			"""|static method|
+			
+			Set the parameters for the function you set for a :class:`ViewButton` with the custom_id :attr:`ViewButton.ID_CALLER`
+			
+			Parameters
+			----------
+			func: Callable[..., :class:`None`]
+				The function object that will be called when the associated button is pressed
+			
+			*args: `Any`
+				An argument list that represents the parameters of that function
+			
+			**kwargs: `Any`
+				An argument list that represents the kwarg parameters of that function
+			
+			Returns
+			-------
+			:class:`Details`: The :class:`NamedTuple` containing the values needed to internally call the function you have set
+			
+			Raises
+			------
+			- `IncorrectType`: Parameter "func" was not a callable object
+			"""
+			if callable(func):
+				func = func.callback if isinstance(func, Command) else func
+				return Details(func=func, args=args, kwargs=kwargs)
+			else:
+				raise IncorrectType('Parameter "func" must be callable')
+
+	@classmethod
+	def _base_nav_buttons(cls) -> Tuple[str, str, str, str, str]:
+		return (cls.ID_PREVIOUS_PAGE, cls.ID_NEXT_PAGE, cls.ID_GO_TO_FIRST_PAGE, cls.ID_GO_TO_LAST_PAGE, cls.ID_GO_TO_PAGE)
+	
+	@classmethod
+	def _get_id_name_from_id(cls, id_: str, **kwargs) -> str:
+		# if its a CALLER, SEND_MESSAGE, or CUSTOM_EMBED id, convert to it's true representation, because when passed, it's form is "[ButtonID]_[unique ID]"
+		# see :meth:`_button_add_check` or :meth:`_maybe_custom_id` for details
+
+		is_link_button = kwargs.get('is_link_button', False)
+		if is_link_button:
+			return 'LINK_BUTTON'
+		
+		unique_id_set = re.compile(ViewButton._RE_UNIQUE_ID_SET)
+		if re.search(unique_id_set, id_):
+			id_ = re.sub(unique_id_set, '', id_)
+		
+		for key, val in cls.__dict__.items():
+			if id_ == val:
+				return f'ViewButton.{key}'
+		
+		assert False, "id name could not be found"
+	
+	@property
+	def menu(self) -> Optional[ViewMenu]:
+		"""
+		Returns
+		-------
+		Optional[:class:`ViewMenu`]: The menu instance this button is attached to. Could be :class:`None` if the button is not attached to a menu
+		"""
+		return self._menu
+	
+	@classmethod
+	def generate_skip(cls, label: str, action: Literal['+', '-'], amount: int) -> ViewButton:
+		"""|class method|
+		
+		A factory method that returns a :class:`ViewButton` with the following parameters set:
+		
+		- style: `discord.ButtonStyle.gray`
+		- label: `<label>`
+		- custom_id: :attr:`ViewButton.ID_SKIP`
+		- skip: `ViewButton.Skip(<action>, <amount>)`
+		"""
+		return cls(style=discord.ButtonStyle.gray, label=label, custom_id=cls.ID_SKIP, skip=cls.Skip(action, amount))
+	
+	@classmethod
+	def link(cls, label: str, url: str) -> ViewButton:
+		"""|class method|
+		
+		A factory method that returns a :class:`ViewButton` with the following parameters set:
+		
+		- style: `discord.ButtonStyle.link`
+		- label: `<label>`
+		- url: `<url>`
+		"""
+		return cls(style=discord.ButtonStyle.link, label=str(label), url=str(url))
+	
+	@classmethod
+	def back(cls) -> ViewButton:
+		"""|class method|
+		
+		A factory method that returns a :class:`ViewButton` with the following parameters set:
+		
+		- style: `discord.ButtonStyle.gray`
+		- label: "Back"
+		- custom_id: :attr:`ViewButton.ID_PREVIOUS_PAGE`
+		"""
+		return cls(style=discord.ButtonStyle.gray, label='Back', custom_id=cls.ID_PREVIOUS_PAGE)
+	
+	@classmethod
+	def next(cls) -> ViewButton:
+		"""|class method|
+		
+		A factory method that returns a :class:`ViewButton` with the following parameters set:
+		
+		- style: `discord.ButtonStyle.gray`
+		- label: "Next"
+		- custom_id: :attr:`ViewButton.ID_NEXT_PAGE`
+		"""
+		return cls(style=discord.ButtonStyle.gray, label='Next', custom_id=cls.ID_NEXT_PAGE)
+	
+	@classmethod
+	def go_to_first_page(cls) -> ViewButton:
+		"""|class method|
+		
+		A factory method that returns a :class:`ViewButton` with the following parameters set:
+		
+		- style: `discord.ButtonStyle.gray`
+		- label: "First Page"
+		- custom_id: :attr:`ViewButton.ID_GO_TO_FIRST_PAGE`
+		"""
+		return cls(style=discord.ButtonStyle.gray, label='First Page', custom_id=cls.ID_GO_TO_FIRST_PAGE)
+	
+	@classmethod
+	def go_to_last_page(cls) -> ViewButton:
+		"""|class method|
+		
+		A factory method that returns a :class:`ViewButton` with the following parameters set:
+		
+		- style: `discord.ButtonStyle.gray`
+		- label: "Last Page"
+		- custom_id: :attr:`ViewButton.ID_GO_TO_LAST_PAGE`
+		"""
+		return cls(style=discord.ButtonStyle.gray, label='Last Page', custom_id=cls.ID_GO_TO_LAST_PAGE)
+	
+	@classmethod
+	def go_to_page(cls) -> ViewButton:
+		"""|class method|
+		
+		A factory method that returns a :class:`ViewButton` with the following parameters set:
+		
+		- style: `discord.ButtonStyle.gray`
+		- label: "Page Selection"
+		- custom_id: :attr:`ViewButton.ID_GO_TO_PAGE`
+		"""
+		return cls(style=discord.ButtonStyle.gray, label='Page Selection', custom_id=cls.ID_GO_TO_PAGE)
+	
+	@classmethod
+	def end_session(cls) -> ViewButton:
+		"""|class method|
+		
+		A factory method that returns a :class:`ViewButton` with the following parameters set:
+		
+		- style: `discord.ButtonStyle.gray`
+		- label: "Close"
+		- custom_id: :attr:`ViewButton.ID_END_SESSION`
+		"""
+		return cls(style=discord.ButtonStyle.gray, label='Close', custom_id=cls.ID_END_SESSION)
+	
+	@classmethod
+	def all(cls) -> List[ViewButton]:
+		"""|class method|
+		
+		A factory method that returns a list of all base navigation buttons. The following buttons are returned with pre-set values:
+		
+		- Button 1
+			- style: `discord.ButtonStyle.gray`
+			- label: "First Page"
+			- custom_id: :attr:`ViewButton.ID_GO_TO_FIRST_PAGE`
+		- Button 2
+			- style: `discord.ButtonStyle.gray`
+			- label: "Back"
+			- custom_id: :attr:`ViewButton.ID_PREVIOUS_PAGE`
+		- Button 3
+			- style: `discord.ButtonStyle.gray`
+			- label: "Next"
+			- custom_id: :attr:`ViewButton.ID_NEXT_PAGE`
+		- Button 4
+			- style: `discord.ButtonStyle.gray`
+			- label: "Last Page"
+			- custom_id: :attr:`ViewButton.ID_GO_TO_LAST_PAGE`
+		- Button 5
+			- style: `discord.ButtonStyle.gray`
+			- label: "Page Selection"
+			- custom_id: :attr:`ViewButton.ID_GO_TO_PAGE`
+		- Button 6
+			- style: `discord.ButtonStyle.gray`
+			- label: "Close"
+			- custom_id: :attr:`ViewButton.ID_END_SESSION`
+
+		They are returned in that order
+		
+		Returns
+		-------
+		List[:class:`ViewButton`]
+		"""
+		return [cls.go_to_first_page(), cls.back(), cls.next(), cls.go_to_last_page(), cls.go_to_page(), cls.end_session()]
+	
+	@classmethod
+	def all_with_emojis(cls) -> List[ViewButton]:
+		"""|class method|
+		
+		A factory method that returns a list of all base navigation buttons with emojis assigned instead of labels. The following buttons are returned with pre-set values:
+		
+		- Button 1
+			- style: `discord.ButtonStyle.gray`
+			- emoji: ⏪
+			- custom_id: :attr:`ViewButton.ID_GO_TO_FIRST_PAGE`
+		- Button 2
+			- style: `discord.ButtonStyle.gray`
+			- emoji: ◀️
+			- custom_id: :attr:`ViewButton.ID_PREVIOUS_PAGE`
+		- Button 3
+			- style: `discord.ButtonStyle.gray`
+			- emoji: ▶️
+			- custom_id: :attr:`ViewButton.ID_NEXT_PAGE`
+		- Button 4
+			- style: `discord.ButtonStyle.gray`
+			- emoji: ⏩
+			- custom_id: :attr:`ViewButton.ID_GO_TO_LAST_PAGE`
+		- Button 5
+			- style: `discord.ButtonStyle.gray`
+			- emoji: 🔢
+			- custom_id: :attr:`ViewButton.ID_GO_TO_PAGE`
+		- Button 6
+			- style: `discord.ButtonStyle.gray`
+			- emoji: ⏹️
+			- custom_id: :attr:`ViewButton.ID_END_SESSION`
+
+		They are returned in that order
+		
+		Returns
+		-------
+		List[:class:`ViewButton`]
+
+			.. added:: v3.1.0
+		"""
+		return [
+			cls(style=discord.ButtonStyle.gray, emoji='⏪', custom_id=cls.ID_GO_TO_FIRST_PAGE),
+			cls(style=discord.ButtonStyle.gray, emoji='◀️', custom_id=cls.ID_PREVIOUS_PAGE),
+			cls(style=discord.ButtonStyle.gray, emoji='▶️', custom_id=cls.ID_NEXT_PAGE),
+			cls(style=discord.ButtonStyle.gray, emoji='⏩', custom_id=cls.ID_GO_TO_LAST_PAGE),
+			cls(style=discord.ButtonStyle.gray, emoji='🔢', custom_id=cls.ID_GO_TO_PAGE),
+			cls(style=discord.ButtonStyle.gray, emoji='⏹️', custom_id=cls.ID_END_SESSION)
+		]
+
+class ButtonType(Enum):
+	"""A helper class for :class:`ReactionMenu`. Determines the generic action a button can perform."""
+	NEXT_PAGE = auto()
+	PREVIOUS_PAGE = auto()
+	GO_TO_FIRST_PAGE = auto()
+	GO_TO_LAST_PAGE = auto()
+	GO_TO_PAGE = auto()
+	END_SESSION = auto()
+	CUSTOM_EMBED = auto()
+	CALLER = auto()
+	SKIP = auto()
+
+	@staticmethod
+	def _get_buttontype_name_from_type(type_: ButtonType) -> str:
+		"""|static method| Used to determine the `linked_to` type. Returns the full :class:`str` representation of that type"""
+		return f'{type_.__class__.__name__}.{type_.name}'
+
+class ReactionButton(_BaseButton):
+	"""A helper class for :class:`ReactionMenu`. Represents a reaction.
+	
+	Parameters
+	----------
+	emoji: :class:`str`
+		The discord reaction that will be used
+
+	linked_to: :class:`ReactionButton.Type`
+		A generic action a button can perform
+	
+	Kwargs
+	------
+	embed: :class:`discord.Embed`
+		Only used when :param:`linked_to` is set as :attr:`ReactionButton.Type.CUSTOM_EMBED`. This is the embed that can be selected separately from the menu (`TypeEmbed` menu's only)
+
+	name: :class:`str`
+		An optional name for the button. Can be set to retrieve it later via :meth:`ReactionMenu.get_button()`
+
+	details: :meth:`ReactionButton.set_caller_details()`
+		The class method used to set the function and it's arguments to be called when the button is pressed
+	
+	event: :class:`ReactionButton.Event`
+		Determine when a button should be removed depending on how many times it has been pressed
+
+	skip: :class:`ReactionButton.Skip`
+		Set the action and the amount of pages to skip when using a `linked_to` of `ReactionButton.Type.SKIP`
+	"""
+
+	Type = ButtonType
+
+	def __init__(self, *, emoji: str, linked_to: ReactionButton.Type, **kwargs):
+		super().__init__(name=kwargs.get('name'), event=kwargs.get('event'), skip=kwargs.get('skip')) # type: ignore
+		self.emoji = str(emoji)
+		self.linked_to = linked_to
+		
+		self.custom_embed: Optional[discord.Embed] = kwargs.get('embed')
+		self.details: Optional[Details] = kwargs.get('details')
+		
+		# abc
+		self._menu: Optional[ReactionMenu] = None
+	
+	def __str__(self):
+		return self.emoji
+	
+	def __repr__(self):
+		return f'<ReactionButton emoji={self.emoji!r} linked_to={ButtonType._get_buttontype_name_from_type(self.linked_to)} total_clicks={self.total_clicks} name={self.name!r}>'
+	
+	@property
+	def menu(self) -> Optional[ReactionMenu]:
+		"""
+		Returns
+		-------
+		Optional[:class:`ReactionMenu`]: The menu the button is currently operating under. Can be :class:`None` if the button is not registered to a menu
+		"""
+		return self._menu
+	
+	@staticmethod
+	def set_caller_details(func: Callable[..., None], *args, **kwargs) -> Details:
+		"""|static method|
+		
+		Set the parameters for the function you set for a :class:`ReactionButton` with a `linked_to` of :attr:`ReactionButton.Type.CALLER`
+
+		Parameters
+		----------
+		func: Callable[..., :class:`None`]
+			The function object that will be called when the associated button is pressed
+		
+		*args: `Any`
+			An argument list that represents the parameters of that function
+		
+		**kwargs: `Any`
+			An argument list that represents the kwarg parameters of that function
+		
+		Returns
+		-------
+		:class:`Details`: The :class:`NamedTuple` containing the values needed to internally call the function you have set
+		
+		Raises
+		------
+		- `IncorrectType`: Parameter "func" was not a callable object
+		"""
+		if callable(func):
+			func = func.callback if isinstance(func, Command) else func
+			return Details(func=func, args=args, kwargs=kwargs)
+		else:
+			raise IncorrectType('Parameter "func" must be callable')
+	
+	@classmethod
+	def generate_skip(cls, emoji: str, action: Literal['+', '-'], amount: int) -> ReactionButton:
+		"""|class method|
+		
+		A factory method that returns a :class:`ReactionButton` with the following parameters set:
+		
+		- emoji: `<emoji>`
+		- linked_to: :attr:`ReactionButton.Type.SKIP`
+		- skip: `ReactionButton.Skip(<action>, <amount>)`
+		"""
+		return cls(emoji=emoji, linked_to=cls.Type.SKIP, skip=cls.Skip(action, amount))
+	
+	@classmethod
+	def back(cls) -> ReactionButton:
+		"""|class method|
+		
+		A factory method that returns a :class:`ReactionButton` with the following parameters set:
+		
+		- emoji: ◀️
+		- linked_to: :attr:`ReactionButton.Type.PREVIOUS_PAGE`
+		"""
+		return cls(emoji=PaginationEmojis.BACK_BUTTON, linked_to=cls.Type.PREVIOUS_PAGE)
+	
+	@classmethod
+	def next(cls) -> ReactionButton:
+		"""|class method|
+		
+		A factory method that returns a :class:`ReactionButton` with the following parameters set:
+		
+		- emoji: ▶️
+		- linked_to: :attr:`ReactionButton.Type.NEXT_PAGE`
+		"""
+		return cls(emoji=PaginationEmojis.NEXT_BUTTON, linked_to=cls.Type.NEXT_PAGE)
+	
+	@classmethod
+	def go_to_first_page(cls) -> ReactionButton:
+		"""|class method|
+		
+		A factory method that returns a :class:`ReactionButton` with the following parameters set:
+		
+		- emoji: ⏪
+		- linked_to: :attr:`ReactionButton.Type.GO_TO_FIRST_PAGE`
+		"""
+		return cls(emoji=PaginationEmojis.FIRST_PAGE, linked_to=cls.Type.GO_TO_FIRST_PAGE)
+	
+	@classmethod
+	def go_to_last_page(cls) -> ReactionButton:
+		"""|class method|
+		
+		A factory method that returns a :class:`ReactionButton` with the following parameters set:
+		
+		- emoji: ⏩
+		- linked_to: :attr:`ReactionButton.Type.GO_TO_LAST_PAGE`
+		"""
+		return cls(emoji=PaginationEmojis.LAST_PAGE, linked_to=cls.Type.GO_TO_LAST_PAGE)
+	
+	@classmethod
+	def go_to_page(cls) -> ReactionButton:
+		"""|class method|
+		
+		A factory method that returns a :class:`ReactionButton` with the following parameters set:
+		
+		- emoji: 🔢
+		- linked_to: :attr:`ReactionButton.Type.GO_TO_PAGE`
+		"""
+		return cls(emoji=PaginationEmojis.GO_TO_PAGE, linked_to=cls.Type.GO_TO_PAGE)
+	
+	@classmethod
+	def end_session(cls) -> ReactionButton:
+		"""|class method|
+		
+		A factory method that returns a :class:`ReactionButton` with the following parameters set:
+		
+		- emoji: ⏹️
+		- linked_to: :attr:`ReactionButton.Type.END_SESSION`
+		"""
+		return cls(emoji=PaginationEmojis.END_SESSION, linked_to=cls.Type.END_SESSION)
+	
+	@classmethod
+	def all(cls) -> List[ReactionButton]:
+		"""|class method|
+		
+		A factory method that returns a `list` of all base navigation buttons. Base navigation buttons are :class:`ReactionButton` with a `linked_to` of:
+		
+		- :attr:`ReactionButton.Type.GO_TO_FIRST_PAGE`
+		- :attr:`ReactionButton.Type.PREVIOUS_PAGE`
+		- :attr:`ReactionButton.Type.NEXT_PAGE`
+		- :attr:`ReactionButton.Type.GO_TO_LAST_PAGE`
+		- :attr:`ReactionButton.Type.GO_TO_PAGE`
+		- :attr:`ReactionButton.Type.END_SESSION`
+
+		They are returned in that order
+		"""
+		return [cls.go_to_first_page(), cls.back(), cls.next(), cls.go_to_last_page(), cls.go_to_page(), cls.end_session()]
```

### Comparing `reactionmenu-3.1.3/reactionmenu/core.py` & `reactionmenu-3.1.4/reactionmenu/core.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,712 +1,712 @@
-"""
-MIT License
-
-Copyright (c) 2021-present Defxult#8269
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
-DEALINGS IN THE SOFTWARE.
-"""
-
-from __future__ import annotations
-
-import asyncio
-import inspect
-from typing import TYPE_CHECKING, ClassVar, List, Literal, Optional, Sequence, Union, overload
-
-import discord
-from discord.ext.commands import Context
-
-if TYPE_CHECKING:
-	from .abc import MenuType
-	from discord.ext.commands import Bot
-
-from .abc import DEFAULT_BUTTONS, _BaseMenu, _PageController
-from .buttons import ReactionButton
-from .decorators import ensure_not_primed
-from .errors import *
-
-
-class ReactionMenu(_BaseMenu):
-	"""A class to create a discord pagination menu using reactions
-	
-	Parameters
-	----------
-	method: Union[:class:`discord.ext.commands.Context`, :class:`discord.Interaction`]
-		The Context object. You can get this using a command or if you're in a `discord.on_message` event. Also accepts interactions, typically received when using slash commands
-
-	menu_type: :class:`MenuType`
-		The configuration of the menu. Class variables :attr:`ReactionMenu.TypeEmbed`, :attr:`ReactionMenu.TypeEmbedDynamic`, or :attr:`ReactionMenu.TypeText`
-
-	Kwargs
-	------
-	all_can_click: :class:`bool`
-		Sets if everyone is allowed to control when pages are 'turned' when buttons are pressed (defaults to `False`)
-
-	allowed_mentions: :class:`discord.AllowedMentions`
-		Controls the mentions being processed in the menu message (defaults to :class:`discord.AllowedMentions(everyone=False, users=True, roles=False, replied_user=True)`)
-
-	clear_reactions_after: :class:`bool`
-		If the menu times out, remove all reactions (defaults to `True`)
-	
-	custom_embed: :class:`discord.Embed`
-		Embed object to use when adding data with :meth:`ReactionMenu.add_row()`. Used for styling purposes (:attr:`ReactionMenu.TypeEmbedDynamic` only/defaults to :class:`None`)
-
-	delete_interactions: :class:`bool`
-		Delete the prompt message by the bot and response message by the user when asked what page they would like to go to when using :attr:`ReactionButton.Type.GO_TO_PAGE` (defaults to `True`)
-
-	delete_on_timeout: :class:`bool`
-		When the menu times out, delete the menu message. This overrides :attr:`clear_reactions_after` (defaults to `False`)
-	
-	name: :class:`str`
-		A name you can set for the menu (defaults to :class:`None`)
-
-	navigation_speed: :class:`str`
-		Sets if the user needs to wait for the reaction to be removed by the bot before "turning" the page. Setting the speed to :attr:`ReactionMenu.FAST` makes it so that there is no need to wait (reactions are not removed on each press) and can
-		navigate lengthy menu's more quickly (defaults to :attr:`ReactionMenu.NORMAL`)
-
-	only_roles: List[:class:`discord.Role`]
-		Members with any of the provided roles are the only ones allowed to control the menu. The member who started the menu will always be able to control it. This overrides :attr:`all_can_click` (defaults to :class:`None`)
-	
-	remove_extra_reactions: :class:`bool`
-		If `True`, all emojis (reactions) added to the menu message that were not originally added to the menu will be removed (defaults to `False`)
-
-	rows_requested: :class:`int`
-		The amount of information per :meth:`ReactionMenu.add_row()` you would like applied to each embed page (:attr:`ReactionMenu.TypeEmbedDynamic` only/defaults to :class:`None`)
-
-	show_page_director: :class:`bool`
-		Shown at the bottom of each embed page. "Page 1/20" (defaults to `True`)
-
-	style: :class:`str`
-		A custom page director style you can select. "$" represents the current page, "&" represents the total amount of pages (defaults to "Page $/&") Example: `ReactionMenu(ctx, ..., style='On $ out of &')`
-
-	timeout: Union[:class:`float`, :class:`int`, :class:`None`]
-		Timer for when the menu should end. Can be :class:`None` for no timeout (defaults to 60.0)
-
-	wrap_in_codeblock: :class:`str`
-		The discord codeblock language identifier (:attr:`ReactionMenu.TypeEmbedDynamic` only/defaults to :class:`None`). Example: `ReactionMenu(ctx, ..., wrap_in_codeblock='py')`
-	"""
-
-	NORMAL: ClassVar[str] = 'NORMAL'
-	FAST: ClassVar[str] = 'FAST'
-
-	_active_sessions: List[ReactionMenu] = []
-
-	def __init__(self, method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs):
-		super().__init__(method, menu_type, **kwargs)
-
-		self.__buttons: List[ReactionButton] = []
-		
-		self.__main_session_task: Optional[asyncio.Task] = None
-		
-		# kwargs
-		self.timeout: Union[float, int, None] = kwargs.get('timeout', 60.0)
-		self.clear_reactions_after: bool = kwargs.get('clear_reactions_after', True)
-		self.remove_extra_reactions: bool = kwargs.get('remove_extra_reactions', False)
-		self.__navigation_speed: str = kwargs.get('navigation_speed', ReactionMenu.NORMAL)
-	
-	def __repr__(self):
-		return f'<ReactionMenu name={self.name!r} owner={str(self._extract_proper_user(self._method))!r} is_running={self._is_running} timeout={self.timeout} menu_type={self._menu_type.name}>'
-	
-	@property
-	def navigation_speed(self) -> str:
-		"""
-		Returns
-		-------
-		:class:`str`: The current :attr:`navigation_speed` that is set for the menu
-		"""
-		return self.__navigation_speed
-	
-	@property
-	def buttons(self) -> List[ReactionButton]:
-		"""
-		Returns
-		-------
-		List[:class:`ReactionButton`]: A list of all the buttons that have been added to the menu
-		"""
-		return self.__buttons
-	
-	@property
-	def buttons_most_clicked(self) -> List[ReactionButton]:
-		"""
-		Returns
-		-------
-		List[:class:`ReactionButton`]: The list of buttons on the menu ordered from highest (button with the most clicks) to lowest (button with the least clicks). Can be an empty list if there are no buttons registered to the menu
-		"""
-		return self._sort_buttons(self.__buttons)
-	
-	@classmethod
-	async def quick_start(cls, method: Union[Context, discord.Interaction], /, pages: Sequence[Union[discord.Embed, str]], buttons: Optional[Sequence[ReactionButton]]=DEFAULT_BUTTONS) -> ReactionMenu:
-		"""|coro class method|
-		
-		Start a menu with default settings either with a `menu_type` of `ReactionMenu.TypeEmbed` (all values in `pages` are of type `discord.Embed`) or `ReactionMenu.TypeText` (all values in `pages` are of type `str`)
-
-		Parameters
-		----------
-		method: Union[:class:`discord.ext.commands.Context`, :class:`discord.Interaction`]
-			The Context object. You can get this using a command or if you're in a `discord.on_message` event. Also accepts interactions, typically received when using slash commands
-
-		pages: Sequence[Union[:class:`discord.Embed`, :class:`str`]]
-			The pages to add
-
-		buttons: Optional[Sequence[:class:`ReactionButton`]]
-			The buttons to add. If left as `DEFAULT_BUTTONS`, that is equivalent to `ReactionButton.all()`
-		
-		Returns
-		-------
-		:class:`ReactionMenu`: The menu that was started
-		
-		Raises
-		------
-		- `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-		- `NoPages`: The menu was started when no pages have been added
-		- `NoButtons`: Attempted to start the menu when no Buttons have been registered
-		- `IncorrectType`: All items in :param:`pages` were not of type :class:`discord.Embed` or :class:`str`
-
-			.. added v3.1.0
-		"""
-		menu = cls(method, menu_type=cls._quick_check(pages))
-		menu.add_pages(pages) # type: ignore
-		menu.add_buttons(ReactionButton.all() if not buttons else buttons)
-		await menu.start()
-		return menu
-
-	def __extract_all_emojis(self) -> List[str]:
-		"""Return a list of all the emojis registered to each button. Can return an empty list if there are no buttons"""
-		return [button.emoji for button in self.__buttons]
-	
-	async def _handle_event(self, button: ReactionButton) -> None:
-		"""|coro| If an event is set, remove the buttons from the menu when the click requirement has been met"""
-		if button.event:
-			event_type = button.event.event_type
-			event_value = button.event.value
-			if button.total_clicks == event_value:
-				if event_type == ReactionButton.Event._REMOVE:
-					self._bypass_primed = True
-					self.remove_button(button)
-					await self._msg.clear_reaction(button.emoji)
-	
-	def _button_add_check(self, button: ReactionButton) -> None:
-		"""A set of checks to ensure the button can properly be added to the menu"""
-		if isinstance(button, ReactionButton):
-			if button.emoji not in self.__extract_all_emojis():
-				if button.linked_to == ReactionButton.Type.CUSTOM_EMBED and not button.custom_embed:
-					raise MissingSetting('When adding a button with the type "ReactionButton.Type.CUSTOM_EMBED", the kwarg "embed" is needed')
-				
-				if button.linked_to != ReactionButton.Type.CUSTOM_EMBED and button.custom_embed:
-					raise MenuSettingsMismatch('ReactionButton is not set as "ReactionButton.Type.CUSTOM_EMBED" but the "embed" of that button was set')
-
-				if button.linked_to == ReactionButton.Type.CALLER and not button.details:
-					raise MissingSetting('When adding a button with the type "ReactionButton.Type.CALLER", the kwarg "details" for that ReactionButton must be set.')
-				
-				# if the menu_type is TypeText, disallow custom embed buttons
-				if self._menu_type == ReactionMenu.TypeText and button.linked_to == ReactionButton.Type.CUSTOM_EMBED:
-					raise MenuSettingsMismatch('ReactionButton with a linked_to of ReactionButton.Type.CUSTOM_EMBED cannot be used when the menu_type is TypeText')
-				
-				# if using a skip button, ensure the skip attribute was set
-				if button.linked_to == ReactionButton.Type.SKIP and button.skip is None:
-					raise ReactionMenuException('When attempting to add a button with the type ReactionButton.Type.SKIP, the "skip" kwarg was not set')
-				
-				if len(self.__buttons) > 20:
-					raise TooManyButtons
-			else:
-				raise DuplicateButton(f'The emoji "{button.emoji}" has already been registered as a button')
-		else:
-			raise IncorrectType(f'Parameter "button" expected ReactionButton, got {button.__class__.__name__}')
-	
-	def _session_done_callback(self, task: asyncio.Task) -> None:
-		"""Handles the final cleanup after the menu session correctly/incorrectly ends"""
-		try:
-			task.result() # this is needed to raise ANY exception that occurred during the pagination process
-		except asyncio.CancelledError:
-			pass
-		finally:
-			self._is_running = False # already set in :meth:`.stop()`, but just in case this was reached without that method being called
-			if self in ReactionMenu._active_sessions:
-				ReactionMenu._active_sessions.remove(self)
-	
-	@overload
-	def get_button(self, identity: str, *, search_by: Literal['name', 'emoji', 'type']='name') -> List[ReactionButton]:
-		...
-	
-	@overload
-	def get_button(self, identity: int, *, search_by: Literal['name', 'emoji', 'type']='name') -> List[ReactionButton]:
-		...
-	
-	def get_button(self, identity: Union[str, int], *, search_by: Literal['name', 'emoji', 'type']='name') -> List[ReactionButton]:
-		"""Get a button that has been registered to the menu by name, emoji, or type
-
-		Parameters
-		----------
-		identity: :class:`str`
-			The button name, emoji, or type
-
-		search_by: :class:`str`
-			How to search for the button. If "name", it's searched by button names. If "emoji", it's searched by it's emojis. 
-			If "type", it's searched by :attr:`ReactionMenu.Type`, aka the `linked_to` of the button
-
-		Returns
-		-------
-		List[:class:`ReactionButton`]: The button(s) matching the given identity
-		
-		Raises
-		------
-		- `ReactionMenuException`: Parameter :param:`search_by` was not "name", "emoji", or "type"
-		"""
-		search_by = str(search_by).lower() # type: ignore
-		if search_by in ('name', 'emoji'):
-			identity = str(identity)
-
-		if search_by == 'name':
-			matched_names: List[ReactionButton] = [btn for btn in self.__buttons if btn.name == identity]
-			return matched_names
-
-		elif search_by == 'emoji':
-			for btn in self.__buttons:
-				if btn.emoji == identity:
-					return [btn]
-			return []
-		
-		elif search_by == 'type':
-			matched_types: List[ReactionButton] = [btn for btn in self.__buttons if btn.linked_to == identity]
-			return matched_types
-		
-		else:
-			raise ReactionMenuException(f'Parameter "search_by" expected "name", "emoji", or "type", got {search_by!r}')
-
-	@ensure_not_primed
-	def add_button(self, button: ReactionButton) -> None:
-		"""Add a button to the menu
-
-		Parameters
-		----------
-		button: :class:`ReactionButton`
-			The button to add
-
-		Raises
-		------
-		- `MenuAlreadyRunning`: Attempted to call this method after the menu has started
-		- `MissingSetting`: Set the buttons `linked_to` as :attr:`ReactionButton.Type.CALLER` but did not assign the :class:`ReactionButton` kwarg "details" a value
-		- `DuplicateButton`: The emoji used is already registered as a button
-		- `TooManyButtons`: More than 20 buttons were added. Discord has a reaction limit of 20
-		- `IncorrectType`: Parameter :param:`button` was not of type :class:`ReactionButton`
-		- `ReactionMenuException`: When attempting to add a button with the type `ReactionButton.Type.SKIP`, the "skip" kwarg was not set
-		- `MenuSettingsMismatch`: A :class:`ReactionButton` with a `linked_to` of :attr:`ReactionButton.Type.CUSTOM_EMBED` cannot be used when the `menu_type` is `TypeText`
-		"""
-		self._button_add_check(button)
-		button._menu = self
-		self.__buttons.append(button)
-	
-	@ensure_not_primed
-	def add_buttons(self, buttons: Sequence[ReactionButton]) -> None:
-		"""Add multiple buttons to the menu at once
-		
-		Parameters
-		----------
-		buttons: Sequence[:class:`ReactionButton`]
-			The buttons to add
-
-		Raises
-		------
-		- `MenuAlreadyRunning`: Attempted to call this method after the menu has started
-		- `MissingSetting`: Set the buttons `linked_to` as :attr:`ReactionButton.Type.CALLER` but did not assign the :class:`ReactionButton` kwarg "details" a value
-		- `DuplicateButton`: The emoji used is already registered as a button
-		- `TooManyButtons`: More than 20 buttons were added. Discord has a reaction limit of 20
-		- `IncorrectType`: Parameter :param:`button` was not of type :class:`ReactionButton`
-		- `ReactionMenuException`: When attempting to add a button with the type `ReactionButton.Type.SKIP`, the "skip" kwarg was not set
-		- `MenuSettingsMismatch`: A :class:`ReactionButton` with a `linked_to` of :attr:`ReactionButton.Type.CUSTOM_EMBED` cannot be used when the `menu_type` is `TypeText`
-		"""
-		for btn in buttons:
-			self.add_button(btn)
-	
-	@ensure_not_primed
-	def remove_button(self, button: ReactionButton) -> None:
-		"""Remove a button from the menu
-
-		Parameters
-		----------
-		button: :class:`ReactionButton`
-			The button to remove
-
-		Raises
-		------
-		- `MenuAlreadyRunning`: Attempted to call this method after the menu has started
-		- `ButtonNotFound`: The provided button was not found in the list of buttons on the menu
-		"""
-		if button in self.__buttons:
-			button._menu = None
-			self.__buttons.remove(button)
-		else:
-			raise ButtonNotFound('Cannot remove a button that is not registered')
-	
-	@ensure_not_primed
-	def remove_all_buttons(self) -> None:
-		"""Remove all buttons from the menu
-		
-		Raises
-		------
-		- `MenuAlreadyRunning`: Attempted to call this method after the menu has started
-		"""
-		for btn in self.__buttons:
-			btn._menu = None
-		self.__buttons.clear()
-	
-	def __wait_check(self, reaction: discord.Reaction, user: Union[discord.Member, discord.User]) -> bool:
-		"""Predicate for :meth:`discord.Client.wait_for()`. This also handles :attr:`all_can_click`"""
-		not_bot = False
-		correct_msg = False
-		correct_user = False
-
-		if not user.bot:
-			not_bot = True
-		
-		if reaction.message.id == self._msg.id:
-			correct_msg = True
-
-		if self.only_roles:
-			self.all_can_click = False
-			for role in self.only_roles:
-				if role in user.roles: # type: ignore / this will always have role objects (if the member has roles) because :attr:`only_roles` is overridden to `None` if the menu was sent in a DM
-					correct_user = True
-					break
-
-		if self.all_can_click:
-			correct_user = True
-		
-		menu_owner = self._extract_proper_user(self._method)
-		if user.id == menu_owner.id and not correct_user:
-			correct_user = True
-
-		return all([not_bot, correct_msg, correct_user])
-	
-	def __get_custom_embed_buttons(self) -> List[ReactionButton]:
-		"""Gets all custom embed buttons that have been set"""
-		return [btn for btn in self.__buttons if btn.linked_to == ReactionButton.Type.CUSTOM_EMBED]
-	
-	def __extract_proper_client(self) -> Union[Bot, discord.Client]:
-		"""Depending on the :attr:`_method`, this retrieves the proper client depending on if it's :class:`discord.Client` or :class:`commands.Bot`"""
-		if isinstance(self._method, Context): return self._method.bot
-		else: return self._method.client
-
-	async def __paginate(self, ready_event: asyncio.Event) -> None:
-		"""|coro| Handles the pagination process for all menu types"""
-		
-		async def determine_removal(emoji: str, user: Union[discord.Member, discord.User]) -> None:
-			"""|coro| Determines if the reaction should be removed or not depending on the menus :attr:`navigation_speed`"""
-			if self.__navigation_speed != ReactionMenu.FAST and self._method.guild is not None:
-				await self._msg.remove_reaction(emoji, user)
-		
-		async def update_and_dispatch(emoji: str, user: Union[discord.Member, discord.User], button: ReactionButton) -> None:
-			"""|coro| Handle reaction removal for :attr:`navigation_speed`. Update the buttons statistics. Contact the relay if one was set and handle any events if set"""
-			btn._update_statistics(user)
-			await determine_removal(emoji, user)
-			await self._handle_event(button)
-			await self._contact_relay(user, button)
-		
-		def proper_timeout() -> Optional[float]:
-			"""In :var:`wait_for_aws`, if the menu does not have a timeout (`Menu.timeout = None`), :class:`None` + :class:`float`, the float being "`self._timeout + 0.1`" from v1.0.5, will fail for obvious reasons. This checks if there is no timeout, 
-			and instead of adding those two together, simply return :class:`None` to avoid :exc:`TypeError`. This would happen if the menu's :attr:`Menu.navigation_speed` was set to :attr:`Menu.FAST` and
-			the :attr:`Menu.timeout` was set to :class:`None`
-			"""
-			if self.timeout is not None:
-				return self.timeout + 0.1
-			else:
-				return None
-
-		# apply the reactions (buttons) to the menu message
-		for btn in self.__buttons:
-			await self._msg.add_reaction(btn.emoji)
-		
-		ready_event.set()
-		self._is_running = True
-		ReactionMenu._active_sessions.append(self)
-		registered_emojis = self.__extract_all_emojis()
-		client = self.__extract_proper_client()
-		menu_owner = self._extract_proper_user(self._method)
-		
-		while self._is_running:
-			try:
-				if self.__navigation_speed == ReactionMenu.NORMAL:
-					reaction, user = await client.wait_for('reaction_add', check=self.__wait_check, timeout=self.timeout)
-				elif self.__navigation_speed == ReactionMenu.FAST:
-					wait_for_aws = (
-						client.wait_for('reaction_add', check=self.__wait_check, timeout=self.timeout),
-						client.wait_for('reaction_remove', check=self.__wait_check, timeout=proper_timeout()) 
-					)
-					done, pending = await asyncio.wait(wait_for_aws, return_when=asyncio.FIRST_COMPLETED)
-					
-					temp_pending: asyncio.Task = list(pending)[0]
-					temp_pending.cancel()
-
-					temp_done: asyncio.Task = list(done)[0]
-					reaction, user = temp_done.result()
-				else:
-					raise ReactionMenuException(f'Navigation speed {self.__navigation_speed!r} is not recognized')
-			except (asyncio.TimeoutError, asyncio.CancelledError):
-				self._menu_timed_out = True
-				await self.stop(delete_menu_message=self.delete_on_timeout, clear_reactions=self.clear_reactions_after)
-			else:
-				emoji = str(reaction.emoji)
-
-				if self.remove_extra_reactions and emoji not in registered_emojis:
-					if not self.in_dms:
-						await self._msg.clear_reaction(emoji)
-						continue
-
-				for btn in self.__buttons:
-					# previous
-					if emoji == btn.emoji and btn.linked_to == ReactionButton.Type.PREVIOUS_PAGE:
-						await self._msg.edit(**self._determine_kwargs(self._pc.prev()))
-						await update_and_dispatch(emoji, user, btn)
-					
-					# next
-					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.NEXT_PAGE:
-						await self._msg.edit(**self._determine_kwargs(self._pc.next()))
-						await update_and_dispatch(emoji, user, btn)
-					
-					# first page
-					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.GO_TO_FIRST_PAGE:
-						await self._msg.edit(**self._determine_kwargs(self._pc.first_page()))
-						await update_and_dispatch(emoji, user, btn)
-					
-					# last page
-					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.GO_TO_LAST_PAGE:
-						await self._msg.edit(**self._determine_kwargs(self._pc.last_page()))
-						await update_and_dispatch(emoji, user, btn)
-					
-					# skip
-					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.SKIP:
-						await self._msg.edit(**self._determine_kwargs(self._pc.skip(btn.skip)))
-						await update_and_dispatch(emoji, user, btn)
-					
-					# go to page
-					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.GO_TO_PAGE:
-						prompt: discord.Message = await self._msg.channel.send(f'{menu_owner.display_name}, what page would you like to go to?')
-						try:
-							selection_message: discord.Message = await client.wait_for('message', check=lambda m: all([m.channel.id == self._msg.channel.id, m.author.id == menu_owner.id]), timeout=self.timeout)
-							page = int(selection_message.content)
-						except (asyncio.TimeoutError, ValueError):
-							# dont call :meth:`.stop()` here because I want the timeout factor to only be applicable after the
-							# original reactions were added
-							continue
-						else:
-							if 1 <= page <= len(self._pages):
-								self._pc.index = page - 1
-								await self._msg.edit(**self._determine_kwargs(self._pc.current_page))
-								if self.delete_interactions:
-									await prompt.delete()
-									await selection_message.delete()
-								
-								await update_and_dispatch(emoji, user, btn)
-					
-					# end session
-					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.END_SESSION:
-						await update_and_dispatch(emoji, user, btn)
-						await self.stop(delete_menu_message=True)
-					
-					# caller buttons
-					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.CALLER:
-						func = btn.details.func # type: ignore / details member "func" is mandatory
-						args = btn.details.args # type: ignore / details member "args" could be an iterable
-						kwargs = btn.details.kwargs # type: ignore / details member "kwargs" could be an dict
-						
-						try:
-							if inspect.iscoroutinefunction(func):
-								await func(*args, **kwargs) # type: ignore / `func` is already confirmed to be a coroutine
-							else:
-								func(*args, **kwargs)
-						except Exception as err:
-							raise ReactionMenuException(inspect.cleandoc(
-								f"""
-								A ReactionButton with a linked_to of ReactionButton.Type.CALLER raised an error during it's execution
-								-> {err.__class__.__name__}: {err}
-								"""
-							))
-						else:
-							await update_and_dispatch(emoji, user, btn)
-						
-					# custom buttons
-					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.CUSTOM_EMBED:
-						await update_and_dispatch(emoji, user, btn)
-						await self._msg.edit(embed=btn.custom_embed)
-
-	async def stop(self, *, delete_menu_message: bool=False, clear_reactions: bool=False) -> None:
-		"""|coro|
-		
-		Stops the process of the menu with the option of deleting the menu's message or clearing reactions upon stop
-		
-		Parameters
-		----------
-		delete_menu_message: :class:`bool`
-			Delete the menu message
-		
-		clear_reactions: :class:`bool`
-			Remove all reactions
-		
-		Raises
-		------
-		- `discord.DiscordException`: Any exception that can be raised when deleting a message or removing a reaction from a message
-		"""
-		if self._is_running:
-			try:
-				if delete_menu_message:
-					await self._msg.delete()
-				elif clear_reactions:
-					await self._msg.clear_reactions()
-				await self._handle_on_timeout()
-			except discord.DiscordException as discord_error:
-				raise discord_error
-			finally:
-				self._is_running = False
-				self._on_close_event.set()
-				self.__main_session_task.cancel() # type: ignore / task object would have been set by the time this is executed
-	
-	def _override_dm_settings(self) -> None:
-		"""If a menu session is in a direct message the following settings are disabled/changed because of discord limitations and resource/safety reasons"""
-		if self.in_dms:
-			# Not allowed to remove reactions in DMs
-			if self.clear_reactions_after:
-				self.clear_reactions_after = False
-			
-			# Has to be set to `FAST` because bots are not allowed to remove reactions in DMs
-			if self.__navigation_speed == ReactionMenu.NORMAL:
-				self.__navigation_speed = ReactionMenu.FAST
-			
-			# Can't delete someone else's message in DMs
-			if self.delete_interactions:
-				self.delete_interactions = False
-			
-			# There are no roles in DMs
-			if self.only_roles:
-				self.only_roles = None
-			
-			# No point in having an *indefinite* menu in DMs
-			if self.timeout is None:
-				self.timeout = 60.0
-		
-	def __generate_reactionmenu_payload(self) -> dict:
-		"""Creates the parameters needed for :meth:`discord.Messageable.send()`
-
-			.. added:: v3.1.0
-		"""
-		return {
-			"content" : self._pages[0].content if self._pages else None,
-			"embed" : self._pages[0].embed if self._pages else discord.utils.MISSING,
-			"files" : self._pages[0].files if self._pages else discord.utils.MISSING,
-			"allowed_mentions" : self.allowed_mentions
-		}
-	
-	@overload
-	async def start(self, *, send_to: Optional[str]=None, reply: bool=False) -> None:
-		...
-	
-	@overload
-	async def start(self, *, send_to: Optional[int]=None, reply: bool=False) -> None:
-		...
-	
-	@overload
-	async def start(self, *, send_to: Optional[discord.TextChannel]=None, reply: bool=False) -> None:
-		...
-	
-	@overload
-	async def start(self, *, send_to: Optional[discord.VoiceChannel]=None, reply: bool=False) -> None:
-		...
-	
-	@overload
-	async def start(self, *, send_to: Optional[discord.Thread]=None, reply: bool=False) -> None:
-		...
-	
-	@ensure_not_primed
-	async def start(self, *, send_to: Optional[Union[str, int, discord.TextChannel, discord.VoiceChannel, discord.Thread]]=None, reply: bool=False) -> None:
-		"""|coro|
-		
-		Start the menu
-
-		Parameters
-		----------
-		send_to: Optional[Union[:class:`str`, :class:`int`, :class:`discord.TextChannel`, :class:`discord.VoiceChannel`, :class:`discord.Thread`]]
-			The channel/thread you'd like the menu to start in. Use the channel/threads name, ID, or it's object. Please note that if you intend to use a channel/thread object, using
-			method :meth:`discord.Client.get_channel()` (or any other related methods), that channel should be in the same list as if you were to use `ctx.guild.text_channels`
-			or `ctx.guild.threads`. This only works on a context guild channel basis. That means a menu instance cannot be created in one guild and the menu itself (:param:`send_to`)
-			be sent to another. Whichever guild context the menu was instantiated in, the channels/threads of that guild are the only options for :param:`send_to`
-
-		reply: :class:`bool`
-			Enables the menu message to reply to the message that triggered it. Parameter :param:`send_to` must be :class:`None` if this is `True`. This only pertains to a non-interaction based menu.
-
-		Raises
-		------
-		- `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-		- `NoPages`: The menu was started when no pages have been added
-		- `NoButtons`: Attempted to start the menu when no Buttons have been registered
-		- `ReactionMenuException`: The :class:`ReactionMenu`'s `menu_type` was not recognized
-		- `DescriptionOversized`: When using a `menu_type` of :attr:`ReactionMenu.TypeEmbedDynamic`, the embed description was over discords size limit
-		- `IncorrectType`: Parameter :param:`send_to` was not of the expected type
-		- `MenuException`: The channel set in :param:`send_to` was not found
-		"""
-		if ReactionMenu._sessions_limit_details.set_by_user:
-			can_proceed = await self._handle_session_limits()
-			if not can_proceed:
-				return
-		
-		self._override_dm_settings()
-		
-		if self._menu_type not in ReactionMenu._all_menu_types():
-			raise ReactionMenuException('ReactionMenu menu_type not recognized')
-		if not self.__buttons:
-			raise NoButtons
-
-		reply_kwargs = self._handle_reply_kwargs(send_to, reply)
-		menu_payload = self.__generate_reactionmenu_payload()
-
-		if isinstance(self._method, Context):
-			menu_payload.update(reply_kwargs)
-		
-		if self._menu_type == ReactionMenu.TypeEmbed:
-			if self._pages:
-				self._refresh_page_director_info(self._menu_type, self._pages)
-			
-			custom_embed_buttons = self.__get_custom_embed_buttons()
-			# no pages and no custom embeds (no pages at all)
-			if not self._pages and not custom_embed_buttons:
-				raise NoPages	
-
-			# only custom embeds
-			if not self._pages and custom_embed_buttons:
-				menu_payload['embed'] = custom_embed_buttons[0].custom_embed
-				await self._handle_send_to(send_to, menu_payload)
-			
-			# normal pages, no custom embeds
-			else:
-				await self._handle_send_to(send_to, menu_payload)
-		
-		elif self._menu_type == ReactionMenu.TypeText:
-			if not self._pages:
-				raise NoPages
-			
-			self._refresh_page_director_info(self._menu_type, self._pages)
-			menu_payload['content'] = self._pages[0].content
-			await self._handle_send_to(send_to, menu_payload)
-		
-		elif self._menu_type == ReactionMenu.TypeEmbedDynamic:
-			# page director info is refreshed in method
-			await self._build_dynamic_pages(send_to, payload=menu_payload)
-
-		ready_event = asyncio.Event()
-		self._pc = _PageController(self._pages)
-		self.__main_session_task = self.__extract_proper_client().loop.create_task(self.__paginate(ready_event))
-		self.__main_session_task.add_done_callback(self._session_done_callback)
-		await ready_event.wait()
+"""
+MIT License
+
+Copyright (c) 2021-present Defxult#8269
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+import asyncio
+import inspect
+from typing import TYPE_CHECKING, ClassVar, List, Literal, Optional, Sequence, Union, overload
+
+import discord
+from discord.ext.commands import Context
+
+if TYPE_CHECKING:
+	from .abc import MenuType
+	from discord.ext.commands import Bot
+
+from .abc import DEFAULT_BUTTONS, _BaseMenu, _PageController
+from .buttons import ReactionButton
+from .decorators import ensure_not_primed
+from .errors import *
+
+
+class ReactionMenu(_BaseMenu):
+	"""A class to create a discord pagination menu using reactions
+	
+	Parameters
+	----------
+	method: Union[:class:`discord.ext.commands.Context`, :class:`discord.Interaction`]
+		The Context object. You can get this using a command or if you're in a `discord.on_message` event. Also accepts interactions, typically received when using slash commands
+
+	menu_type: :class:`MenuType`
+		The configuration of the menu. Class variables :attr:`ReactionMenu.TypeEmbed`, :attr:`ReactionMenu.TypeEmbedDynamic`, or :attr:`ReactionMenu.TypeText`
+
+	Kwargs
+	------
+	all_can_click: :class:`bool`
+		Sets if everyone is allowed to control when pages are 'turned' when buttons are pressed (defaults to `False`)
+
+	allowed_mentions: :class:`discord.AllowedMentions`
+		Controls the mentions being processed in the menu message (defaults to :class:`discord.AllowedMentions(everyone=False, users=True, roles=False, replied_user=True)`)
+
+	clear_reactions_after: :class:`bool`
+		If the menu times out, remove all reactions (defaults to `True`)
+	
+	custom_embed: :class:`discord.Embed`
+		Embed object to use when adding data with :meth:`ReactionMenu.add_row()`. Used for styling purposes (:attr:`ReactionMenu.TypeEmbedDynamic` only/defaults to :class:`None`)
+
+	delete_interactions: :class:`bool`
+		Delete the prompt message by the bot and response message by the user when asked what page they would like to go to when using :attr:`ReactionButton.Type.GO_TO_PAGE` (defaults to `True`)
+
+	delete_on_timeout: :class:`bool`
+		When the menu times out, delete the menu message. This overrides :attr:`clear_reactions_after` (defaults to `False`)
+	
+	name: :class:`str`
+		A name you can set for the menu (defaults to :class:`None`)
+
+	navigation_speed: :class:`str`
+		Sets if the user needs to wait for the reaction to be removed by the bot before "turning" the page. Setting the speed to :attr:`ReactionMenu.FAST` makes it so that there is no need to wait (reactions are not removed on each press) and can
+		navigate lengthy menu's more quickly (defaults to :attr:`ReactionMenu.NORMAL`)
+
+	only_roles: List[:class:`discord.Role`]
+		Members with any of the provided roles are the only ones allowed to control the menu. The member who started the menu will always be able to control it. This overrides :attr:`all_can_click` (defaults to :class:`None`)
+	
+	remove_extra_reactions: :class:`bool`
+		If `True`, all emojis (reactions) added to the menu message that were not originally added to the menu will be removed (defaults to `False`)
+
+	rows_requested: :class:`int`
+		The amount of information per :meth:`ReactionMenu.add_row()` you would like applied to each embed page (:attr:`ReactionMenu.TypeEmbedDynamic` only/defaults to :class:`None`)
+
+	show_page_director: :class:`bool`
+		Shown at the bottom of each embed page. "Page 1/20" (defaults to `True`)
+
+	style: :class:`str`
+		A custom page director style you can select. "$" represents the current page, "&" represents the total amount of pages (defaults to "Page $/&") Example: `ReactionMenu(ctx, ..., style='On $ out of &')`
+
+	timeout: Union[:class:`float`, :class:`int`, :class:`None`]
+		Timer for when the menu should end. Can be :class:`None` for no timeout (defaults to 60.0)
+
+	wrap_in_codeblock: :class:`str`
+		The discord codeblock language identifier (:attr:`ReactionMenu.TypeEmbedDynamic` only/defaults to :class:`None`). Example: `ReactionMenu(ctx, ..., wrap_in_codeblock='py')`
+	"""
+
+	NORMAL: ClassVar[str] = 'NORMAL'
+	FAST: ClassVar[str] = 'FAST'
+
+	_active_sessions: List[ReactionMenu] = []
+
+	def __init__(self, method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs):
+		super().__init__(method, menu_type, **kwargs)
+
+		self.__buttons: List[ReactionButton] = []
+		
+		self.__main_session_task: Optional[asyncio.Task] = None
+		
+		# kwargs
+		self.timeout: Union[float, int, None] = kwargs.get('timeout', 60.0)
+		self.clear_reactions_after: bool = kwargs.get('clear_reactions_after', True)
+		self.remove_extra_reactions: bool = kwargs.get('remove_extra_reactions', False)
+		self.__navigation_speed: str = kwargs.get('navigation_speed', ReactionMenu.NORMAL)
+	
+	def __repr__(self):
+		return f'<ReactionMenu name={self.name!r} owner={str(self._extract_proper_user(self._method))!r} is_running={self._is_running} timeout={self.timeout} menu_type={self._menu_type.name}>'
+	
+	@property
+	def navigation_speed(self) -> str:
+		"""
+		Returns
+		-------
+		:class:`str`: The current :attr:`navigation_speed` that is set for the menu
+		"""
+		return self.__navigation_speed
+	
+	@property
+	def buttons(self) -> List[ReactionButton]:
+		"""
+		Returns
+		-------
+		List[:class:`ReactionButton`]: A list of all the buttons that have been added to the menu
+		"""
+		return self.__buttons
+	
+	@property
+	def buttons_most_clicked(self) -> List[ReactionButton]:
+		"""
+		Returns
+		-------
+		List[:class:`ReactionButton`]: The list of buttons on the menu ordered from highest (button with the most clicks) to lowest (button with the least clicks). Can be an empty list if there are no buttons registered to the menu
+		"""
+		return self._sort_buttons(self.__buttons)
+	
+	@classmethod
+	async def quick_start(cls, method: Union[Context, discord.Interaction], /, pages: Sequence[Union[discord.Embed, str]], buttons: Optional[Sequence[ReactionButton]]=DEFAULT_BUTTONS) -> ReactionMenu:
+		"""|coro class method|
+		
+		Start a menu with default settings either with a `menu_type` of `ReactionMenu.TypeEmbed` (all values in `pages` are of type `discord.Embed`) or `ReactionMenu.TypeText` (all values in `pages` are of type `str`)
+
+		Parameters
+		----------
+		method: Union[:class:`discord.ext.commands.Context`, :class:`discord.Interaction`]
+			The Context object. You can get this using a command or if you're in a `discord.on_message` event. Also accepts interactions, typically received when using slash commands
+
+		pages: Sequence[Union[:class:`discord.Embed`, :class:`str`]]
+			The pages to add
+
+		buttons: Optional[Sequence[:class:`ReactionButton`]]
+			The buttons to add. If left as `DEFAULT_BUTTONS`, that is equivalent to `ReactionButton.all()`
+		
+		Returns
+		-------
+		:class:`ReactionMenu`: The menu that was started
+		
+		Raises
+		------
+		- `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+		- `NoPages`: The menu was started when no pages have been added
+		- `NoButtons`: Attempted to start the menu when no Buttons have been registered
+		- `IncorrectType`: All items in :param:`pages` were not of type :class:`discord.Embed` or :class:`str`
+
+			.. added v3.1.0
+		"""
+		menu = cls(method, menu_type=cls._quick_check(pages))
+		menu.add_pages(pages) # type: ignore
+		menu.add_buttons(ReactionButton.all() if not buttons else buttons)
+		await menu.start()
+		return menu
+
+	def __extract_all_emojis(self) -> List[str]:
+		"""Return a list of all the emojis registered to each button. Can return an empty list if there are no buttons"""
+		return [button.emoji for button in self.__buttons]
+	
+	async def _handle_event(self, button: ReactionButton) -> None:
+		"""|coro| If an event is set, remove the buttons from the menu when the click requirement has been met"""
+		if button.event:
+			event_type = button.event.event_type
+			event_value = button.event.value
+			if button.total_clicks == event_value:
+				if event_type == ReactionButton.Event._REMOVE:
+					self._bypass_primed = True
+					self.remove_button(button)
+					await self._msg.clear_reaction(button.emoji)
+	
+	def _button_add_check(self, button: ReactionButton) -> None:
+		"""A set of checks to ensure the button can properly be added to the menu"""
+		if isinstance(button, ReactionButton):
+			if button.emoji not in self.__extract_all_emojis():
+				if button.linked_to == ReactionButton.Type.CUSTOM_EMBED and not button.custom_embed:
+					raise MissingSetting('When adding a button with the type "ReactionButton.Type.CUSTOM_EMBED", the kwarg "embed" is needed')
+				
+				if button.linked_to != ReactionButton.Type.CUSTOM_EMBED and button.custom_embed:
+					raise MenuSettingsMismatch('ReactionButton is not set as "ReactionButton.Type.CUSTOM_EMBED" but the "embed" of that button was set')
+
+				if button.linked_to == ReactionButton.Type.CALLER and not button.details:
+					raise MissingSetting('When adding a button with the type "ReactionButton.Type.CALLER", the kwarg "details" for that ReactionButton must be set.')
+				
+				# if the menu_type is TypeText, disallow custom embed buttons
+				if self._menu_type == ReactionMenu.TypeText and button.linked_to == ReactionButton.Type.CUSTOM_EMBED:
+					raise MenuSettingsMismatch('ReactionButton with a linked_to of ReactionButton.Type.CUSTOM_EMBED cannot be used when the menu_type is TypeText')
+				
+				# if using a skip button, ensure the skip attribute was set
+				if button.linked_to == ReactionButton.Type.SKIP and button.skip is None:
+					raise ReactionMenuException('When attempting to add a button with the type ReactionButton.Type.SKIP, the "skip" kwarg was not set')
+				
+				if len(self.__buttons) > 20:
+					raise TooManyButtons
+			else:
+				raise DuplicateButton(f'The emoji "{button.emoji}" has already been registered as a button')
+		else:
+			raise IncorrectType(f'Parameter "button" expected ReactionButton, got {button.__class__.__name__}')
+	
+	def _session_done_callback(self, task: asyncio.Task) -> None:
+		"""Handles the final cleanup after the menu session correctly/incorrectly ends"""
+		try:
+			task.result() # this is needed to raise ANY exception that occurred during the pagination process
+		except asyncio.CancelledError:
+			pass
+		finally:
+			self._is_running = False # already set in :meth:`.stop()`, but just in case this was reached without that method being called
+			if self in ReactionMenu._active_sessions:
+				ReactionMenu._active_sessions.remove(self)
+	
+	@overload
+	def get_button(self, identity: str, *, search_by: Literal['name', 'emoji', 'type']='name') -> List[ReactionButton]:
+		...
+	
+	@overload
+	def get_button(self, identity: int, *, search_by: Literal['name', 'emoji', 'type']='name') -> List[ReactionButton]:
+		...
+	
+	def get_button(self, identity: Union[str, int], *, search_by: Literal['name', 'emoji', 'type']='name') -> List[ReactionButton]:
+		"""Get a button that has been registered to the menu by name, emoji, or type
+
+		Parameters
+		----------
+		identity: :class:`str`
+			The button name, emoji, or type
+
+		search_by: :class:`str`
+			How to search for the button. If "name", it's searched by button names. If "emoji", it's searched by it's emojis. 
+			If "type", it's searched by :attr:`ReactionMenu.Type`, aka the `linked_to` of the button
+
+		Returns
+		-------
+		List[:class:`ReactionButton`]: The button(s) matching the given identity
+		
+		Raises
+		------
+		- `ReactionMenuException`: Parameter :param:`search_by` was not "name", "emoji", or "type"
+		"""
+		search_by = str(search_by).lower() # type: ignore
+		if search_by in ('name', 'emoji'):
+			identity = str(identity)
+
+		if search_by == 'name':
+			matched_names: List[ReactionButton] = [btn for btn in self.__buttons if btn.name == identity]
+			return matched_names
+
+		elif search_by == 'emoji':
+			for btn in self.__buttons:
+				if btn.emoji == identity:
+					return [btn]
+			return []
+		
+		elif search_by == 'type':
+			matched_types: List[ReactionButton] = [btn for btn in self.__buttons if btn.linked_to == identity]
+			return matched_types
+		
+		else:
+			raise ReactionMenuException(f'Parameter "search_by" expected "name", "emoji", or "type", got {search_by!r}')
+
+	@ensure_not_primed
+	def add_button(self, button: ReactionButton) -> None:
+		"""Add a button to the menu
+
+		Parameters
+		----------
+		button: :class:`ReactionButton`
+			The button to add
+
+		Raises
+		------
+		- `MenuAlreadyRunning`: Attempted to call this method after the menu has started
+		- `MissingSetting`: Set the buttons `linked_to` as :attr:`ReactionButton.Type.CALLER` but did not assign the :class:`ReactionButton` kwarg "details" a value
+		- `DuplicateButton`: The emoji used is already registered as a button
+		- `TooManyButtons`: More than 20 buttons were added. Discord has a reaction limit of 20
+		- `IncorrectType`: Parameter :param:`button` was not of type :class:`ReactionButton`
+		- `ReactionMenuException`: When attempting to add a button with the type `ReactionButton.Type.SKIP`, the "skip" kwarg was not set
+		- `MenuSettingsMismatch`: A :class:`ReactionButton` with a `linked_to` of :attr:`ReactionButton.Type.CUSTOM_EMBED` cannot be used when the `menu_type` is `TypeText`
+		"""
+		self._button_add_check(button)
+		button._menu = self
+		self.__buttons.append(button)
+	
+	@ensure_not_primed
+	def add_buttons(self, buttons: Sequence[ReactionButton]) -> None:
+		"""Add multiple buttons to the menu at once
+		
+		Parameters
+		----------
+		buttons: Sequence[:class:`ReactionButton`]
+			The buttons to add
+
+		Raises
+		------
+		- `MenuAlreadyRunning`: Attempted to call this method after the menu has started
+		- `MissingSetting`: Set the buttons `linked_to` as :attr:`ReactionButton.Type.CALLER` but did not assign the :class:`ReactionButton` kwarg "details" a value
+		- `DuplicateButton`: The emoji used is already registered as a button
+		- `TooManyButtons`: More than 20 buttons were added. Discord has a reaction limit of 20
+		- `IncorrectType`: Parameter :param:`button` was not of type :class:`ReactionButton`
+		- `ReactionMenuException`: When attempting to add a button with the type `ReactionButton.Type.SKIP`, the "skip" kwarg was not set
+		- `MenuSettingsMismatch`: A :class:`ReactionButton` with a `linked_to` of :attr:`ReactionButton.Type.CUSTOM_EMBED` cannot be used when the `menu_type` is `TypeText`
+		"""
+		for btn in buttons:
+			self.add_button(btn)
+	
+	@ensure_not_primed
+	def remove_button(self, button: ReactionButton) -> None:
+		"""Remove a button from the menu
+
+		Parameters
+		----------
+		button: :class:`ReactionButton`
+			The button to remove
+
+		Raises
+		------
+		- `MenuAlreadyRunning`: Attempted to call this method after the menu has started
+		- `ButtonNotFound`: The provided button was not found in the list of buttons on the menu
+		"""
+		if button in self.__buttons:
+			button._menu = None
+			self.__buttons.remove(button)
+		else:
+			raise ButtonNotFound('Cannot remove a button that is not registered')
+	
+	@ensure_not_primed
+	def remove_all_buttons(self) -> None:
+		"""Remove all buttons from the menu
+		
+		Raises
+		------
+		- `MenuAlreadyRunning`: Attempted to call this method after the menu has started
+		"""
+		for btn in self.__buttons:
+			btn._menu = None
+		self.__buttons.clear()
+	
+	def __wait_check(self, reaction: discord.Reaction, user: Union[discord.Member, discord.User]) -> bool:
+		"""Predicate for :meth:`discord.Client.wait_for()`. This also handles :attr:`all_can_click`"""
+		not_bot = False
+		correct_msg = False
+		correct_user = False
+
+		if not user.bot:
+			not_bot = True
+		
+		if reaction.message.id == self._msg.id:
+			correct_msg = True
+
+		if self.only_roles:
+			self.all_can_click = False
+			for role in self.only_roles:
+				if role in user.roles: # type: ignore / this will always have role objects (if the member has roles) because :attr:`only_roles` is overridden to `None` if the menu was sent in a DM
+					correct_user = True
+					break
+
+		if self.all_can_click:
+			correct_user = True
+		
+		menu_owner = self._extract_proper_user(self._method)
+		if user.id == menu_owner.id and not correct_user:
+			correct_user = True
+
+		return all([not_bot, correct_msg, correct_user])
+	
+	def __get_custom_embed_buttons(self) -> List[ReactionButton]:
+		"""Gets all custom embed buttons that have been set"""
+		return [btn for btn in self.__buttons if btn.linked_to == ReactionButton.Type.CUSTOM_EMBED]
+	
+	def __extract_proper_client(self) -> Union[Bot, discord.Client]:
+		"""Depending on the :attr:`_method`, this retrieves the proper client depending on if it's :class:`discord.Client` or :class:`commands.Bot`"""
+		if isinstance(self._method, Context): return self._method.bot
+		else: return self._method.client
+
+	async def __paginate(self, ready_event: asyncio.Event) -> None:
+		"""|coro| Handles the pagination process for all menu types"""
+		
+		async def determine_removal(emoji: str, user: Union[discord.Member, discord.User]) -> None:
+			"""|coro| Determines if the reaction should be removed or not depending on the menus :attr:`navigation_speed`"""
+			if self.__navigation_speed != ReactionMenu.FAST and self._method.guild is not None:
+				await self._msg.remove_reaction(emoji, user)
+		
+		async def update_and_dispatch(emoji: str, user: Union[discord.Member, discord.User], button: ReactionButton) -> None:
+			"""|coro| Handle reaction removal for :attr:`navigation_speed`. Update the buttons statistics. Contact the relay if one was set and handle any events if set"""
+			btn._update_statistics(user)
+			await determine_removal(emoji, user)
+			await self._handle_event(button)
+			await self._contact_relay(user, button)
+		
+		def proper_timeout() -> Optional[float]:
+			"""In :var:`wait_for_aws`, if the menu does not have a timeout (`Menu.timeout = None`), :class:`None` + :class:`float`, the float being "`self._timeout + 0.1`" from v1.0.5, will fail for obvious reasons. This checks if there is no timeout, 
+			and instead of adding those two together, simply return :class:`None` to avoid :exc:`TypeError`. This would happen if the menu's :attr:`Menu.navigation_speed` was set to :attr:`Menu.FAST` and
+			the :attr:`Menu.timeout` was set to :class:`None`
+			"""
+			if self.timeout is not None:
+				return self.timeout + 0.1
+			else:
+				return None
+
+		# apply the reactions (buttons) to the menu message
+		for btn in self.__buttons:
+			await self._msg.add_reaction(btn.emoji)
+		
+		ready_event.set()
+		self._is_running = True
+		ReactionMenu._active_sessions.append(self)
+		registered_emojis = self.__extract_all_emojis()
+		client = self.__extract_proper_client()
+		menu_owner = self._extract_proper_user(self._method)
+		
+		while self._is_running:
+			try:
+				if self.__navigation_speed == ReactionMenu.NORMAL:
+					reaction, user = await client.wait_for('reaction_add', check=self.__wait_check, timeout=self.timeout)
+				elif self.__navigation_speed == ReactionMenu.FAST:
+					wait_for_aws = (
+						client.wait_for('reaction_add', check=self.__wait_check, timeout=self.timeout),
+						client.wait_for('reaction_remove', check=self.__wait_check, timeout=proper_timeout()) 
+					)
+					done, pending = await asyncio.wait(wait_for_aws, return_when=asyncio.FIRST_COMPLETED)
+					
+					temp_pending: asyncio.Task = list(pending)[0]
+					temp_pending.cancel()
+
+					temp_done: asyncio.Task = list(done)[0]
+					reaction, user = temp_done.result()
+				else:
+					raise ReactionMenuException(f'Navigation speed {self.__navigation_speed!r} is not recognized')
+			except (asyncio.TimeoutError, asyncio.CancelledError):
+				self._menu_timed_out = True
+				await self.stop(delete_menu_message=self.delete_on_timeout, clear_reactions=self.clear_reactions_after)
+			else:
+				emoji = str(reaction.emoji)
+
+				if self.remove_extra_reactions and emoji not in registered_emojis:
+					if not self.in_dms:
+						await self._msg.clear_reaction(emoji)
+						continue
+
+				for btn in self.__buttons:
+					# previous
+					if emoji == btn.emoji and btn.linked_to == ReactionButton.Type.PREVIOUS_PAGE:
+						await self._msg.edit(**self._determine_kwargs(self._pc.prev()))
+						await update_and_dispatch(emoji, user, btn)
+					
+					# next
+					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.NEXT_PAGE:
+						await self._msg.edit(**self._determine_kwargs(self._pc.next()))
+						await update_and_dispatch(emoji, user, btn)
+					
+					# first page
+					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.GO_TO_FIRST_PAGE:
+						await self._msg.edit(**self._determine_kwargs(self._pc.first_page()))
+						await update_and_dispatch(emoji, user, btn)
+					
+					# last page
+					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.GO_TO_LAST_PAGE:
+						await self._msg.edit(**self._determine_kwargs(self._pc.last_page()))
+						await update_and_dispatch(emoji, user, btn)
+					
+					# skip
+					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.SKIP:
+						await self._msg.edit(**self._determine_kwargs(self._pc.skip(btn.skip)))
+						await update_and_dispatch(emoji, user, btn)
+					
+					# go to page
+					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.GO_TO_PAGE:
+						prompt: discord.Message = await self._msg.channel.send(f'{menu_owner.display_name}, what page would you like to go to?')
+						try:
+							selection_message: discord.Message = await client.wait_for('message', check=lambda m: all([m.channel.id == self._msg.channel.id, m.author.id == menu_owner.id]), timeout=self.timeout)
+							page = int(selection_message.content)
+						except (asyncio.TimeoutError, ValueError):
+							# dont call :meth:`.stop()` here because I want the timeout factor to only be applicable after the
+							# original reactions were added
+							continue
+						else:
+							if 1 <= page <= len(self._pages):
+								self._pc.index = page - 1
+								await self._msg.edit(**self._determine_kwargs(self._pc.current_page))
+								if self.delete_interactions:
+									await prompt.delete()
+									await selection_message.delete()
+								
+								await update_and_dispatch(emoji, user, btn)
+					
+					# end session
+					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.END_SESSION:
+						await update_and_dispatch(emoji, user, btn)
+						await self.stop(delete_menu_message=True)
+					
+					# caller buttons
+					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.CALLER:
+						func = btn.details.func # type: ignore / details member "func" is mandatory
+						args = btn.details.args # type: ignore / details member "args" could be an iterable
+						kwargs = btn.details.kwargs # type: ignore / details member "kwargs" could be an dict
+						
+						try:
+							if inspect.iscoroutinefunction(func):
+								await func(*args, **kwargs) # type: ignore / `func` is already confirmed to be a coroutine
+							else:
+								func(*args, **kwargs)
+						except Exception as err:
+							raise ReactionMenuException(inspect.cleandoc(
+								f"""
+								A ReactionButton with a linked_to of ReactionButton.Type.CALLER raised an error during it's execution
+								-> {err.__class__.__name__}: {err}
+								"""
+							))
+						else:
+							await update_and_dispatch(emoji, user, btn)
+						
+					# custom buttons
+					elif emoji == btn.emoji and btn.linked_to == ReactionButton.Type.CUSTOM_EMBED:
+						await update_and_dispatch(emoji, user, btn)
+						await self._msg.edit(embed=btn.custom_embed)
+
+	async def stop(self, *, delete_menu_message: bool=False, clear_reactions: bool=False) -> None:
+		"""|coro|
+		
+		Stops the process of the menu with the option of deleting the menu's message or clearing reactions upon stop
+		
+		Parameters
+		----------
+		delete_menu_message: :class:`bool`
+			Delete the menu message
+		
+		clear_reactions: :class:`bool`
+			Remove all reactions
+		
+		Raises
+		------
+		- `discord.DiscordException`: Any exception that can be raised when deleting a message or removing a reaction from a message
+		"""
+		if self._is_running:
+			try:
+				if delete_menu_message:
+					await self._msg.delete()
+				elif clear_reactions:
+					await self._msg.clear_reactions()
+				await self._handle_on_timeout()
+			except discord.DiscordException as discord_error:
+				raise discord_error
+			finally:
+				self._is_running = False
+				self._on_close_event.set()
+				self.__main_session_task.cancel() # type: ignore / task object would have been set by the time this is executed
+	
+	def _override_dm_settings(self) -> None:
+		"""If a menu session is in a direct message the following settings are disabled/changed because of discord limitations and resource/safety reasons"""
+		if self.in_dms:
+			# Not allowed to remove reactions in DMs
+			if self.clear_reactions_after:
+				self.clear_reactions_after = False
+			
+			# Has to be set to `FAST` because bots are not allowed to remove reactions in DMs
+			if self.__navigation_speed == ReactionMenu.NORMAL:
+				self.__navigation_speed = ReactionMenu.FAST
+			
+			# Can't delete someone else's message in DMs
+			if self.delete_interactions:
+				self.delete_interactions = False
+			
+			# There are no roles in DMs
+			if self.only_roles:
+				self.only_roles = None
+			
+			# No point in having an *indefinite* menu in DMs
+			if self.timeout is None:
+				self.timeout = 60.0
+		
+	def __generate_reactionmenu_payload(self) -> dict:
+		"""Creates the parameters needed for :meth:`discord.Messageable.send()`
+
+			.. added:: v3.1.0
+		"""
+		return {
+			"content" : self._pages[0].content if self._pages else None,
+			"embed" : self._pages[0].embed if self._pages else discord.utils.MISSING,
+			"files" : self._pages[0].files if self._pages else discord.utils.MISSING,
+			"allowed_mentions" : self.allowed_mentions
+		}
+	
+	@overload
+	async def start(self, *, send_to: Optional[str]=None, reply: bool=False) -> None:
+		...
+	
+	@overload
+	async def start(self, *, send_to: Optional[int]=None, reply: bool=False) -> None:
+		...
+	
+	@overload
+	async def start(self, *, send_to: Optional[discord.TextChannel]=None, reply: bool=False) -> None:
+		...
+	
+	@overload
+	async def start(self, *, send_to: Optional[discord.VoiceChannel]=None, reply: bool=False) -> None:
+		...
+	
+	@overload
+	async def start(self, *, send_to: Optional[discord.Thread]=None, reply: bool=False) -> None:
+		...
+	
+	@ensure_not_primed
+	async def start(self, *, send_to: Optional[Union[str, int, discord.TextChannel, discord.VoiceChannel, discord.Thread]]=None, reply: bool=False) -> None:
+		"""|coro|
+		
+		Start the menu
+
+		Parameters
+		----------
+		send_to: Optional[Union[:class:`str`, :class:`int`, :class:`discord.TextChannel`, :class:`discord.VoiceChannel`, :class:`discord.Thread`]]
+			The channel/thread you'd like the menu to start in. Use the channel/threads name, ID, or it's object. Please note that if you intend to use a channel/thread object, using
+			method :meth:`discord.Client.get_channel()` (or any other related methods), that channel should be in the same list as if you were to use `ctx.guild.text_channels`
+			or `ctx.guild.threads`. This only works on a context guild channel basis. That means a menu instance cannot be created in one guild and the menu itself (:param:`send_to`)
+			be sent to another. Whichever guild context the menu was instantiated in, the channels/threads of that guild are the only options for :param:`send_to`
+
+		reply: :class:`bool`
+			Enables the menu message to reply to the message that triggered it. Parameter :param:`send_to` must be :class:`None` if this is `True`. This only pertains to a non-interaction based menu.
+
+		Raises
+		------
+		- `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+		- `NoPages`: The menu was started when no pages have been added
+		- `NoButtons`: Attempted to start the menu when no Buttons have been registered
+		- `ReactionMenuException`: The :class:`ReactionMenu`'s `menu_type` was not recognized
+		- `DescriptionOversized`: When using a `menu_type` of :attr:`ReactionMenu.TypeEmbedDynamic`, the embed description was over discords size limit
+		- `IncorrectType`: Parameter :param:`send_to` was not of the expected type
+		- `MenuException`: The channel set in :param:`send_to` was not found
+		"""
+		if ReactionMenu._sessions_limit_details.set_by_user:
+			can_proceed = await self._handle_session_limits()
+			if not can_proceed:
+				return
+		
+		self._override_dm_settings()
+		
+		if self._menu_type not in ReactionMenu._all_menu_types():
+			raise ReactionMenuException('ReactionMenu menu_type not recognized')
+		if not self.__buttons:
+			raise NoButtons
+
+		reply_kwargs = self._handle_reply_kwargs(send_to, reply)
+		menu_payload = self.__generate_reactionmenu_payload()
+
+		if isinstance(self._method, Context):
+			menu_payload.update(reply_kwargs)
+		
+		if self._menu_type == ReactionMenu.TypeEmbed:
+			if self._pages:
+				self._refresh_page_director_info(self._menu_type, self._pages)
+			
+			custom_embed_buttons = self.__get_custom_embed_buttons()
+			# no pages and no custom embeds (no pages at all)
+			if not self._pages and not custom_embed_buttons:
+				raise NoPages	
+
+			# only custom embeds
+			if not self._pages and custom_embed_buttons:
+				menu_payload['embed'] = custom_embed_buttons[0].custom_embed
+				await self._handle_send_to(send_to, menu_payload)
+			
+			# normal pages, no custom embeds
+			else:
+				await self._handle_send_to(send_to, menu_payload)
+		
+		elif self._menu_type == ReactionMenu.TypeText:
+			if not self._pages:
+				raise NoPages
+			
+			self._refresh_page_director_info(self._menu_type, self._pages)
+			menu_payload['content'] = self._pages[0].content
+			await self._handle_send_to(send_to, menu_payload)
+		
+		elif self._menu_type == ReactionMenu.TypeEmbedDynamic:
+			# page director info is refreshed in method
+			await self._build_dynamic_pages(send_to, payload=menu_payload)
+
+		ready_event = asyncio.Event()
+		self._pc = _PageController(self._pages)
+		self.__main_session_task = self.__extract_proper_client().loop.create_task(self.__paginate(ready_event))
+		self.__main_session_task.add_done_callback(self._session_done_callback)
+		await ready_event.wait()
```

### Comparing `reactionmenu-3.1.3/reactionmenu/decorators.py` & `reactionmenu-3.1.4/reactionmenu/decorators.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-"""
-MIT License
-
-Copyright (c) 2021-present Defxult#8269
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
-DEALINGS IN THE SOFTWARE.
-"""
-
-from asyncio import iscoroutinefunction
-from functools import wraps
-
-from .errors import MenuAlreadyRunning
-
-
-def ensure_not_primed(func):
-    """Check to make sure certain methods cannot be ran once the menu has been fully started"""
-    if iscoroutinefunction(func):
-        @wraps(func)
-        async def wrapper(*args, **kwargs): # type: ignore
-            inst = args[0]
-            if not inst._is_running or inst._bypass_primed:
-                if inst._bypass_primed:
-                    inst._bypass_primed = False
-                return await func(*args, **kwargs)
-            else:
-                raise MenuAlreadyRunning(f'You cannot use method "{func.__name__}" after the menu has started. Menu name: {inst.name!r}')
-        return wrapper
-    else:
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            inst = args[0]
-            if not inst._is_running or inst._bypass_primed:
-                if inst._bypass_primed:
-                    inst._bypass_primed = False
-                return func(*args, **kwargs)
-            else:
-                raise MenuAlreadyRunning(f'You cannot use method "{func.__name__}" after the menu has started. Menu name: {inst.name!r}')
-        return wrapper
+"""
+MIT License
+
+Copyright (c) 2021-present Defxult#8269
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+DEALINGS IN THE SOFTWARE.
+"""
+
+from asyncio import iscoroutinefunction
+from functools import wraps
+
+from .errors import MenuAlreadyRunning
+
+
+def ensure_not_primed(func):
+    """Check to make sure certain methods cannot be ran once the menu has been fully started"""
+    if iscoroutinefunction(func):
+        @wraps(func)
+        async def wrapper(*args, **kwargs): # type: ignore
+            inst = args[0]
+            if not inst._is_running or inst._bypass_primed:
+                if inst._bypass_primed:
+                    inst._bypass_primed = False
+                return await func(*args, **kwargs)
+            else:
+                raise MenuAlreadyRunning(f'You cannot use method "{func.__name__}" after the menu has started. Menu name: {inst.name!r}')
+        return wrapper
+    else:
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            inst = args[0]
+            if not inst._is_running or inst._bypass_primed:
+                if inst._bypass_primed:
+                    inst._bypass_primed = False
+                return func(*args, **kwargs)
+            else:
+                raise MenuAlreadyRunning(f'You cannot use method "{func.__name__}" after the menu has started. Menu name: {inst.name!r}')
+        return wrapper
```

### Comparing `reactionmenu-3.1.3/reactionmenu/errors.py` & `reactionmenu-3.1.4/reactionmenu/errors.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-"""
-MIT License
-
-Copyright (c) 2021-present Defxult#8269
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
-DEALINGS IN THE SOFTWARE.
-"""
-
-class MenuException(Exception):
-	"""Base exception for all menu's"""
-	pass
-
-class ViewMenuException(MenuException):
-	"""Base :class:`ViewMenu` exception"""
-	pass
-
-class ReactionMenuException(MenuException):
-	"""Base :class:`ReactionMenu` exception"""
-	pass
-
-class IncorrectType(MenuException):
-	"""Raised when the expected type was not given"""
-	def __init__(self, message: str):
-		super().__init__(message)
-
-class NoButtons(MenuException):
-	"""Raised when the menu was started but no buttons were registered or the action initiated requires buttons to be registered"""
-	def __init__(self, message: str='You cannot start the menu when no buttons are registered'):
-		super().__init__(message)
-
-class InvalidPage(MenuException):
-	"""Raised when the page selected to remove does not exist"""
-	pass
-	
-class DescriptionOversized(MenuException):
-	"""Used for `TypeEmbedDynamic` menus. The embed description of the menu has a character count > 4096"""
-	pass
-
-class MenuSettingsMismatch(MenuException):
-	"""Used settings for a specific `menu_type` but different/unrecognized values for those settings were given"""
-	pass
-
-class DuplicateButton(MenuException):
-	"""The emoji selected as a button has already been registered"""
-	pass
-
-class ImproperStyleFormat(MenuException):
-	"""The custom style selected by the user did not meet formatting requirements"""
-	def __init__(self):
-		super().__init__('There needs to be at least but no more than 1 "$" character and at least but no more than 1 "&" character. "$" represents the current page, "&" represents the total amount of pages. Example: "On $ out of &"')
-
-class TooManyButtons(MenuException):
-	"""The amount of buttons registered is > 20 (over discords reaction limit)"""
-	def __init__(self, message: str='Discord currently has a limit of 20 reactions or less per message. Remove 1 or more buttons'):
-		super().__init__(message)
-
-class MissingSetting(MenuException):
-	"""Raised when an action requires specific input from the user"""
-	pass
-
-class NoPages(MenuException):
-	"""Tried to start the menu when they haven't added any pages"""
-	def __init__(self, message: str="You cannot start a menu when you haven't added any pages"):
-		super().__init__(message)
-
-class MenuAlreadyRunning(MenuException):
-	"""Called a method that is not allowed to be called after the menu has started"""
-	def __init__(self, message: str):
-		super().__init__(message)
-
-class ButtonNotFound(MenuException):
-	"""Raised when :meth:`.remove_button()` did not find any matching buttons"""
-	pass
-
-class SelectNotFound(MenuException):
-	"""Raised when :meth:`.remove_select()` did not find any matching selects
-	
-		.. added:: v3.1.0
-	"""
-	pass
+"""
+MIT License
+
+Copyright (c) 2021-present Defxult#8269
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+DEALINGS IN THE SOFTWARE.
+"""
+
+class MenuException(Exception):
+	"""Base exception for all menu's"""
+	pass
+
+class ViewMenuException(MenuException):
+	"""Base :class:`ViewMenu` exception"""
+	pass
+
+class ReactionMenuException(MenuException):
+	"""Base :class:`ReactionMenu` exception"""
+	pass
+
+class IncorrectType(MenuException):
+	"""Raised when the expected type was not given"""
+	def __init__(self, message: str):
+		super().__init__(message)
+
+class NoButtons(MenuException):
+	"""Raised when the menu was started but no buttons were registered or the action initiated requires buttons to be registered"""
+	def __init__(self, message: str='You cannot start the menu when no buttons are registered'):
+		super().__init__(message)
+
+class InvalidPage(MenuException):
+	"""Raised when the page selected to remove does not exist"""
+	pass
+	
+class DescriptionOversized(MenuException):
+	"""Used for `TypeEmbedDynamic` menus. The embed description of the menu has a character count > 4096"""
+	pass
+
+class MenuSettingsMismatch(MenuException):
+	"""Used settings for a specific `menu_type` but different/unrecognized values for those settings were given"""
+	pass
+
+class DuplicateButton(MenuException):
+	"""The emoji selected as a button has already been registered"""
+	pass
+
+class ImproperStyleFormat(MenuException):
+	"""The custom style selected by the user did not meet formatting requirements"""
+	def __init__(self):
+		super().__init__('There needs to be at least but no more than 1 "$" character and at least but no more than 1 "&" character. "$" represents the current page, "&" represents the total amount of pages. Example: "On $ out of &"')
+
+class TooManyButtons(MenuException):
+	"""The amount of buttons registered is > 20 (over discords reaction limit)"""
+	def __init__(self, message: str='Discord currently has a limit of 20 reactions or less per message. Remove 1 or more buttons'):
+		super().__init__(message)
+
+class MissingSetting(MenuException):
+	"""Raised when an action requires specific input from the user"""
+	pass
+
+class NoPages(MenuException):
+	"""Tried to start the menu when they haven't added any pages"""
+	def __init__(self, message: str="You cannot start a menu when you haven't added any pages"):
+		super().__init__(message)
+
+class MenuAlreadyRunning(MenuException):
+	"""Called a method that is not allowed to be called after the menu has started"""
+	def __init__(self, message: str):
+		super().__init__(message)
+
+class ButtonNotFound(MenuException):
+	"""Raised when :meth:`.remove_button()` did not find any matching buttons"""
+	pass
+
+class SelectNotFound(MenuException):
+	"""Raised when :meth:`.remove_select()` did not find any matching selects
+	
+		.. added:: v3.1.0
+	"""
+	pass
```

### Comparing `reactionmenu-3.1.3/reactionmenu/views_menu.py` & `reactionmenu-3.1.4/reactionmenu/views_menu.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,1455 +1,1455 @@
-"""
-MIT License
-
-Copyright (c) 2021-present Defxult#8269
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
-DEALINGS IN THE SOFTWARE.
-"""
-
-from __future__ import annotations
-
-import asyncio
-import collections
-import inspect
-import random
-import re
-from typing import (
-    TYPE_CHECKING,
-    Callable,
-    Dict,
-    Final,
-    List,
-    Literal,
-    NamedTuple,
-    NoReturn,
-    Optional,
-    Sequence,
-    Union,
-    overload
-)
-
-if TYPE_CHECKING:
-    from .abc import MenuType
-
-import discord
-from discord.ext.commands import Context
-
-from . import ViewButton
-from .abc import (
-    _DEFAULT_STYLE,
-    DEFAULT_BUTTONS,
-    Page,
-    _BaseMenu,
-    _PageController
-)
-
-from .decorators import ensure_not_primed
-from .errors import *
-
-_SelectOptionRelayPayload = collections.namedtuple('_SelectOptionRelayPayload', ['func', 'only'])
-
-class ViewSelect(discord.ui.Select):
-    """A class to assist in the process of categorizing information on a :class:`ViewMenu`
-
-    Parameters
-    ----------
-    title: Union[:class:`str`, `None`]
-        The category name. If `None`, the category name defaults to "Select a category"
-    
-    options: Dict[:class:`discord.SelectOption`, List[:class:`Page`]]
-        A key/value pair associating the category options with pages to navigate
-    
-    disabled: :class:`bool`
-        If the select should start enabled or disabled
-
-        .. added:: v3.1.0
-    """
-    def __init__(self, *, title: Union[str, None], options: Dict[discord.SelectOption, List[Page]], disabled: bool=False) -> None:
-        self._menu: Optional[ViewMenu] = None
-        self._view_select_options = options
-        
-        super().__init__(custom_id=discord.utils.MISSING, placeholder='Select a category' if title is None else title, min_values=1, max_values=1, options=options.keys(), disabled=disabled, row=None) # type: ignore
-    
-    def __repr__(self) -> str:
-        return f'<ViewSelect title={self.placeholder!r} disabled={self.disabled}>'
-    
-    @property
-    def menu(self) -> Optional[ViewMenu]:
-        """
-        Returns
-        -------
-        Optional[:class:`ViewMenu`]: The menu this select is attached to. Can be `None` if not attached to any menu
-        """
-        return self._menu
-    
-    async def __dispatch_relay(self, interaction: discord.Interaction) -> None:
-        if self._menu:
-            relay_info = self._menu._options_relay_info
-            if relay_info is not None:
-                SelectOptionRelayPayload = collections.namedtuple('SelectOptionRelayPayload', ['member', 'option', 'menu'])
-                CLICKED_OPTION: Final[str] = self.values[0]
-                
-                # Find which :class:`discord.SelectOption` was clicked
-                filtered_options = [sel for sel in self._view_select_options if sel.label == CLICKED_OPTION]
-                select_option = filtered_options[0]
-                payload = SelectOptionRelayPayload(member=interaction.user, option=select_option, menu=self._menu)
-
-                async def call():
-                    if asyncio.iscoroutinefunction(relay_info.func):
-                        await relay_info.func(payload)
-                    else:
-                        relay_info.func(payload)
-                
-                if relay_info.only:
-                    for option_label in relay_info.only:
-                        if CLICKED_OPTION == option_label:
-                            await call()
-                            break
-                else:
-                    if filtered_options:
-                        await call()
-    
-    async def callback(self, interaction: discord.Interaction) -> None:
-        """*INTERNAL USE ONLY* - The callback function from the select interaction. This should not be manually called"""
-        for option, pages in self._view_select_options.items():
-            if option.label == self.values[0]:
-                if self._menu:
-                    self._menu._pc = _PageController(pages)
-                    await interaction.response.edit_message(**self._menu._determine_kwargs(self._menu._pc.first_page()))
-                    break
-        await self.__dispatch_relay(interaction)
-
-    class GoTo(discord.ui.Select):
-        """Represents a UI based version of a :class:`ViewButton` with the ID `ViewButton.ID_GO_TO_PAGE`
-
-        Parameters
-        ----------
-        title: Union[:class:`str`, `None`]
-            The selects name. If `None`, the name defaults to "Navigate to page..."
-        
-        page_numbers: This parameter accepts 3 different types and are explained below
-        - List[:class:`int`]
-            - If set to a list of integers, those specified values are the only options that are available when the select is clicked
-        
-        - Dict[:class:`int`, Union[:class:`str`, :class:`discord.Emoji`, :class:`discord.PartialEmoji`]]
-            - You can use this type if you'd like to utilize emojis in your select options
-        
-        - `ellipsis`
-            - Set an ellipsis to have the library automatically assign all page numbers to the amount of pages that you've added to the menu.
-            
-        NOTE: Setting the `page_numbers` parameter to an ellipsis (...) only works as intended if you've added the go to select AFTER you've added pages to the menu
-        
-            .. added:: v3.1.0
-        """
-        def __init__(self, *, title: Union[str, None], page_numbers: Union[List[int], Dict[int, Union[str, discord.Emoji, discord.PartialEmoji]], ellipsis]) -> None:
-            self.callback = self._select_go_to_callback
-            self._menu: Optional[ViewMenu] = None
-            self._page_numbers = page_numbers
-            self._gt_options: List[discord.SelectOption] = []
-            
-            if isinstance(page_numbers, list):
-                self._gt_options.extend([discord.SelectOption(label=str(n)) for n in page_numbers])
-            elif isinstance(page_numbers, dict):
-                for n, emoji in page_numbers.items():
-                    self._gt_options.append(discord.SelectOption(label=str(n), emoji=emoji))
-            
-            super().__init__(placeholder="Navigate to page..." if title is None else str(title), options=self._gt_options)
-        
-        @property
-        def menu(self) -> Optional[ViewMenu]:
-            """
-            Returns
-            -------
-            Optional[:class:`ViewMenu`]: The menu this select is attached to. Can be `None` if not attached to any menu
-            """
-            return self._menu
-        
-        async def _select_go_to_callback(self, interaction: discord.Interaction) -> None:
-            if interaction.data:
-                values = interaction.data.get('values') 
-                if values:
-                    CLICKED_OPTION: Final[int] = int(values[0])
-                    if self._menu:
-                        if 1 <= CLICKED_OPTION <= self._menu._pc.total_pages + 1:
-                            self._menu._pc.index = CLICKED_OPTION - 1
-                            await interaction.response.edit_message(**self._menu._determine_kwargs(self._menu._pc.current_page))
-                            return
-            else:
-                assert False, "No interaction data"
-
-class ViewMenu(_BaseMenu):
-    """A class to create a discord pagination menu using :class:`discord.ui.View`
-    
-    Parameters
-    ----------
-    method: Union[:class:`discord.ext.commands.Context`, :class:`discord.Interaction`]
-        The Context object. You can get this using a command or if you're in a `discord.on_message` event. Also accepts interactions, typically received when using slash commands
-    
-    menu_type: :class:`MenuType`
-        The configuration of the menu. Class variables :attr:`ViewMenu.TypeEmbed`, :attr:`ViewMenu.TypeEmbedDynamic`, or :attr:`ViewMenu.TypeText`
-    
-    Kwargs
-    ------
-    all_can_click: :class:`bool`
-        Sets if everyone is allowed to control when pages are 'turned' when buttons are pressed (defaults to `False`)
-    
-    allowed_mentions: :class:`discord.AllowedMentions`
-        Controls the mentions being processed in the menu message (defaults to :class:`discord.AllowedMentions(everyone=False, users=True, roles=False, replied_user=True)`).
-        Not valid for `ViewMenu` with a `menu_type` of `TypeText`
-    
-    custom_embed: :class:`discord.Embed`
-        Embed object to use when adding data with :meth:`ViewMenu.add_row()`. Used for styling purposes only (:attr:`ViewMenu.TypeEmbedDynamic` only/defaults to :class:`None`)
-    
-    delete_interactions: :class:`bool`
-        Delete the prompt message by the bot and response message by the user when asked what page they would like to go to when using :attr:`ViewButton.ID_GO_TO_PAGE` (defaults to `True`)
-    
-    delete_on_timeout: :class:`bool`
-        Delete the menu when it times out (defaults to `False`) If `True`, :attr:`disable_items_on_timeout` and :attr:`remove_items_on_timeout` will not execute regardless of if they are `True`. This takes priority over those actions
-    
-    disable_items_on_timeout: :class:`bool`
-        Disable the buttons on the menu when the menu times out (defaults to `True`) If :attr:`delete_on_timeout` is `True`, this will be overridden
-    
-    name: :class:`str`
-        A name you can set for the menu (defaults to :class:`None`)
-    
-    only_roles: List[:class:`discord.Role`]
-        If set, only members with any of the given roles are allowed to control the menu. The menu owner can always control the menu (defaults to :class:`None`)
-    
-    remove_items_on_timeout: :class:`bool`
-        Remove the buttons on the menu when the menu times out (defaults to `False`) If :attr:`disable_items_on_timeout` is `True`, this will be overridden
-    
-    rows_requested: :class:`int`
-        The amount of information per :meth:`ViewMenu.add_row()` you would like applied to each embed page (:attr:`ViewMenu.TypeEmbedDynamic` only/defaults to :class:`None`)
-    
-    show_page_director: :class:`bool`
-        Shown at the bottom of each embed page. "Page 1/20" (defaults to `True`)
-    
-    style: :class:`str`
-        A custom page director style you can select. "$" represents the current page, "&" represents the total amount of pages (defaults to "Page $/&") Example: `ViewMenu(ctx, ..., style='On $ out of &')`
-    
-    timeout: Union[:class:`int`, :class:`float`, :class:`None`]
-        The timer for when the menu times out. Can be :class:`None` for no timeout (defaults to `60.0`)
-    
-    wrap_in_codeblock: :class:`str`
-        The discord codeblock language identifier to wrap your data in (:attr:`ViewMenu.TypeEmbedDynamic` only/defaults to :class:`None`). Example: `ViewMenu(ctx, ..., wrap_in_codeblock='py')`
-    """
-    
-    _active_sessions: List[ViewMenu] = []
-    
-    def __init__(self, method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs):
-        super().__init__(method, menu_type, **kwargs)
-
-        self.__buttons: List[ViewButton] = []
-        self._stop_initiated = False
-
-        # kwargs
-        self.disable_items_on_timeout: bool = kwargs.get('disable_items_on_timeout', True)
-        self.remove_items_on_timeout: bool = kwargs.get('remove_items_on_timeout', False)
-        self.__timeout: Union[int, float, None] = kwargs.get('timeout', 60.0) # property get/set
-
-        # view
-        self.__view = discord.ui.View(timeout=self.__timeout)
-        self.__view.on_timeout = self._on_dpy_view_timeout
-        self.__view.on_error = self._on_dpy_view_error
-
-        # select
-        self.__selects: List[ViewSelect] = []
-        self._options_relay_info: Optional[_SelectOptionRelayPayload] = None
-        self._gotos: List[ViewSelect.GoTo] = []
-    
-    def __repr__(self):
-        return f'<ViewMenu name={self.name!r} owner={str(self._extract_proper_user(self._method))!r} is_running={self._is_running} timeout={self.timeout} menu_type={self._menu_type.name}>'
-
-    async def _on_dpy_view_timeout(self) -> None:
-        self._menu_timed_out = True
-        await self.stop(delete_menu_message=self.delete_on_timeout, disable_items=self.disable_items_on_timeout, remove_items=self.remove_items_on_timeout) 
-    
-    async def _on_dpy_view_error(self, interaction: discord.Interaction, error: Exception, item: discord.ui.Item) -> NoReturn:
-        try:
-            raise error
-        finally:
-            await self.stop()
-    
-    def _get_new_view(self) -> discord.ui.View:
-        """Returns a new :class:`discord.ui.View` object with the `timeout` parameter already set along with `on_timeout` and `on_error`"""
-        new_view = discord.ui.View(timeout=self.timeout)
-        new_view.on_timeout = self._on_dpy_view_timeout
-        new_view.on_error = self._on_dpy_view_error
-        return new_view
-    
-    @property
-    def selects(self) -> List[ViewSelect]:
-        """
-        Returns
-        -------
-        List[:class:`ViewSelect`]: All selects that have been added to the menu
-        
-            .. added:: v3.1.0
-        """
-        return self.__selects
-    
-    @property
-    def go_to_selects(self) -> List[ViewSelect.GoTo]:
-        """
-        Returns
-        -------
-        List[:class:`ViewSelect.GoTo`]: All go to selects that have been added to the menu
-        
-            .. added:: v3.1.0
-        """
-        return self._gotos
-    
-    @property
-    def timeout(self):
-        return self.__timeout
-    
-    @timeout.setter
-    def timeout(self, value) -> Union[int, float, None]:
-        """A property getter/setter for kwarg `timeout`"""
-        if isinstance(value, (int, float, type(None))):
-            self.__view.timeout = value
-            self.__timeout = value
-        else:
-            raise IncorrectType(f'"timeout" expected int, float, or None, got {value.__class__.__name__}')
-        
-    @property
-    def buttons(self) -> List[ViewButton]:
-        """
-        Returns
-        -------
-        List[:class:`ViewButton`]: All buttons that have been added to the menu
-        """
-        return self.__buttons
-    
-    @property
-    def buttons_most_clicked(self) -> List[ViewButton]:
-        """
-        Returns
-        -------
-        List[:class:`ViewButton`]: The list of buttons on the menu ordered from highest (button with the most clicks) to lowest (button with the least clicks). Can be an empty list if there are no buttons registered to the menu
-        """
-        return self._sort_buttons(self.__buttons)
-    
-    @classmethod
-    async def quick_start(cls, method: Union[Context, discord.Interaction], /, pages: Sequence[Union[discord.Embed, str]], buttons: Optional[Sequence[ViewButton]]=DEFAULT_BUTTONS) -> ViewMenu:
-        """|coro class method|
-        
-        Start a menu with default settings either with a `menu_type` of `ViewMenu.TypeEmbed` (all values in `pages` are of type `discord.Embed`) or `ViewMenu.TypeText` (all values in `pages` are of type `str`)
-
-        Parameters
-        ----------
-        method: Union[:class:`discord.ext.commands.Context`, :class:`discord.Interaction`]
-            The Context object. You can get this using a command or if you're in a `discord.on_message` event. Also accepts interactions, typically received when using slash commands
-
-        pages: Sequence[Union[:class:`discord.Embed`, :class:`str`]]
-            The pages to add
-
-        buttons: Optional[Sequence[:class:`ViewButton`]]
-            The buttons to add. If left as `DEFAULT_BUTTONS`, that is equivalent to `ViewButton.all()`
-        
-        Returns
-        -------
-        :class:`ViewMenu`: The menu that was started
-        
-        Raises
-        ------
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        - `NoPages`: The menu was started when no pages have been added
-        - `NoButtons`: Attempted to start the menu when no Buttons have been registered
-        - `IncorrectType`: All items in :param:`pages` were not of type :class:`discord.Embed` or :class:`str`
-        
-            .. added v3.1.0
-        """
-        menu = cls(method, menu_type=cls._quick_check(pages))
-        menu.add_pages(pages) # type: ignore
-        menu.add_buttons(ViewButton.all() if buttons is DEFAULT_BUTTONS else buttons) # type: ignore
-        await menu.start()
-        return menu
-    
-    def _should_persist(self, button: ViewButton) -> bool:
-        """Determine if a link button should stay enabled/remain on the menu when it times out or is stopped
-
-            .. added:: v3.1.0
-        """
-        return True if all([
-            button.custom_id is None,
-            button.url,
-            button.persist,
-            self._stop_initiated
-        ]) else False
-    
-    def _check(self, inter: discord.Interaction) -> bool:
-        """Base menu button interaction check. Verifies who (user, everyone, or role) can interact with the button"""
-        author_pass = False
-        if self._extract_proper_user(inter).id == self.owner.id: author_pass = True
-        if self.only_roles: self.all_can_click = False
-
-        if self.only_roles:
-            for role in self.only_roles:
-                if role in inter.user.roles: # type: ignore / will be :class:`discord.Member`. :attr:`only_roles` will always be `None` because of overridden DM settings so this line will never be reached
-                    author_pass = True
-                    break
-        if self.all_can_click:
-            author_pass = True
-
-        return author_pass
-    
-    async def _handle_event(self, button: ViewButton) -> None:
-        """|coro| If an event is set, disable/remove the buttons from the menu when the click requirement has been met"""
-        if button.event:
-            event_type = button.event.event_type
-            event_value = button.event.value
-            if button.total_clicks == event_value:
-                if event_type == ViewButton.Event._DISABLE:
-                    self.disable_button(button)
-                
-                elif event_type == ViewButton.Event._REMOVE:
-                    self.remove_button(button)
-                
-                await self.refresh_menu_items()
-    
-    def _remove_director(self, page: Page) -> Page:
-        """Removes the page director contents from the page. This is used for :meth:`ViewMenu.update()`"""
-        style = self.style
-        if style is None:
-            style = _DEFAULT_STYLE
-        
-        escaped_style = re.escape(style)
-        STYLE_PATTERN = escaped_style.replace(r'\$', r'\d{1,}').replace(r'\&', r'\d{1,}')
-        STYLE_STR_PATTERN = escaped_style.replace(r'\$', r'\d{1,}').replace(r'\&', r'(\d{1,}.*)')
-        
-        if self.show_page_director:
-            # TypeEmbed
-            if isinstance(page.embed, discord.Embed) and self._menu_type == ViewMenu.TypeEmbed:
-                embed = page.embed
-                if embed.footer.text:
-                    DIRECTOR_PATTERN = STYLE_PATTERN + r':? '
-                    if re.search(DIRECTOR_PATTERN, embed.footer.text):
-                        embed.set_footer(text=re.sub(DIRECTOR_PATTERN, '', embed.footer.text), icon_url=embed.footer.icon_url)
-                
-                return page
-            
-            # TypeText
-            elif isinstance(page.content, str) and self._menu_type == ViewMenu.TypeText:
-                if re.search(STYLE_STR_PATTERN, page.content):
-                    page.content = re.sub(STYLE_STR_PATTERN, '', page.content).rstrip('\n')
-                
-                return page
-
-            else:
-                raise TypeError(f'_remove_director parameter "page" expected discord.Embed or str, got {page.__class__.__name__}')
-        else:
-            return page
-    
-    def set_select_option_relay(self, func: Callable[[NamedTuple], None], *, only: Optional[Sequence[str]]=None) -> None:
-        """Set a function to be called with a given set of information when a select option is pressed on the menu. The information passed is `SelectOptionRelayPayload`, a named tuple.
-        The named tuple contains the following attributes:
-
-        - `member`: The :class:`discord.Member` object of the person who pressed the option. Could be :class:`discord.User` if the menu was started in a DM
-        - `option`: The :class:`discord.SelectOption` that was pressed
-        - `menu`: An instance of :class:`ViewMenu` that the select option is operating under
-
-        Parameters
-        ----------
-        func: Callable[[:class:`NamedTuple`], :class:`None`]
-            The function should only contain a single positional argument. Command functions (`@bot.command()`) not supported
-
-        only: Optional[Sequence[:class:`str`]]
-            A sequence of :class:`discord.SelectOption` labels associated with the current menu instance. If this is :class:`None`, all select options on the menu will be relayed.
-            If set, only presses from the options matching the given labels specified will be relayed
-
-        Raises
-        ------
-        - `IncorrectType`: The :param:`func` argument provided was not callable
-        
-            .. added:: v3.1.0
-        """
-        
-        if callable(func):
-            self._options_relay_info = _SelectOptionRelayPayload(func, only)
-        else:
-            raise IncorrectType('When setting the relay for a select option, argument "func" must be callable')
-    
-    def remove_select_option_relay(self) -> None:
-        """Remove the select option relay that's been set
-        
-            .. added:: v3.1.0
-        """
-        self._options_relay_info = None
-    
-    @ensure_not_primed
-    def add_select(self, select: ViewSelect) -> None:
-        """Add a select category to the menu
-
-        Parameters
-        ----------
-        select: :class:`ViewSelect`
-            The category listing to add
-        
-        Raises
-        ------
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        - `ViewMenuException`:  The `menu_type` was not of :attr:`TypeEmbed`. The "embed" parameter in a :class:`Page` was not set. Or both :class:`ViewSelect` and a :class:`ViewSelect.GoTo` were being used
-
-            .. added:: v3.1.0
-        """
-        if self._gotos:
-            raise ViewMenuException('Category selects cannot be used in conjunction with go to selects')
-        
-        pages = select._view_select_options.values()
-        for all_pages in pages:
-            for individual_page in all_pages:
-                if not individual_page.embed:
-                    raise ViewMenuException("The 'embed' parameter in a Page must be set when using selects")
-        else:
-            if self._menu_type == ViewMenu.TypeEmbed:
-                select._menu = self
-                self.__view.add_item(select)
-                self.__selects.append(select)
-            else:
-                raise ViewMenuException('Selects can only be added when the menu_type is TypeEmbed')
-    
-    def remove_select(self, select: ViewSelect) -> None:
-        """Remove a select from the menu
-        
-        Parameters
-        ----------
-        select: :class:`ViewSelect`
-            The select to remove
-        
-        Raises
-        ------
-        - `SelectNotFound`: The provided select was not found in the list of selects on the menu
-        
-            .. added:: v3.1.0
-        """
-        if select in self.__selects:
-            select._menu = None
-            self.__view.remove_item(select)
-            self.__selects.remove(select)
-        else:
-            raise SelectNotFound('Cannot remove a select that is not registered')
-    
-    def remove_all_selects(self) -> None:
-        """Remove all selects from the menu
-        
-            .. added:: v3.1.0
-        """
-        while self.__selects:
-            self.remove_select(self.__selects[0])
-
-    def disable_select(self, select: ViewSelect) -> None:
-        """Disable a select on the menu
-        
-        Parameters
-        ----------
-        select: :class:`ViewSelect`
-            The select to disable
-        
-        Raises
-        ------
-        - `SelectNotFound`: The provided select was not found in the list of selects on the menu
-        
-            .. added:: v3.1.0
-        """
-        if select in self.__selects:
-            select.disabled = True
-        else:
-            raise SelectNotFound('Cannot disable a select that is not registered')
-    
-    def disable_all_selects(self) -> None:
-        """Disable all selects on the menu
-        
-            .. added:: v3.1.0
-        """
-        for select in self.__selects:
-            select.disabled = True
-    
-    def enable_select(self, select: ViewSelect) -> None:
-        """Enable the specified select
-        
-        Parameters
-        ----------
-        select: :class:`ViewSelect`
-            The select to enable
-        
-        Raises
-        ------
-        - `SelectNotFound`: The provided select was not found in the list of selects on the menu
-        
-            .. added:: v3.1.0
-        """
-        if select in self.__selects:
-            select.disabled = False
-        else:
-            raise SelectNotFound('Cannot enable a select that is not registered')
-    
-    def enable_all_selects(self) -> None:
-        """Enable all selects on the menu
-        
-            .. added:: v3.1.0
-        """
-        for select in self.__selects:
-            self.enable_select(select)
-    
-    @overload
-    def get_select(self, title: str) -> List[ViewSelect]:
-        ...
-    
-    @overload
-    def get_select(self, title: None) -> List[ViewSelect]:
-        ...
-    
-    def get_select(self, title: Union[str, None]) -> List[ViewSelect]:
-        """Get a select by it's title (category name) that has been registered to the menu
-        
-        Parameters
-        ----------
-        title: Union[:class:`str`, `None`]
-            Title of the category
-        
-        Returns
-        -------
-        List[:class:`ViewSelect`]: All selects matching the given title
-        """
-        return [select for select in self.__selects if select.placeholder == title]
-    
-    @ensure_not_primed
-    def add_go_to_select(self, goto: ViewSelect.GoTo) -> None:
-        """Add a select where the user can choose which page they'd like to navigate to.
-
-        Parameters
-        ----------
-        goto: :class:`ViewSelect.GoTo`
-            The navigation listing
-        
-        Raises
-        ------
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        - `ViewMenuException`:  A :class:`ViewSelect` was already added to the menu. A :class:`ViewSelect` and a :class:`ViewSelect.GoTo` cannot both be used on a single menu 
-
-            .. added:: v3.1.0
-        """
-        if not self.__selects:
-            goto._menu = self
-            if goto._page_numbers is ...:
-                for n in range(1, len(self._pages) + 1):
-                    goto._gt_options.append(discord.SelectOption(label=str(n)))
-            self._gotos.append(goto)
-            self.__view.add_item(goto)
-        else:
-            raise ViewMenuException('Category selects cannot be used in conjunction with go to selects')
-    
-    def enable_go_to_select(self, goto: ViewSelect.GoTo) -> None:
-        """Enable the specified go to select
-
-        Parameters
-        ----------
-        goto: :class:`ViewSelect.GoTo`
-            The go to select to enable
-        
-            .. added:: v3.1.0
-        """
-        if goto in self._gotos:
-            goto.disabled = False
-    
-    def enable_all_go_to_selects(self) -> None:
-        """Enable all go to selects
-        
-            .. added:: v3.1.0
-        """
-        for goto in self._gotos:
-            goto.disabled = False
-    
-    def disable_go_to_select(self, goto: ViewSelect.GoTo) -> None:
-        """Disable the specified go to select
-
-        Parameters
-        ----------
-        goto: :class:`ViewSelect.GoTo`
-            The go to select to disable
-        
-            .. added:: v3.1.0
-        """
-        if goto in self._gotos:
-            goto.disabled = True
-    
-    def disable_all_go_to_selects(self) -> None:
-        """Disable all go to selects
-        
-            .. added:: v3.1.0
-        """
-        for goto in self._gotos:
-            goto.disabled = True
-    
-    def remove_go_to_select(self, goto: ViewSelect.GoTo) -> None:
-        """Remove a go to select from the menu
-        
-        Parameters
-        ----------
-        goto: :class:`ViewSelect.GoTo`
-            The go to select to remove
-        
-        Raises
-        ------
-        - `SelectNotFound`: The provided go to select was not found in the list of selects on the menu
-        
-            .. added:: v3.1.0
-        """
-        if goto in self._gotos:
-            goto._menu = None
-            self.__view.remove_item(goto)
-            self._gotos.remove(goto)
-        else:
-            raise SelectNotFound('Cannot remove a go to select that is not registered')
-
-    def remove_all_go_to_selects(self) -> None:
-        """Remove all go to selects from the menu
-        
-            .. added:: v3.1.0
-        """
-        while self._gotos:
-            self.remove_go_to_select(self._gotos[0])
-    
-    async def update(self, *, new_pages: Union[List[Union[discord.Embed, str]], None], new_buttons: Union[List[ViewButton], None]) -> None:
-        """|coro|
-        
-        When the menu is running, update the pages or buttons. It should be noted that `ViewSelect`s are not supported here, and they will automatically be removed
-        once the menu is updated. This method only supports pages and buttons.
-        
-        Parameters
-        ----------
-        new_pages: List[Union[:class:`discord.Embed`, :class:`str`]]
-            Pages to *replace* the current pages with. If the menus current `menu_type` is :attr:`ViewMenu.TypeEmbed`, only :class:`discord.Embed` can be used. If :attr:`ViewMenu.TypeText`, only :class:`str` can be used. If you
-            don't want to replace any pages, set this to :class:`None`
-        
-        new_buttons: List[:class:`ViewButton`]
-            Buttons to *replace* the current buttons with. Can be an empty list if you want the updated menu to have no buttons. Can also be set to :class:`None` if you don't want to replace any buttons
-        
-        Raises
-        ------
-        - `ViewMenuException`: The :class:`ViewButton` custom_id was not recognized or a :class:`ViewButton` with that ID has already been added
-        - `TooManyButtons`: There are already 25 buttons on the menu
-        - `IncorrectType`: The values in :param:`new_pages` did not match the :class:`ViewMenu`'s `menu_type`. An attempt to use this method when the `menu_type` is :attr:`ViewMenu.TypeEmbedDynamic` which is not allowed. Or
-        all :param:`new_buttons` values were not of type :class:`ViewButton`
-        """
-        if self._is_running:
-            # ----------------------- CHECKS -----------------------
-
-            # Note: button count > 25 check is done in :meth:`ViewMenu.add_button`
-            
-            if new_pages is None and new_buttons is None:
-                return
-
-            if self._menu_type not in (ViewMenu.TypeEmbed, ViewMenu.TypeText):
-                raise IncorrectType('Updating a menu is only valid for a menu with menu_type ViewMenu.TypeEmbed or ViewMenu.TypeText')
-            
-            if self._menu_type == ViewMenu.TypeEmbed and new_pages:
-                if not all([isinstance(page, discord.Embed) for page in new_pages]):
-                    raise IncorrectType('When updating the menu, all values must be of type discord.Embed because the current menu_type is ViewMenu.TypeEmbed')
-            
-            if self._menu_type == ViewMenu.TypeText and new_pages:
-                if not all([isinstance(page, str) for page in new_pages]):
-                    raise IncorrectType('When updating the menu, all values must be of type str because the current menu_type is ViewMenu.TypeText')
-            
-            if isinstance(new_pages, list) and len(new_pages) == 0:
-                raise ViewMenuException('new_pages cannot be an empty list. Must be None if no new pages should be added')
-            
-            # ----------------------- END CHECKS -----------------------
-
-            if new_pages is not None:
-                # TypeEmbed
-                if self._menu_type == ViewMenu.TypeEmbed:
-                    for new_embed_page in new_pages:
-                        self._remove_director(Page(embed=new_embed_page)) # type: ignore / contains embed if TypeEmbed
-                    
-                    self._pages = [Page(embed=e) for e in new_pages.copy()] # type: ignore
-                    self._pc = _PageController(self._pages)
-                    self._refresh_page_director_info(ViewMenu.TypeEmbed, self._pages)
-                
-                # TypeText
-                else:
-                    removed_director_info: List[Page] = []
-                    for new_str_page in new_pages.copy():
-                        removed_director_info.append(self._remove_director(Page(content=new_str_page))) # type: ignore
-                    
-                    self._pages = removed_director_info.copy()
-                    self._pc = _PageController(self._pages)
-                    self._refresh_page_director_info(ViewMenu.TypeText, self._pages)
-            else:
-                # page controller needs to be reset because even though there are no new pages. the page index is still in the location BEFORE the update
-                # EXAMPLE: 5 page menu > click Next button  (on page 2) > update menu no new pages > click Next button (on page 3)
-                # that makes no sense and resetting the page controller fixes that issue 
-                self._pc = _PageController(self._pages)
-            
-            kwargs_to_pass = {}
-            self.remove_all_selects()
-
-            self.__view.stop()
-            self.__view = self._get_new_view()
-
-            # re-using current buttons
-            if isinstance(new_buttons, type(None)):
-                original_buttons = self.__buttons.copy()
-                self.remove_all_buttons()
-                for orig_button in original_buttons:
-                    self._bypass_primed = True
-                    self.add_button(orig_button)
-            
-            # using new buttons
-            elif isinstance(new_buttons, list):
-                self.remove_all_buttons()
-                if len(new_buttons) >= 1: # empty lists mean all buttons will be removed
-                    for new_btn in new_buttons:
-                        self._bypass_primed = True
-                        self.add_button(new_btn)
-            
-            kwargs_to_pass['view'] = self.__view
-            
-            if self._menu_type == ViewMenu.TypeEmbed:
-                kwargs_to_pass['embed'] = self._pages[0].embed
-            else:
-                kwargs_to_pass['content'] = self._pages[0].content
-            
-            await self._msg.edit(**kwargs_to_pass)
-    
-    def randomize_button_styles(self) -> None:
-        """Set all buttons currently registered to the menu to a random :class:`discord.ButtonStyle` excluding link buttons"""
-        all_styles = (
-            discord.ButtonStyle.blurple,
-            discord.ButtonStyle.green,
-            discord.ButtonStyle.gray,
-            discord.ButtonStyle.red
-        )
-        for btn in [button for button in self.__buttons if button.style not in (discord.ButtonStyle.link, discord.ButtonStyle.url)]:
-            btn.style = random.choice(all_styles)
-    
-    def set_button_styles(self, style: discord.ButtonStyle) -> None:
-        """Set all buttons currently registered to the menu to the specified :class:`discord.ButtonStyle` excluding link buttons
-        
-        Parameters
-        ----------
-        style: :class:`discord.ButtonStyle`
-            The button style to set
-        """
-        for btn in [button for button in self.__buttons if button.style not in (discord.ButtonStyle.link, discord.ButtonStyle.url)]:
-            btn.style = style
-    
-    async def refresh_menu_items(self) -> None:
-        """|coro|
-        
-        When the menu is running, update the message to reflect the buttons/selects that were removed, enabled, or disabled
-        """
-        if self._is_running:
-            current_items = self.__view.children.copy()
-            self.remove_all_buttons()
-            self.remove_all_selects()
-            self.remove_all_go_to_selects()
-            self.__view.stop()
-            self.__view = self._get_new_view()
-            for item in current_items:
-                self._bypass_primed = True
-                if isinstance(item, discord.ui.Select):
-                    if item.__class__.__name__ == "ViewSelect":
-                        self.add_select(item) # type: ignore / it's subclassed
-                    elif item.__class__.__name__ == "GoTo":
-                        self.add_go_to_select(item) # type: ignore / it's subclassed
-                elif isinstance(item, ViewButton):
-                    self.add_button(item)
-                elif isinstance(item, ViewSelect.GoTo):
-                    self.add_go_to_select(item)
-            await self._msg.edit(view=self.__view)
-    
-    def remove_button(self, button: ViewButton) -> None:
-        """Remove a button from the menu
-        
-        Parameters
-        ----------
-        button: :class:`ViewButton`
-            The button to remove
-        
-        Raises
-        ------
-        - `ButtonNotFound`: The provided button was not found in the list of buttons on the menu
-        """
-        if button in self.__buttons:
-            button._menu = None
-            self.__buttons.remove(button)
-            self.__view.remove_item(button)
-        else:
-            raise ButtonNotFound('Cannot remove a button that is not registered')
-    
-    def remove_all_buttons(self) -> None:
-        """Remove all buttons from the menu"""
-        # Set persists
-        persistent_link_buttons: List[ViewButton] = []
-        for btn in self.__buttons:
-            if self._should_persist(btn):
-                persistent_link_buttons.append(btn)
-                continue
-        else:
-            while self.__buttons:
-                self.remove_button(self.__buttons[0])
-            else:
-                for plb in persistent_link_buttons:
-                    self._bypass_primed = True
-                    self.add_button(plb)
-    
-    def disable_button(self, button: ViewButton) -> None:
-        """Disable a button on the menu
-        
-        Parameters
-        ----------
-        button: :class:`ViewButton`
-            The button to disable
-        
-        Raises
-        ------
-        - `ButtonNotFound`: The provided button was not found in the list of buttons on the menu
-        """
-        if button in self.__buttons:
-            idx = self.__buttons.index(button)
-            self.__buttons[idx].disabled = True
-        else:
-            raise ButtonNotFound('Cannot disable a button that is not registered')
-    
-    def disable_all_buttons(self) -> None:
-        """Disable all buttons on the menu"""
-        for btn in self.__buttons:
-            if self._should_persist(btn): continue
-            btn.disabled = True
-    
-    def enable_button(self, button: ViewButton) -> None:
-        """Enable the specified button
-        
-        Parameters
-        ----------
-        button: :class:`ViewButton`
-            The button to enable
-        
-        Raises
-        ------
-        - `ButtonNotFound`: The provided button was not found in the list of buttons on the menu
-        """
-        if button in self.__buttons:
-            idx = self.__buttons.index(button)
-            self.__buttons[idx].disabled = False
-        else:
-            raise ButtonNotFound('Cannot enable a button that is not registered')
-    
-    def enable_all_buttons(self) -> None:
-        """Enable all buttons on the menu"""
-        for btn in self.__buttons:
-            btn.disabled = False
-    
-    def _button_add_check(self, button: ViewButton) -> None:
-        """A set of checks to ensure the proper button is being added"""
-        # ensure they are using only the ViewButton and not ReactionMenus :class:`ReactionButton`
-        if isinstance(button, ViewButton):
-
-            # ensure the button custom_id is a valid one, but skip this check if its a link button because they dont have custom_ids
-            if button.style == discord.ButtonStyle.link:
-                pass
-            else:
-                # Note: this needs to be an re search because of buttons with an ID of "[ID]_[unique ID]"
-                if not re.search(ViewButton._RE_IDs, button.custom_id): # type: ignore
-                    raise ViewMenuException(f'ViewButton custom_id {button.custom_id!r} was not recognized')
-            
-            # ensure there are no duplicate custom_ids for the base navigation buttons
-            # Note: there's no need to have a check for buttons that are not navigation buttons because they have a unique ID and duplicates of those are allowed
-            active_button_ids: List[str] = [btn.custom_id for btn in self.__buttons] # type: ignore
-            if button.custom_id in active_button_ids:
-                if not all([button.custom_id is None, button.style == discord.ButtonStyle.link]):
-                    name = ViewButton._get_id_name_from_id(button.custom_id)
-                    raise ViewMenuException(f'A ViewButton with custom_id {name!r} has already been added')
-            
-            # if the menu_type is TypeText, disallow custom embed buttons
-            if button.style != discord.ButtonStyle.link and self._menu_type == ViewMenu.TypeText:
-                if button.custom_id == ViewButton.ID_CUSTOM_EMBED:
-                    if button.followup and button.followup.embed is not None:
-                        raise MenuSettingsMismatch('ViewButton with custom_id ViewButton.ID_CUSTOM_EMBED cannot be used when the menu_type is ViewMenu.TypeText')
-            
-            # if using a skip button, ensure the skip attribute was set
-            if button.custom_id == ViewButton.ID_SKIP and button.skip is None:
-                raise ViewMenuException('When attempting to add a button custom_id ViewButton.ID_SKIP, the "skip" kwarg was not set')
-            
-            # ensure there are no more than 25 buttons
-            if len(self.__buttons) >= 25:
-                raise TooManyButtons('ViewMenu cannot have more than 25 buttons (discord limitation)')
-        else:
-            raise IncorrectType(f'When adding a button to the ViewMenu, the button type must be ViewButton, got {button.__class__.__name__}')
-    
-    def _maybe_unique_id(self, button: ViewButton) -> None:
-        """Create a unique ID if the `custom_id` for buttons that are allowed to have duplicates
-        
-            Note ::
-                This excludes link buttons because they don't have a `custom_id`
-        """
-        if button.custom_id in (ViewButton.ID_CALLER, ViewButton.ID_SEND_MESSAGE, ViewButton.ID_CUSTOM_EMBED, ViewButton.ID_SKIP):
-            button.custom_id = f'{button.custom_id}_{id(button)}'
-    
-    @ensure_not_primed
-    def add_button(self, button: ViewButton) -> None:
-        """Add a button to the menu
-        
-        Parameters
-        ----------
-        button: :class:`ViewButton`
-            The button to add
-        
-        Raises
-        ------
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        - `MenuSettingsMismatch`: The buttons custom_id was set as :attr:`ViewButton.ID_CUSTOM_EMBED` but the `menu_type` is :attr:`ViewMenu.TypeText`
-        - `ViewMenuException`: The custom_id for the button was not recognized or a button with that custom_id has already been added
-        - `TooManyButtons`: There are already 25 buttons on the menu
-        - `IncorrectType`: Parameter :param:`button` was not of type :class:`ViewButton`
-        """
-        self._button_add_check(button)
-        self._maybe_unique_id(button)
-
-        button._menu = self
-        self.__view.add_item(button)
-        self.__buttons.append(button)
-    
-    @ensure_not_primed
-    def add_buttons(self, buttons: Sequence[ViewButton]) -> None:
-        """Add multiple buttons to the menu at once
-        
-        Parameters
-        ----------
-        buttons: Sequence[:class:`ViewButton`]
-            The buttons to add
-        
-        Raises
-        ------
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        - `MenuSettingsMismatch`: One of the buttons `custom_id` was set as :attr:`ViewButton.ID_CUSTOM_EMBED` but the `menu_type` is :attr:`ViewMenu.TypeText`
-        - `ViewMenuException`: The `custom_id` for a button was not recognized or a button with that `custom_id` has already been added
-        - `TooManyButtons`: There are already 25 buttons on the menu
-        - `IncorrectType`: One or more values supplied in parameter :param:`buttons` was not of type :class:`ViewButton`
-        """
-        for btn in buttons:
-            self.add_button(btn)
-    
-    def get_button(self, identity: str, *, search_by: Literal['label', 'id', 'name']='label') -> List[ViewButton]:
-        """Get a button that has been registered to the menu by it's label, custom_id, or name
-        
-        Parameters
-        ----------
-        identity: :class:`str`
-            The button label, custom_id, or name
-        
-        search_by: :class:`str`
-            How to search for the button. If "label", it's searched by button labels. If "id", it's searched by it's custom_id. 
-            If "name", it's searched by button names
-        
-        Returns
-        -------
-        List[:class:`ViewButton`]: The button(s) matching the given identity
-        
-        Raises
-        ------
-        - `ViewMenuException`: Parameter :param:`search_by` was not "label", "id", or "name"
-        """
-        identity = str(identity)
-        search_by = str(search_by).lower() # type: ignore
-
-        if search_by == 'label':
-            matched_labels: List[ViewButton] = [btn for btn in self.__buttons if btn.label and btn.label == identity]
-            return matched_labels
-        
-        elif search_by == 'id':
-            matched_ids: List[ViewButton] = [btn for btn in self.__buttons if btn.custom_id and btn.custom_id.startswith(identity)]
-            return matched_ids
-        
-        elif search_by == 'name':
-            matched_names: List[ViewButton] = [btn for btn in self.__buttons if btn.name and btn.name == identity]
-            return matched_names
-        
-        else:
-            raise ViewMenuException(f'Parameter "search_by" expected "label", "id", or "name", got {search_by!r}')
-
-    async def _paginate(self, button: ViewButton, inter: discord.Interaction) -> None:
-        """|coro| When the button is pressed, handle the pagination process"""
-        if not self._check(inter):
-            await inter.response.defer()
-            return
-        
-        button._update_statistics(inter.user)
-        await self._handle_event(button)
-        
-        if button.custom_id == ViewButton.ID_PREVIOUS_PAGE:
-            await inter.response.edit_message(**self._determine_kwargs(self._pc.prev()))
-        
-        elif button.custom_id == ViewButton.ID_NEXT_PAGE:
-            await inter.response.edit_message(**self._determine_kwargs(self._pc.next()))
-        
-        elif button.custom_id == ViewButton.ID_GO_TO_FIRST_PAGE:
-            await inter.response.edit_message(**self._determine_kwargs(self._pc.first_page()))
-        
-        elif button.custom_id == ViewButton.ID_GO_TO_LAST_PAGE:
-            await inter.response.edit_message(**self._determine_kwargs(self._pc.last_page()))
-        
-        elif button.custom_id == ViewButton.ID_GO_TO_PAGE:
-            await inter.response.defer()
-            prompt: discord.Message = await self._msg.channel.send(f'{inter.user.display_name}, what page would you like to go to?') # type: ignore / `.channel` is know at this point
-            try:
-                selection_message: discord.Message = await inter.client.wait_for('message', check=lambda m: all([m.channel.id == self._msg.channel.id, m.author.id == inter.user.id]), timeout=self.timeout) # type: ignore / `.channel` is know at this point
-                page = int(selection_message.content)
-            except (asyncio.TimeoutError, ValueError):
-                return
-            else:
-                if 1 <= page <= len(self._pages):
-                    self._pc.index = page - 1
-                    await self._msg.edit(**self._determine_kwargs(self._pc.current_page))
-                    if self.delete_interactions:
-                        await prompt.delete()
-                        await selection_message.delete()
-        
-        elif button.custom_id == ViewButton.ID_END_SESSION:
-            await self.stop(delete_menu_message=True)
-        
-        else:
-            #* NOTE: Link buttons, aka buttons with a `custom_id` of `None` do not send interactions, so there's no need for an if check
-
-            if button.custom_id.startswith(ViewButton.ID_CALLER): # type: ignore
-                if button.followup is None or button.followup.details is None:
-                    error_msg = 'ViewButton custom_id was set as ViewButton.ID_CALLER but the "followup" kwarg for that ViewButton was not set ' \
-                                'or method ViewButton.Followup.set_caller_details(..) was not called to set the caller information'
-                    raise ViewMenuException(error_msg)
-                
-                func = button.followup.details.func
-                args = button.followup.details.args
-                kwargs = button.followup.details.kwargs
-
-                # reply now because we don't know how long the users function will take to execute
-                await inter.response.defer()
-
-                try:
-                    if asyncio.iscoroutinefunction(func): await func(*args, **kwargs) # type: ignore / `func` is already confirmed to be a coroutine
-                    else: func(*args, **kwargs)
-                except Exception as err:
-                    call_failed_error_msg = inspect.cleandoc(
-                        f"""
-                        The button with custom_id ViewButton.ID_CALLER with the label "{button.label}" raised an error during it's execution
-                        -> {err.__class__.__name__}: {err}
-                        """
-                    )
-                    raise ViewMenuException(call_failed_error_msg)
-                else:
-                    if button.followup:
-                        # if this executes, the user doesn't want to respond with a message, only with the caller function (already called ^)
-                        if all((button.followup.content is None, button.followup.embed is None, button.followup.file is None)):
-                            pass
-                        else:
-                            followup_kwargs = button.followup._to_dict()
-
-                            # inter.followup() has no attribute delete_after/details, so manually delete the key/val pairs to avoid :exc:`TypeError`, got an unexpected kwarg
-                            del followup_kwargs['delete_after']
-                            del followup_kwargs['details']
-                            
-                            # if there's no file, remove it to avoid an NoneType error
-                            if followup_kwargs['file'] is None:
-                                del followup_kwargs['file']
-                            
-                            followup_message: discord.WebhookMessage = await inter.followup.send(**followup_kwargs)
-                            
-                            if button.followup.delete_after:
-                                await followup_message.delete(delay=button.followup.delete_after)
-            
-            elif button.custom_id.startswith(ViewButton.ID_SEND_MESSAGE): # type: ignore
-                if button.followup is None:
-                    raise ViewMenuException('ViewButton custom_id was set as ViewButton.ID_SEND_MESSAGE but the "followup" kwarg for that ViewButton was not set')
-                
-                # there must be at least 1. cannot send an empty message
-                if all((button.followup.content is None, button.followup.embed is None, button.followup.file is None)):
-                    raise ViewMenuException('When using a ViewButton with a custom_id of ViewButton.ID_SEND_MESSAGE, the followup message cannot be empty')
-                
-                followup_kwargs = button.followup._to_dict()
-
-                # inter.followup.send() has no kwarg "details"
-                del followup_kwargs['details']
-                
-                # files are ignored
-                del followup_kwargs['file']
-                
-                # inter.followup.send() has no kwarg "delete_after"
-                del followup_kwargs['delete_after']
-
-                # defer instead of inter.response.send_message() so `delete_after` and `allowed_mentions` can be used
-                # inter.followup.send() is used instead
-                await inter.response.defer()
-
-                sent_message: discord.WebhookMessage = await inter.followup.send(**followup_kwargs)
-                if button.followup.delete_after:
-                    await sent_message.delete(delay=button.followup.delete_after)
-            
-            elif button.custom_id.startswith(ViewButton.ID_CUSTOM_EMBED): # type: ignore
-                if self._menu_type not in (ViewMenu.TypeEmbed, ViewMenu.TypeEmbedDynamic):
-                    raise ViewMenuException('Buttons with custom_id ViewButton.ID_CUSTOM_EMBED can only be used when the menu_type is ViewMenu.TypeEmbed or ViewMenu.TypeEmbedDynamic')
-                else:
-                    if button.followup is None or button.followup.embed is None:
-                        raise ViewMenuException('ViewButton custom_id was set as ViewButton.ID_CUSTOM_EMBED but the "followup" kwargs for that ViewButton was not set or the "embed" kwarg for the followup was not set')
-                   
-                    await inter.response.edit_message(embed=button.followup.embed)            
-            
-            elif button.custom_id.startswith(ViewButton.ID_SKIP): # type: ignore
-                await inter.response.edit_message(**self._determine_kwargs(self._pc.skip(button.skip)))
-            
-            else:
-                # this shouldn't execute because of :meth:`_button_add_check`, but just in case i missed something, raise the appropriate error
-                raise ViewMenuException(f'ViewButton custom_id {button.custom_id!r} was not recognized')
-
-        await self._contact_relay(inter.user, button)
-
-    async def stop(self, *, delete_menu_message: bool=False, disable_items: bool=False, remove_items: bool=False) -> None:
-        """|coro|
-        
-        Stops the process of the menu with the option of deleting the menu's message, removing the buttons, or disabling the buttons upon stop
-        
-        Parameters
-        ----------
-        delete_menu_message: :class:`bool`
-            Delete the message the menu is operating from
-
-        disable_items: :class:`bool`
-            Disable the buttons & selects on the menu
-        
-        remove_items: :class:`bool`
-            Remove the buttons & selects from the menu
-
-        Parameter Hierarchy
-        -------------------
-        Only one option is available when stopping the menu. If you have multiple parameters as `True`, only one will execute
-        - `disable_items` > `remove_items`
-
-        Raises
-        ------
-        - `discord.DiscordException`: Any exception that can be raised when deleting or editing a message
-        """
-        if self._is_running:
-            self._stop_initiated = True
-            try:
-                if delete_menu_message:
-                    await self._msg.delete()
-                else:
-                    already_disabled = False
-                    if disable_items:
-                        self.disable_all_buttons()
-                        self.disable_all_selects()
-                        self.disable_all_go_to_selects()
-                        already_disabled = True
-                        await self._msg.edit(view=self.__view)
-                    
-                    if remove_items and not already_disabled:
-                        self.remove_all_buttons()
-                        self.remove_all_selects()
-                        self.remove_all_go_to_selects()
-                        await self._msg.edit(view=self.__view)
-            
-            except discord.DiscordException as dpy_error:
-                raise dpy_error
-            
-            finally:
-                self.__view.stop()
-                self._is_running = False
-
-                if self in ViewMenu._active_sessions:
-                    ViewMenu._active_sessions.remove(self)
-                
-                self._on_close_event.set()
-                await self._handle_on_timeout()
-    
-    def _override_dm_settings(self) -> None:
-        """If a menu session is in a direct message the following settings are disabled/changed because of discord limitations and resource/safety reasons
-        
-            .. added:: v3.1.0
-        """
-        if self.in_dms:
-            # Can't delete someone else's message in DMs
-            if self.delete_interactions:
-                self.delete_interactions = False
-            
-            # There are no roles in DMs
-            if self.only_roles:
-                self.only_roles = None
-            
-            # No point in having an *indefinite* menu in DMs
-            if self.timeout is None:
-                self.timeout = 60.0
-    
-    def __generate_viewmenu_payload(self) -> dict:
-        """Creates the parameters needed for :meth:`discord.Messageable.send()`
-        
-            .. added:: v3.1.0
-        """
-        return {
-            "content" : self._pages[0].content if self._pages else None,
-            "embed" : self._pages[0].embed if self._pages else discord.utils.MISSING,
-            "files" : self._pages[0].files if self._pages else discord.utils.MISSING,
-            "view" : self.__view,
-            "allowed_mentions" : self.allowed_mentions
-        }
-    
-    def __refresh_select_pages(self, menu_type: MenuType) -> None:
-        if self.__selects:
-            for vm_select in self.__selects:
-                for pages in vm_select._view_select_options.values():
-                    self._refresh_page_director_info(menu_type, pages)
-
-    @overload
-    async def start(self, *, send_to: Optional[str]=None, reply: bool=False) -> None:
-        ...
-    
-    @overload
-    async def start(self, *, send_to: Optional[int]=None, reply: bool=False) -> None:
-        ...
-    
-    @overload
-    async def start(self, *, send_to: Optional[discord.TextChannel]=None, reply: bool=False) -> None:
-        ...
-    
-    @overload
-    async def start(self, *, send_to: Optional[discord.VoiceChannel]=None, reply: bool=False) -> None:
-        ...
-    
-    @overload
-    async def start(self, *, send_to: Optional[discord.Thread]=None, reply: bool=False) -> None:
-        ...
-    
-    @ensure_not_primed
-    async def start(self, *, send_to: Optional[Union[str, int, discord.TextChannel, discord.VoiceChannel, discord.Thread]]=None, reply: bool=False) -> None:
-        """|coro|
-        
-        Start the menu
-        
-        Parameters
-        ----------
-        send_to: Optional[Union[:class:`str`, :class:`int`, :class:`discord.TextChannel`, :class:`discord.VoiceChannel`, :class:`discord.Thread`]]
-			The channel/thread you'd like the menu to start in. Use the channel/threads name, ID, or it's object. Please note that if you intend to use a channel/thread object, using
-			method :meth:`discord.Client.get_channel()` (or any other related methods), that channel should be in the same list as if you were to use `ctx.guild.text_channels`
-			or `ctx.guild.threads`. This only works on a context guild channel basis. That means a menu instance cannot be created in one guild and the menu itself (:param:`send_to`)
-			be sent to another. Whichever guild context the menu was instantiated in, the channels/threads of that guild are the only options for :param:`send_to`
-
-            Note: This parameter is not available if your `method` is a :class:`discord.Interaction`, aka a slash command
-        
-        reply: :class:`bool`
-            Enables the menu message to reply to the message that triggered it. Parameter :param:`send_to` must be :class:`None` if this is `True`. This only pertains to a non-interaction based menu.
-        
-        Raises
-        ------
-        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
-        - `NoPages`: The menu was started when no pages have been added
-        - `NoButtons`: Attempted to start the menu when no Buttons have been registered
-        - `ViewMenuException`: The :class:`ViewMenu`'s `menu_type` was not recognized. There were more than one base navigation buttons. Or a :attr:`ViewButton.ID_CUSTOM_EMBED` button was not correctly formatted
-        - `DescriptionOversized`: When using a `menu_type` of :attr:`ViewMenu.TypeEmbedDynamic`, the embed description was over discords size limit
-        - `IncorrectType`: Parameter :param:`send_to` was not of the expected type
-        - `MenuException`: The channel set in :param:`send_to` was not found
-        """
-        if ViewMenu._sessions_limit_details.set_by_user:
-            can_proceed = await self._handle_session_limits()
-            if not can_proceed:
-                return
-        
-        self._override_dm_settings()
-        
-        # checks
-        # Note 1: each at least 1 page check is done in it's own if statement to avoid clashing between pages and custom embeds
-        # Note 2: at least 1 page check for add_row is done in "(dynamic menu)"
-        
-        # ensure at least 1 button exists before starting the menu
-        if not self.__buttons: raise NoButtons
-        if self._menu_type not in ViewMenu._all_menu_types(): raise ViewMenuException('ViewMenu menu_type not recognized')
-
-        reply_kwargs = self._handle_reply_kwargs(send_to, reply)
-        menu_payload = self.__generate_viewmenu_payload()
-        
-        if isinstance(self._method, Context):
-            menu_payload.update(reply_kwargs)
-
-        # add page (normal menu)
-        if self._menu_type == ViewMenu.TypeEmbed:
-            self._refresh_page_director_info(ViewMenu.TypeEmbed, self._pages)
-
-            navigation_btns = [btn for btn in self.__buttons if btn.custom_id in ViewButton._base_nav_buttons()]
-
-            # an re search is required here because buttons with ID_CUSTOM_EMBED dont have a normal ID, the ID is "8_[unique ID]"
-            custom_embed_btns = [btn for btn in self.__buttons if btn.style != discord.ButtonStyle.link and re.search(r'8_\d+', btn.custom_id)] # type: ignore / raw string is compatible
-
-            if all([not self._pages, not custom_embed_btns]):
-                raise NoPages
-
-            # normal pages, no custom embeds
-            if self._pages and not custom_embed_btns:
-                await self._handle_send_to(send_to, menu_payload)
-            
-            # only custom embeds
-            elif not self._pages and custom_embed_btns:
-                # since there are only custom embeds, there is no need for base navigation buttons, so remove them if any
-                for nav_btn in navigation_btns:
-                    if nav_btn in self.__buttons:
-                        self.__buttons.remove(nav_btn)
-                
-                # ensure all custom embed buttons have the proper values set
-                for custom_btn in custom_embed_btns:
-                    if custom_btn.followup is None or custom_btn.followup.embed is None:
-                        raise ViewMenuException('ViewButton custom_id was set as ViewButton.ID_CUSTOM_EMBED but the "followup" kwargs for that ViewButton was not set or the "embed" kwarg for the followup was not set')
-                
-                # since there are only custom embeds, self._pages is still set to :class:`None`, so set the embed in `.send()` to the first custom embed in the list
-                menu_payload['embed'] = custom_embed_btns[0].followup.embed # type: ignore
-                await self._handle_send_to(send_to, menu_payload)
-            
-            # normal pages and custom embeds
-            else:
-                # since there are custom embeds, ensure there is at least one base navigation button so they can switch between the normal pages and custom embeds
-                if not navigation_btns:
-                    error_msg = inspect.cleandoc(
-                        """
-                        Since you've added pages and custom embeds, there needs to be at least one base navigation button. Without one, there's no way to go back to the normal pages in the menu if a custom embed button is pressed.
-                        The available base navigation buttons are buttons with the custom_id:
-                        - ViewButton.ID_PREVIOUS_PAGE
-                        - ViewButton.ID_NEXT_PAGE
-                        - ViewButton.ID_GO_TO_FIRST_PAGE
-                        - ViewButton.ID_GO_TO_LAST_PAGE
-                        - ViewButton.ID_GO_TO_PAGE
-                        """
-                    )
-                    raise ViewMenuException(error_msg)
-                else:
-                    await self._handle_send_to(send_to, menu_payload)
-            
-            self.__refresh_select_pages(ViewMenu.TypeEmbed)
-
-        # add row (dynamic menu)
-        elif self._menu_type == ViewMenu.TypeEmbedDynamic:
-            await self._build_dynamic_pages(send_to, view=self.__view, payload=menu_payload)
-        
-        # add page (text menu)
-        else:
-            if not self._pages:
-                raise NoPages
-            
-            self._refresh_page_director_info(ViewMenu.TypeText, self._pages)
-            menu_payload['content'] = self._pages[0].content # reassign the first page to show to director information
-            await self._handle_send_to(send_to, menu_payload)
-        
-        self._pc = _PageController(self._pages)
-        self._is_running = True
-        ViewMenu._active_sessions.append(self)
+"""
+MIT License
+
+Copyright (c) 2021-present Defxult#8269
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+import asyncio
+import collections
+import inspect
+import random
+import re
+from typing import (
+    TYPE_CHECKING,
+    Callable,
+    Dict,
+    Final,
+    List,
+    Literal,
+    NamedTuple,
+    NoReturn,
+    Optional,
+    Sequence,
+    Union,
+    overload
+)
+
+if TYPE_CHECKING:
+    from .abc import MenuType
+
+import discord
+from discord.ext.commands import Context
+
+from . import ViewButton
+from .abc import (
+    _DEFAULT_STYLE,
+    DEFAULT_BUTTONS,
+    Page,
+    _BaseMenu,
+    _PageController
+)
+
+from .decorators import ensure_not_primed
+from .errors import *
+
+_SelectOptionRelayPayload = collections.namedtuple('_SelectOptionRelayPayload', ['func', 'only'])
+
+class ViewSelect(discord.ui.Select):
+    """A class to assist in the process of categorizing information on a :class:`ViewMenu`
+
+    Parameters
+    ----------
+    title: Union[:class:`str`, `None`]
+        The category name. If `None`, the category name defaults to "Select a category"
+    
+    options: Dict[:class:`discord.SelectOption`, List[:class:`Page`]]
+        A key/value pair associating the category options with pages to navigate
+    
+    disabled: :class:`bool`
+        If the select should start enabled or disabled
+
+        .. added:: v3.1.0
+    """
+    def __init__(self, *, title: Union[str, None], options: Dict[discord.SelectOption, List[Page]], disabled: bool=False) -> None:
+        self._menu: Optional[ViewMenu] = None
+        self._view_select_options = options
+        
+        super().__init__(custom_id=discord.utils.MISSING, placeholder='Select a category' if title is None else title, min_values=1, max_values=1, options=options.keys(), disabled=disabled, row=None) # type: ignore
+    
+    def __repr__(self) -> str:
+        return f'<ViewSelect title={self.placeholder!r} disabled={self.disabled}>'
+    
+    @property
+    def menu(self) -> Optional[ViewMenu]:
+        """
+        Returns
+        -------
+        Optional[:class:`ViewMenu`]: The menu this select is attached to. Can be `None` if not attached to any menu
+        """
+        return self._menu
+    
+    async def __dispatch_relay(self, interaction: discord.Interaction) -> None:
+        if self._menu:
+            relay_info = self._menu._options_relay_info
+            if relay_info is not None:
+                SelectOptionRelayPayload = collections.namedtuple('SelectOptionRelayPayload', ['member', 'option', 'menu'])
+                CLICKED_OPTION: Final[str] = self.values[0]
+                
+                # Find which :class:`discord.SelectOption` was clicked
+                filtered_options = [sel for sel in self._view_select_options if sel.label == CLICKED_OPTION]
+                select_option = filtered_options[0]
+                payload = SelectOptionRelayPayload(member=interaction.user, option=select_option, menu=self._menu)
+
+                async def call():
+                    if asyncio.iscoroutinefunction(relay_info.func):
+                        await relay_info.func(payload)
+                    else:
+                        relay_info.func(payload)
+                
+                if relay_info.only:
+                    for option_label in relay_info.only:
+                        if CLICKED_OPTION == option_label:
+                            await call()
+                            break
+                else:
+                    if filtered_options:
+                        await call()
+    
+    async def callback(self, interaction: discord.Interaction) -> None:
+        """*INTERNAL USE ONLY* - The callback function from the select interaction. This should not be manually called"""
+        for option, pages in self._view_select_options.items():
+            if option.label == self.values[0]:
+                if self._menu:
+                    self._menu._pc = _PageController(pages)
+                    await interaction.response.edit_message(**self._menu._determine_kwargs(self._menu._pc.first_page()))
+                    break
+        await self.__dispatch_relay(interaction)
+
+    class GoTo(discord.ui.Select):
+        """Represents a UI based version of a :class:`ViewButton` with the ID `ViewButton.ID_GO_TO_PAGE`
+
+        Parameters
+        ----------
+        title: Union[:class:`str`, `None`]
+            The selects name. If `None`, the name defaults to "Navigate to page..."
+        
+        page_numbers: This parameter accepts 3 different types and are explained below
+        - List[:class:`int`]
+            - If set to a list of integers, those specified values are the only options that are available when the select is clicked
+        
+        - Dict[:class:`int`, Union[:class:`str`, :class:`discord.Emoji`, :class:`discord.PartialEmoji`]]
+            - You can use this type if you'd like to utilize emojis in your select options
+        
+        - `ellipsis`
+            - Set an ellipsis to have the library automatically assign all page numbers to the amount of pages that you've added to the menu.
+            
+        NOTE: Setting the `page_numbers` parameter to an ellipsis (...) only works as intended if you've added the go to select AFTER you've added pages to the menu
+        
+            .. added:: v3.1.0
+        """
+        def __init__(self, *, title: Union[str, None], page_numbers: Union[List[int], Dict[int, Union[str, discord.Emoji, discord.PartialEmoji]], ellipsis]) -> None:
+            self.callback = self._select_go_to_callback
+            self._menu: Optional[ViewMenu] = None
+            self._page_numbers = page_numbers
+            self._gt_options: List[discord.SelectOption] = []
+            
+            if isinstance(page_numbers, list):
+                self._gt_options.extend([discord.SelectOption(label=str(n)) for n in page_numbers])
+            elif isinstance(page_numbers, dict):
+                for n, emoji in page_numbers.items():
+                    self._gt_options.append(discord.SelectOption(label=str(n), emoji=emoji))
+            
+            super().__init__(placeholder="Navigate to page..." if title is None else str(title), options=self._gt_options)
+        
+        @property
+        def menu(self) -> Optional[ViewMenu]:
+            """
+            Returns
+            -------
+            Optional[:class:`ViewMenu`]: The menu this select is attached to. Can be `None` if not attached to any menu
+            """
+            return self._menu
+        
+        async def _select_go_to_callback(self, interaction: discord.Interaction) -> None:
+            if interaction.data:
+                values = interaction.data.get('values') 
+                if values:
+                    CLICKED_OPTION: Final[int] = int(values[0])
+                    if self._menu:
+                        if 1 <= CLICKED_OPTION <= self._menu._pc.total_pages + 1:
+                            self._menu._pc.index = CLICKED_OPTION - 1
+                            await interaction.response.edit_message(**self._menu._determine_kwargs(self._menu._pc.current_page))
+                            return
+            else:
+                assert False, "No interaction data"
+
+class ViewMenu(_BaseMenu):
+    """A class to create a discord pagination menu using :class:`discord.ui.View`
+    
+    Parameters
+    ----------
+    method: Union[:class:`discord.ext.commands.Context`, :class:`discord.Interaction`]
+        The Context object. You can get this using a command or if you're in a `discord.on_message` event. Also accepts interactions, typically received when using slash commands
+    
+    menu_type: :class:`MenuType`
+        The configuration of the menu. Class variables :attr:`ViewMenu.TypeEmbed`, :attr:`ViewMenu.TypeEmbedDynamic`, or :attr:`ViewMenu.TypeText`
+    
+    Kwargs
+    ------
+    all_can_click: :class:`bool`
+        Sets if everyone is allowed to control when pages are 'turned' when buttons are pressed (defaults to `False`)
+    
+    allowed_mentions: :class:`discord.AllowedMentions`
+        Controls the mentions being processed in the menu message (defaults to :class:`discord.AllowedMentions(everyone=False, users=True, roles=False, replied_user=True)`).
+        Not valid for `ViewMenu` with a `menu_type` of `TypeText`
+    
+    custom_embed: :class:`discord.Embed`
+        Embed object to use when adding data with :meth:`ViewMenu.add_row()`. Used for styling purposes only (:attr:`ViewMenu.TypeEmbedDynamic` only/defaults to :class:`None`)
+    
+    delete_interactions: :class:`bool`
+        Delete the prompt message by the bot and response message by the user when asked what page they would like to go to when using :attr:`ViewButton.ID_GO_TO_PAGE` (defaults to `True`)
+    
+    delete_on_timeout: :class:`bool`
+        Delete the menu when it times out (defaults to `False`) If `True`, :attr:`disable_items_on_timeout` and :attr:`remove_items_on_timeout` will not execute regardless of if they are `True`. This takes priority over those actions
+    
+    disable_items_on_timeout: :class:`bool`
+        Disable the buttons on the menu when the menu times out (defaults to `True`) If :attr:`delete_on_timeout` is `True`, this will be overridden
+    
+    name: :class:`str`
+        A name you can set for the menu (defaults to :class:`None`)
+    
+    only_roles: List[:class:`discord.Role`]
+        If set, only members with any of the given roles are allowed to control the menu. The menu owner can always control the menu (defaults to :class:`None`)
+    
+    remove_items_on_timeout: :class:`bool`
+        Remove the buttons on the menu when the menu times out (defaults to `False`) If :attr:`disable_items_on_timeout` is `True`, this will be overridden
+    
+    rows_requested: :class:`int`
+        The amount of information per :meth:`ViewMenu.add_row()` you would like applied to each embed page (:attr:`ViewMenu.TypeEmbedDynamic` only/defaults to :class:`None`)
+    
+    show_page_director: :class:`bool`
+        Shown at the bottom of each embed page. "Page 1/20" (defaults to `True`)
+    
+    style: :class:`str`
+        A custom page director style you can select. "$" represents the current page, "&" represents the total amount of pages (defaults to "Page $/&") Example: `ViewMenu(ctx, ..., style='On $ out of &')`
+    
+    timeout: Union[:class:`int`, :class:`float`, :class:`None`]
+        The timer for when the menu times out. Can be :class:`None` for no timeout (defaults to `60.0`)
+    
+    wrap_in_codeblock: :class:`str`
+        The discord codeblock language identifier to wrap your data in (:attr:`ViewMenu.TypeEmbedDynamic` only/defaults to :class:`None`). Example: `ViewMenu(ctx, ..., wrap_in_codeblock='py')`
+    """
+    
+    _active_sessions: List[ViewMenu] = []
+    
+    def __init__(self, method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs):
+        super().__init__(method, menu_type, **kwargs)
+
+        self.__buttons: List[ViewButton] = []
+        self._stop_initiated = False
+
+        # kwargs
+        self.disable_items_on_timeout: bool = kwargs.get('disable_items_on_timeout', True)
+        self.remove_items_on_timeout: bool = kwargs.get('remove_items_on_timeout', False)
+        self.__timeout: Union[int, float, None] = kwargs.get('timeout', 60.0) # property get/set
+
+        # view
+        self.__view = discord.ui.View(timeout=self.__timeout)
+        self.__view.on_timeout = self._on_dpy_view_timeout
+        self.__view.on_error = self._on_dpy_view_error
+
+        # select
+        self.__selects: List[ViewSelect] = []
+        self._options_relay_info: Optional[_SelectOptionRelayPayload] = None
+        self._gotos: List[ViewSelect.GoTo] = []
+    
+    def __repr__(self):
+        return f'<ViewMenu name={self.name!r} owner={str(self._extract_proper_user(self._method))!r} is_running={self._is_running} timeout={self.timeout} menu_type={self._menu_type.name}>'
+
+    async def _on_dpy_view_timeout(self) -> None:
+        self._menu_timed_out = True
+        await self.stop(delete_menu_message=self.delete_on_timeout, disable_items=self.disable_items_on_timeout, remove_items=self.remove_items_on_timeout) 
+    
+    async def _on_dpy_view_error(self, interaction: discord.Interaction, error: Exception, item: discord.ui.Item) -> NoReturn:
+        try:
+            raise error
+        finally:
+            await self.stop()
+    
+    def _get_new_view(self) -> discord.ui.View:
+        """Returns a new :class:`discord.ui.View` object with the `timeout` parameter already set along with `on_timeout` and `on_error`"""
+        new_view = discord.ui.View(timeout=self.timeout)
+        new_view.on_timeout = self._on_dpy_view_timeout
+        new_view.on_error = self._on_dpy_view_error
+        return new_view
+    
+    @property
+    def selects(self) -> List[ViewSelect]:
+        """
+        Returns
+        -------
+        List[:class:`ViewSelect`]: All selects that have been added to the menu
+        
+            .. added:: v3.1.0
+        """
+        return self.__selects
+    
+    @property
+    def go_to_selects(self) -> List[ViewSelect.GoTo]:
+        """
+        Returns
+        -------
+        List[:class:`ViewSelect.GoTo`]: All go to selects that have been added to the menu
+        
+            .. added:: v3.1.0
+        """
+        return self._gotos
+    
+    @property
+    def timeout(self):
+        return self.__timeout
+    
+    @timeout.setter
+    def timeout(self, value) -> Union[int, float, None]:
+        """A property getter/setter for kwarg `timeout`"""
+        if isinstance(value, (int, float, type(None))):
+            self.__view.timeout = value
+            self.__timeout = value
+        else:
+            raise IncorrectType(f'"timeout" expected int, float, or None, got {value.__class__.__name__}')
+        
+    @property
+    def buttons(self) -> List[ViewButton]:
+        """
+        Returns
+        -------
+        List[:class:`ViewButton`]: All buttons that have been added to the menu
+        """
+        return self.__buttons
+    
+    @property
+    def buttons_most_clicked(self) -> List[ViewButton]:
+        """
+        Returns
+        -------
+        List[:class:`ViewButton`]: The list of buttons on the menu ordered from highest (button with the most clicks) to lowest (button with the least clicks). Can be an empty list if there are no buttons registered to the menu
+        """
+        return self._sort_buttons(self.__buttons)
+    
+    @classmethod
+    async def quick_start(cls, method: Union[Context, discord.Interaction], /, pages: Sequence[Union[discord.Embed, str]], buttons: Optional[Sequence[ViewButton]]=DEFAULT_BUTTONS) -> ViewMenu:
+        """|coro class method|
+        
+        Start a menu with default settings either with a `menu_type` of `ViewMenu.TypeEmbed` (all values in `pages` are of type `discord.Embed`) or `ViewMenu.TypeText` (all values in `pages` are of type `str`)
+
+        Parameters
+        ----------
+        method: Union[:class:`discord.ext.commands.Context`, :class:`discord.Interaction`]
+            The Context object. You can get this using a command or if you're in a `discord.on_message` event. Also accepts interactions, typically received when using slash commands
+
+        pages: Sequence[Union[:class:`discord.Embed`, :class:`str`]]
+            The pages to add
+
+        buttons: Optional[Sequence[:class:`ViewButton`]]
+            The buttons to add. If left as `DEFAULT_BUTTONS`, that is equivalent to `ViewButton.all()`
+        
+        Returns
+        -------
+        :class:`ViewMenu`: The menu that was started
+        
+        Raises
+        ------
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        - `NoPages`: The menu was started when no pages have been added
+        - `NoButtons`: Attempted to start the menu when no Buttons have been registered
+        - `IncorrectType`: All items in :param:`pages` were not of type :class:`discord.Embed` or :class:`str`
+        
+            .. added v3.1.0
+        """
+        menu = cls(method, menu_type=cls._quick_check(pages))
+        menu.add_pages(pages) # type: ignore
+        menu.add_buttons(ViewButton.all() if buttons is DEFAULT_BUTTONS else buttons) # type: ignore
+        await menu.start()
+        return menu
+    
+    def _should_persist(self, button: ViewButton) -> bool:
+        """Determine if a link button should stay enabled/remain on the menu when it times out or is stopped
+
+            .. added:: v3.1.0
+        """
+        return True if all([
+            button.custom_id is None,
+            button.url,
+            button.persist,
+            self._stop_initiated
+        ]) else False
+    
+    def _check(self, inter: discord.Interaction) -> bool:
+        """Base menu button interaction check. Verifies who (user, everyone, or role) can interact with the button"""
+        author_pass = False
+        if self._extract_proper_user(inter).id == self.owner.id: author_pass = True
+        if self.only_roles: self.all_can_click = False
+
+        if self.only_roles:
+            for role in self.only_roles:
+                if role in inter.user.roles: # type: ignore / will be :class:`discord.Member`. :attr:`only_roles` will always be `None` because of overridden DM settings so this line will never be reached
+                    author_pass = True
+                    break
+        if self.all_can_click:
+            author_pass = True
+
+        return author_pass
+    
+    async def _handle_event(self, button: ViewButton) -> None:
+        """|coro| If an event is set, disable/remove the buttons from the menu when the click requirement has been met"""
+        if button.event:
+            event_type = button.event.event_type
+            event_value = button.event.value
+            if button.total_clicks == event_value:
+                if event_type == ViewButton.Event._DISABLE:
+                    self.disable_button(button)
+                
+                elif event_type == ViewButton.Event._REMOVE:
+                    self.remove_button(button)
+                
+                await self.refresh_menu_items()
+    
+    def _remove_director(self, page: Page) -> Page:
+        """Removes the page director contents from the page. This is used for :meth:`ViewMenu.update()`"""
+        style = self.style
+        if style is None:
+            style = _DEFAULT_STYLE
+        
+        escaped_style = re.escape(style)
+        STYLE_PATTERN = escaped_style.replace(r'\$', r'\d{1,}').replace(r'\&', r'\d{1,}')
+        STYLE_STR_PATTERN = escaped_style.replace(r'\$', r'\d{1,}').replace(r'\&', r'(\d{1,}.*)')
+        
+        if self.show_page_director:
+            # TypeEmbed
+            if isinstance(page.embed, discord.Embed) and self._menu_type == ViewMenu.TypeEmbed:
+                embed = page.embed
+                if embed.footer.text:
+                    DIRECTOR_PATTERN = STYLE_PATTERN + r':? '
+                    if re.search(DIRECTOR_PATTERN, embed.footer.text):
+                        embed.set_footer(text=re.sub(DIRECTOR_PATTERN, '', embed.footer.text), icon_url=embed.footer.icon_url)
+                
+                return page
+            
+            # TypeText
+            elif isinstance(page.content, str) and self._menu_type == ViewMenu.TypeText:
+                if re.search(STYLE_STR_PATTERN, page.content):
+                    page.content = re.sub(STYLE_STR_PATTERN, '', page.content).rstrip('\n')
+                
+                return page
+
+            else:
+                raise TypeError(f'_remove_director parameter "page" expected discord.Embed or str, got {page.__class__.__name__}')
+        else:
+            return page
+    
+    def set_select_option_relay(self, func: Callable[[NamedTuple], None], *, only: Optional[Sequence[str]]=None) -> None:
+        """Set a function to be called with a given set of information when a select option is pressed on the menu. The information passed is `SelectOptionRelayPayload`, a named tuple.
+        The named tuple contains the following attributes:
+
+        - `member`: The :class:`discord.Member` object of the person who pressed the option. Could be :class:`discord.User` if the menu was started in a DM
+        - `option`: The :class:`discord.SelectOption` that was pressed
+        - `menu`: An instance of :class:`ViewMenu` that the select option is operating under
+
+        Parameters
+        ----------
+        func: Callable[[:class:`NamedTuple`], :class:`None`]
+            The function should only contain a single positional argument. Command functions (`@bot.command()`) not supported
+
+        only: Optional[Sequence[:class:`str`]]
+            A sequence of :class:`discord.SelectOption` labels associated with the current menu instance. If this is :class:`None`, all select options on the menu will be relayed.
+            If set, only presses from the options matching the given labels specified will be relayed
+
+        Raises
+        ------
+        - `IncorrectType`: The :param:`func` argument provided was not callable
+        
+            .. added:: v3.1.0
+        """
+        
+        if callable(func):
+            self._options_relay_info = _SelectOptionRelayPayload(func, only)
+        else:
+            raise IncorrectType('When setting the relay for a select option, argument "func" must be callable')
+    
+    def remove_select_option_relay(self) -> None:
+        """Remove the select option relay that's been set
+        
+            .. added:: v3.1.0
+        """
+        self._options_relay_info = None
+    
+    @ensure_not_primed
+    def add_select(self, select: ViewSelect) -> None:
+        """Add a select category to the menu
+
+        Parameters
+        ----------
+        select: :class:`ViewSelect`
+            The category listing to add
+        
+        Raises
+        ------
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        - `ViewMenuException`:  The `menu_type` was not of :attr:`TypeEmbed`. The "embed" parameter in a :class:`Page` was not set. Or both :class:`ViewSelect` and a :class:`ViewSelect.GoTo` were being used
+
+            .. added:: v3.1.0
+        """
+        if self._gotos:
+            raise ViewMenuException('Category selects cannot be used in conjunction with go to selects')
+        
+        pages = select._view_select_options.values()
+        for all_pages in pages:
+            for individual_page in all_pages:
+                if not individual_page.embed:
+                    raise ViewMenuException("The 'embed' parameter in a Page must be set when using selects")
+        else:
+            if self._menu_type == ViewMenu.TypeEmbed:
+                select._menu = self
+                self.__view.add_item(select)
+                self.__selects.append(select)
+            else:
+                raise ViewMenuException('Selects can only be added when the menu_type is TypeEmbed')
+    
+    def remove_select(self, select: ViewSelect) -> None:
+        """Remove a select from the menu
+        
+        Parameters
+        ----------
+        select: :class:`ViewSelect`
+            The select to remove
+        
+        Raises
+        ------
+        - `SelectNotFound`: The provided select was not found in the list of selects on the menu
+        
+            .. added:: v3.1.0
+        """
+        if select in self.__selects:
+            select._menu = None
+            self.__view.remove_item(select)
+            self.__selects.remove(select)
+        else:
+            raise SelectNotFound('Cannot remove a select that is not registered')
+    
+    def remove_all_selects(self) -> None:
+        """Remove all selects from the menu
+        
+            .. added:: v3.1.0
+        """
+        while self.__selects:
+            self.remove_select(self.__selects[0])
+
+    def disable_select(self, select: ViewSelect) -> None:
+        """Disable a select on the menu
+        
+        Parameters
+        ----------
+        select: :class:`ViewSelect`
+            The select to disable
+        
+        Raises
+        ------
+        - `SelectNotFound`: The provided select was not found in the list of selects on the menu
+        
+            .. added:: v3.1.0
+        """
+        if select in self.__selects:
+            select.disabled = True
+        else:
+            raise SelectNotFound('Cannot disable a select that is not registered')
+    
+    def disable_all_selects(self) -> None:
+        """Disable all selects on the menu
+        
+            .. added:: v3.1.0
+        """
+        for select in self.__selects:
+            select.disabled = True
+    
+    def enable_select(self, select: ViewSelect) -> None:
+        """Enable the specified select
+        
+        Parameters
+        ----------
+        select: :class:`ViewSelect`
+            The select to enable
+        
+        Raises
+        ------
+        - `SelectNotFound`: The provided select was not found in the list of selects on the menu
+        
+            .. added:: v3.1.0
+        """
+        if select in self.__selects:
+            select.disabled = False
+        else:
+            raise SelectNotFound('Cannot enable a select that is not registered')
+    
+    def enable_all_selects(self) -> None:
+        """Enable all selects on the menu
+        
+            .. added:: v3.1.0
+        """
+        for select in self.__selects:
+            self.enable_select(select)
+    
+    @overload
+    def get_select(self, title: str) -> List[ViewSelect]:
+        ...
+    
+    @overload
+    def get_select(self, title: None) -> List[ViewSelect]:
+        ...
+    
+    def get_select(self, title: Union[str, None]) -> List[ViewSelect]:
+        """Get a select by it's title (category name) that has been registered to the menu
+        
+        Parameters
+        ----------
+        title: Union[:class:`str`, `None`]
+            Title of the category
+        
+        Returns
+        -------
+        List[:class:`ViewSelect`]: All selects matching the given title
+        """
+        return [select for select in self.__selects if select.placeholder == title]
+    
+    @ensure_not_primed
+    def add_go_to_select(self, goto: ViewSelect.GoTo) -> None:
+        """Add a select where the user can choose which page they'd like to navigate to.
+
+        Parameters
+        ----------
+        goto: :class:`ViewSelect.GoTo`
+            The navigation listing
+        
+        Raises
+        ------
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        - `ViewMenuException`:  A :class:`ViewSelect` was already added to the menu. A :class:`ViewSelect` and a :class:`ViewSelect.GoTo` cannot both be used on a single menu 
+
+            .. added:: v3.1.0
+        """
+        if not self.__selects:
+            goto._menu = self
+            if goto._page_numbers is ...:
+                for n in range(1, len(self._pages) + 1):
+                    goto._gt_options.append(discord.SelectOption(label=str(n)))
+            self._gotos.append(goto)
+            self.__view.add_item(goto)
+        else:
+            raise ViewMenuException('Category selects cannot be used in conjunction with go to selects')
+    
+    def enable_go_to_select(self, goto: ViewSelect.GoTo) -> None:
+        """Enable the specified go to select
+
+        Parameters
+        ----------
+        goto: :class:`ViewSelect.GoTo`
+            The go to select to enable
+        
+            .. added:: v3.1.0
+        """
+        if goto in self._gotos:
+            goto.disabled = False
+    
+    def enable_all_go_to_selects(self) -> None:
+        """Enable all go to selects
+        
+            .. added:: v3.1.0
+        """
+        for goto in self._gotos:
+            goto.disabled = False
+    
+    def disable_go_to_select(self, goto: ViewSelect.GoTo) -> None:
+        """Disable the specified go to select
+
+        Parameters
+        ----------
+        goto: :class:`ViewSelect.GoTo`
+            The go to select to disable
+        
+            .. added:: v3.1.0
+        """
+        if goto in self._gotos:
+            goto.disabled = True
+    
+    def disable_all_go_to_selects(self) -> None:
+        """Disable all go to selects
+        
+            .. added:: v3.1.0
+        """
+        for goto in self._gotos:
+            goto.disabled = True
+    
+    def remove_go_to_select(self, goto: ViewSelect.GoTo) -> None:
+        """Remove a go to select from the menu
+        
+        Parameters
+        ----------
+        goto: :class:`ViewSelect.GoTo`
+            The go to select to remove
+        
+        Raises
+        ------
+        - `SelectNotFound`: The provided go to select was not found in the list of selects on the menu
+        
+            .. added:: v3.1.0
+        """
+        if goto in self._gotos:
+            goto._menu = None
+            self.__view.remove_item(goto)
+            self._gotos.remove(goto)
+        else:
+            raise SelectNotFound('Cannot remove a go to select that is not registered')
+
+    def remove_all_go_to_selects(self) -> None:
+        """Remove all go to selects from the menu
+        
+            .. added:: v3.1.0
+        """
+        while self._gotos:
+            self.remove_go_to_select(self._gotos[0])
+    
+    async def update(self, *, new_pages: Union[List[Union[discord.Embed, str]], None], new_buttons: Union[List[ViewButton], None]) -> None:
+        """|coro|
+        
+        When the menu is running, update the pages or buttons. It should be noted that `ViewSelect`s are not supported here, and they will automatically be removed
+        once the menu is updated. This method only supports pages and buttons.
+        
+        Parameters
+        ----------
+        new_pages: List[Union[:class:`discord.Embed`, :class:`str`]]
+            Pages to *replace* the current pages with. If the menus current `menu_type` is :attr:`ViewMenu.TypeEmbed`, only :class:`discord.Embed` can be used. If :attr:`ViewMenu.TypeText`, only :class:`str` can be used. If you
+            don't want to replace any pages, set this to :class:`None`
+        
+        new_buttons: List[:class:`ViewButton`]
+            Buttons to *replace* the current buttons with. Can be an empty list if you want the updated menu to have no buttons. Can also be set to :class:`None` if you don't want to replace any buttons
+        
+        Raises
+        ------
+        - `ViewMenuException`: The :class:`ViewButton` custom_id was not recognized or a :class:`ViewButton` with that ID has already been added
+        - `TooManyButtons`: There are already 25 buttons on the menu
+        - `IncorrectType`: The values in :param:`new_pages` did not match the :class:`ViewMenu`'s `menu_type`. An attempt to use this method when the `menu_type` is :attr:`ViewMenu.TypeEmbedDynamic` which is not allowed. Or
+        all :param:`new_buttons` values were not of type :class:`ViewButton`
+        """
+        if self._is_running:
+            # ----------------------- CHECKS -----------------------
+
+            # Note: button count > 25 check is done in :meth:`ViewMenu.add_button`
+            
+            if new_pages is None and new_buttons is None:
+                return
+
+            if self._menu_type not in (ViewMenu.TypeEmbed, ViewMenu.TypeText):
+                raise IncorrectType('Updating a menu is only valid for a menu with menu_type ViewMenu.TypeEmbed or ViewMenu.TypeText')
+            
+            if self._menu_type == ViewMenu.TypeEmbed and new_pages:
+                if not all([isinstance(page, discord.Embed) for page in new_pages]):
+                    raise IncorrectType('When updating the menu, all values must be of type discord.Embed because the current menu_type is ViewMenu.TypeEmbed')
+            
+            if self._menu_type == ViewMenu.TypeText and new_pages:
+                if not all([isinstance(page, str) for page in new_pages]):
+                    raise IncorrectType('When updating the menu, all values must be of type str because the current menu_type is ViewMenu.TypeText')
+            
+            if isinstance(new_pages, list) and len(new_pages) == 0:
+                raise ViewMenuException('new_pages cannot be an empty list. Must be None if no new pages should be added')
+            
+            # ----------------------- END CHECKS -----------------------
+
+            if new_pages is not None:
+                # TypeEmbed
+                if self._menu_type == ViewMenu.TypeEmbed:
+                    for new_embed_page in new_pages:
+                        self._remove_director(Page(embed=new_embed_page)) # type: ignore / contains embed if TypeEmbed
+                    
+                    self._pages = [Page(embed=e) for e in new_pages.copy()] # type: ignore
+                    self._pc = _PageController(self._pages)
+                    self._refresh_page_director_info(ViewMenu.TypeEmbed, self._pages)
+                
+                # TypeText
+                else:
+                    removed_director_info: List[Page] = []
+                    for new_str_page in new_pages.copy():
+                        removed_director_info.append(self._remove_director(Page(content=new_str_page))) # type: ignore
+                    
+                    self._pages = removed_director_info.copy()
+                    self._pc = _PageController(self._pages)
+                    self._refresh_page_director_info(ViewMenu.TypeText, self._pages)
+            else:
+                # page controller needs to be reset because even though there are no new pages. the page index is still in the location BEFORE the update
+                # EXAMPLE: 5 page menu > click Next button  (on page 2) > update menu no new pages > click Next button (on page 3)
+                # that makes no sense and resetting the page controller fixes that issue 
+                self._pc = _PageController(self._pages)
+            
+            kwargs_to_pass = {}
+            self.remove_all_selects()
+
+            self.__view.stop()
+            self.__view = self._get_new_view()
+
+            # re-using current buttons
+            if isinstance(new_buttons, type(None)):
+                original_buttons = self.__buttons.copy()
+                self.remove_all_buttons()
+                for orig_button in original_buttons:
+                    self._bypass_primed = True
+                    self.add_button(orig_button)
+            
+            # using new buttons
+            elif isinstance(new_buttons, list):
+                self.remove_all_buttons()
+                if len(new_buttons) >= 1: # empty lists mean all buttons will be removed
+                    for new_btn in new_buttons:
+                        self._bypass_primed = True
+                        self.add_button(new_btn)
+            
+            kwargs_to_pass['view'] = self.__view
+            
+            if self._menu_type == ViewMenu.TypeEmbed:
+                kwargs_to_pass['embed'] = self._pages[0].embed
+            else:
+                kwargs_to_pass['content'] = self._pages[0].content
+            
+            await self._msg.edit(**kwargs_to_pass)
+    
+    def randomize_button_styles(self) -> None:
+        """Set all buttons currently registered to the menu to a random :class:`discord.ButtonStyle` excluding link buttons"""
+        all_styles = (
+            discord.ButtonStyle.blurple,
+            discord.ButtonStyle.green,
+            discord.ButtonStyle.gray,
+            discord.ButtonStyle.red
+        )
+        for btn in [button for button in self.__buttons if button.style not in (discord.ButtonStyle.link, discord.ButtonStyle.url)]:
+            btn.style = random.choice(all_styles)
+    
+    def set_button_styles(self, style: discord.ButtonStyle) -> None:
+        """Set all buttons currently registered to the menu to the specified :class:`discord.ButtonStyle` excluding link buttons
+        
+        Parameters
+        ----------
+        style: :class:`discord.ButtonStyle`
+            The button style to set
+        """
+        for btn in [button for button in self.__buttons if button.style not in (discord.ButtonStyle.link, discord.ButtonStyle.url)]:
+            btn.style = style
+    
+    async def refresh_menu_items(self) -> None:
+        """|coro|
+        
+        When the menu is running, update the message to reflect the buttons/selects that were removed, enabled, or disabled
+        """
+        if self._is_running:
+            current_items = self.__view.children.copy()
+            self.remove_all_buttons()
+            self.remove_all_selects()
+            self.remove_all_go_to_selects()
+            self.__view.stop()
+            self.__view = self._get_new_view()
+            for item in current_items:
+                self._bypass_primed = True
+                if isinstance(item, discord.ui.Select):
+                    if item.__class__.__name__ == "ViewSelect":
+                        self.add_select(item) # type: ignore / it's subclassed
+                    elif item.__class__.__name__ == "GoTo":
+                        self.add_go_to_select(item) # type: ignore / it's subclassed
+                elif isinstance(item, ViewButton):
+                    self.add_button(item)
+                elif isinstance(item, ViewSelect.GoTo):
+                    self.add_go_to_select(item)
+            await self._msg.edit(view=self.__view)
+    
+    def remove_button(self, button: ViewButton) -> None:
+        """Remove a button from the menu
+        
+        Parameters
+        ----------
+        button: :class:`ViewButton`
+            The button to remove
+        
+        Raises
+        ------
+        - `ButtonNotFound`: The provided button was not found in the list of buttons on the menu
+        """
+        if button in self.__buttons:
+            button._menu = None
+            self.__buttons.remove(button)
+            self.__view.remove_item(button)
+        else:
+            raise ButtonNotFound('Cannot remove a button that is not registered')
+    
+    def remove_all_buttons(self) -> None:
+        """Remove all buttons from the menu"""
+        # Set persists
+        persistent_link_buttons: List[ViewButton] = []
+        for btn in self.__buttons:
+            if self._should_persist(btn):
+                persistent_link_buttons.append(btn)
+                continue
+        else:
+            while self.__buttons:
+                self.remove_button(self.__buttons[0])
+            else:
+                for plb in persistent_link_buttons:
+                    self._bypass_primed = True
+                    self.add_button(plb)
+    
+    def disable_button(self, button: ViewButton) -> None:
+        """Disable a button on the menu
+        
+        Parameters
+        ----------
+        button: :class:`ViewButton`
+            The button to disable
+        
+        Raises
+        ------
+        - `ButtonNotFound`: The provided button was not found in the list of buttons on the menu
+        """
+        if button in self.__buttons:
+            idx = self.__buttons.index(button)
+            self.__buttons[idx].disabled = True
+        else:
+            raise ButtonNotFound('Cannot disable a button that is not registered')
+    
+    def disable_all_buttons(self) -> None:
+        """Disable all buttons on the menu"""
+        for btn in self.__buttons:
+            if self._should_persist(btn): continue
+            btn.disabled = True
+    
+    def enable_button(self, button: ViewButton) -> None:
+        """Enable the specified button
+        
+        Parameters
+        ----------
+        button: :class:`ViewButton`
+            The button to enable
+        
+        Raises
+        ------
+        - `ButtonNotFound`: The provided button was not found in the list of buttons on the menu
+        """
+        if button in self.__buttons:
+            idx = self.__buttons.index(button)
+            self.__buttons[idx].disabled = False
+        else:
+            raise ButtonNotFound('Cannot enable a button that is not registered')
+    
+    def enable_all_buttons(self) -> None:
+        """Enable all buttons on the menu"""
+        for btn in self.__buttons:
+            btn.disabled = False
+    
+    def _button_add_check(self, button: ViewButton) -> None:
+        """A set of checks to ensure the proper button is being added"""
+        # ensure they are using only the ViewButton and not ReactionMenus :class:`ReactionButton`
+        if isinstance(button, ViewButton):
+
+            # ensure the button custom_id is a valid one, but skip this check if its a link button because they dont have custom_ids
+            if button.style == discord.ButtonStyle.link:
+                pass
+            else:
+                # Note: this needs to be an re search because of buttons with an ID of "[ID]_[unique ID]"
+                if not re.search(ViewButton._RE_IDs, button.custom_id): # type: ignore
+                    raise ViewMenuException(f'ViewButton custom_id {button.custom_id!r} was not recognized')
+            
+            # ensure there are no duplicate custom_ids for the base navigation buttons
+            # Note: there's no need to have a check for buttons that are not navigation buttons because they have a unique ID and duplicates of those are allowed
+            active_button_ids: List[str] = [btn.custom_id for btn in self.__buttons] # type: ignore
+            if button.custom_id in active_button_ids:
+                if not all([button.custom_id is None, button.style == discord.ButtonStyle.link]):
+                    name = ViewButton._get_id_name_from_id(button.custom_id)
+                    raise ViewMenuException(f'A ViewButton with custom_id {name!r} has already been added')
+            
+            # if the menu_type is TypeText, disallow custom embed buttons
+            if button.style != discord.ButtonStyle.link and self._menu_type == ViewMenu.TypeText:
+                if button.custom_id == ViewButton.ID_CUSTOM_EMBED:
+                    if button.followup and button.followup.embed is not None:
+                        raise MenuSettingsMismatch('ViewButton with custom_id ViewButton.ID_CUSTOM_EMBED cannot be used when the menu_type is ViewMenu.TypeText')
+            
+            # if using a skip button, ensure the skip attribute was set
+            if button.custom_id == ViewButton.ID_SKIP and button.skip is None:
+                raise ViewMenuException('When attempting to add a button custom_id ViewButton.ID_SKIP, the "skip" kwarg was not set')
+            
+            # ensure there are no more than 25 buttons
+            if len(self.__buttons) >= 25:
+                raise TooManyButtons('ViewMenu cannot have more than 25 buttons (discord limitation)')
+        else:
+            raise IncorrectType(f'When adding a button to the ViewMenu, the button type must be ViewButton, got {button.__class__.__name__}')
+    
+    def _maybe_unique_id(self, button: ViewButton) -> None:
+        """Create a unique ID if the `custom_id` for buttons that are allowed to have duplicates
+        
+            Note ::
+                This excludes link buttons because they don't have a `custom_id`
+        """
+        if button.custom_id in (ViewButton.ID_CALLER, ViewButton.ID_SEND_MESSAGE, ViewButton.ID_CUSTOM_EMBED, ViewButton.ID_SKIP):
+            button.custom_id = f'{button.custom_id}_{id(button)}'
+    
+    @ensure_not_primed
+    def add_button(self, button: ViewButton) -> None:
+        """Add a button to the menu
+        
+        Parameters
+        ----------
+        button: :class:`ViewButton`
+            The button to add
+        
+        Raises
+        ------
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        - `MenuSettingsMismatch`: The buttons custom_id was set as :attr:`ViewButton.ID_CUSTOM_EMBED` but the `menu_type` is :attr:`ViewMenu.TypeText`
+        - `ViewMenuException`: The custom_id for the button was not recognized or a button with that custom_id has already been added
+        - `TooManyButtons`: There are already 25 buttons on the menu
+        - `IncorrectType`: Parameter :param:`button` was not of type :class:`ViewButton`
+        """
+        self._button_add_check(button)
+        self._maybe_unique_id(button)
+
+        button._menu = self
+        self.__view.add_item(button)
+        self.__buttons.append(button)
+    
+    @ensure_not_primed
+    def add_buttons(self, buttons: Sequence[ViewButton]) -> None:
+        """Add multiple buttons to the menu at once
+        
+        Parameters
+        ----------
+        buttons: Sequence[:class:`ViewButton`]
+            The buttons to add
+        
+        Raises
+        ------
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        - `MenuSettingsMismatch`: One of the buttons `custom_id` was set as :attr:`ViewButton.ID_CUSTOM_EMBED` but the `menu_type` is :attr:`ViewMenu.TypeText`
+        - `ViewMenuException`: The `custom_id` for a button was not recognized or a button with that `custom_id` has already been added
+        - `TooManyButtons`: There are already 25 buttons on the menu
+        - `IncorrectType`: One or more values supplied in parameter :param:`buttons` was not of type :class:`ViewButton`
+        """
+        for btn in buttons:
+            self.add_button(btn)
+    
+    def get_button(self, identity: str, *, search_by: Literal['label', 'id', 'name']='label') -> List[ViewButton]:
+        """Get a button that has been registered to the menu by it's label, custom_id, or name
+        
+        Parameters
+        ----------
+        identity: :class:`str`
+            The button label, custom_id, or name
+        
+        search_by: :class:`str`
+            How to search for the button. If "label", it's searched by button labels. If "id", it's searched by it's custom_id. 
+            If "name", it's searched by button names
+        
+        Returns
+        -------
+        List[:class:`ViewButton`]: The button(s) matching the given identity
+        
+        Raises
+        ------
+        - `ViewMenuException`: Parameter :param:`search_by` was not "label", "id", or "name"
+        """
+        identity = str(identity)
+        search_by = str(search_by).lower() # type: ignore
+
+        if search_by == 'label':
+            matched_labels: List[ViewButton] = [btn for btn in self.__buttons if btn.label and btn.label == identity]
+            return matched_labels
+        
+        elif search_by == 'id':
+            matched_ids: List[ViewButton] = [btn for btn in self.__buttons if btn.custom_id and btn.custom_id.startswith(identity)]
+            return matched_ids
+        
+        elif search_by == 'name':
+            matched_names: List[ViewButton] = [btn for btn in self.__buttons if btn.name and btn.name == identity]
+            return matched_names
+        
+        else:
+            raise ViewMenuException(f'Parameter "search_by" expected "label", "id", or "name", got {search_by!r}')
+
+    async def _paginate(self, button: ViewButton, inter: discord.Interaction) -> None:
+        """|coro| When the button is pressed, handle the pagination process"""
+        if not self._check(inter):
+            await inter.response.defer()
+            return
+        
+        button._update_statistics(inter.user)
+        await self._handle_event(button)
+        
+        if button.custom_id == ViewButton.ID_PREVIOUS_PAGE:
+            await inter.response.edit_message(**self._determine_kwargs(self._pc.prev()))
+        
+        elif button.custom_id == ViewButton.ID_NEXT_PAGE:
+            await inter.response.edit_message(**self._determine_kwargs(self._pc.next()))
+        
+        elif button.custom_id == ViewButton.ID_GO_TO_FIRST_PAGE:
+            await inter.response.edit_message(**self._determine_kwargs(self._pc.first_page()))
+        
+        elif button.custom_id == ViewButton.ID_GO_TO_LAST_PAGE:
+            await inter.response.edit_message(**self._determine_kwargs(self._pc.last_page()))
+        
+        elif button.custom_id == ViewButton.ID_GO_TO_PAGE:
+            await inter.response.defer()
+            prompt: discord.Message = await self._msg.channel.send(f'{inter.user.display_name}, what page would you like to go to?') # type: ignore / `.channel` is know at this point
+            try:
+                selection_message: discord.Message = await inter.client.wait_for('message', check=lambda m: all([m.channel.id == self._msg.channel.id, m.author.id == inter.user.id]), timeout=self.timeout) # type: ignore / `.channel` is know at this point
+                page = int(selection_message.content)
+            except (asyncio.TimeoutError, ValueError):
+                return
+            else:
+                if 1 <= page <= len(self._pages):
+                    self._pc.index = page - 1
+                    await self._msg.edit(**self._determine_kwargs(self._pc.current_page))
+                    if self.delete_interactions:
+                        await prompt.delete()
+                        await selection_message.delete()
+        
+        elif button.custom_id == ViewButton.ID_END_SESSION:
+            await self.stop(delete_menu_message=True)
+        
+        else:
+            #* NOTE: Link buttons, aka buttons with a `custom_id` of `None` do not send interactions, so there's no need for an if check
+
+            if button.custom_id.startswith(ViewButton.ID_CALLER): # type: ignore
+                if button.followup is None or button.followup.details is None:
+                    error_msg = 'ViewButton custom_id was set as ViewButton.ID_CALLER but the "followup" kwarg for that ViewButton was not set ' \
+                                'or method ViewButton.Followup.set_caller_details(..) was not called to set the caller information'
+                    raise ViewMenuException(error_msg)
+                
+                func = button.followup.details.func
+                args = button.followup.details.args
+                kwargs = button.followup.details.kwargs
+
+                # reply now because we don't know how long the users function will take to execute
+                await inter.response.defer()
+
+                try:
+                    if asyncio.iscoroutinefunction(func): await func(*args, **kwargs) # type: ignore / `func` is already confirmed to be a coroutine
+                    else: func(*args, **kwargs)
+                except Exception as err:
+                    call_failed_error_msg = inspect.cleandoc(
+                        f"""
+                        The button with custom_id ViewButton.ID_CALLER with the label "{button.label}" raised an error during it's execution
+                        -> {err.__class__.__name__}: {err}
+                        """
+                    )
+                    raise ViewMenuException(call_failed_error_msg)
+                else:
+                    if button.followup:
+                        # if this executes, the user doesn't want to respond with a message, only with the caller function (already called ^)
+                        if all((button.followup.content is None, button.followup.embed is None, button.followup.file is None)):
+                            pass
+                        else:
+                            followup_kwargs = button.followup._to_dict()
+
+                            # inter.followup() has no attribute delete_after/details, so manually delete the key/val pairs to avoid :exc:`TypeError`, got an unexpected kwarg
+                            del followup_kwargs['delete_after']
+                            del followup_kwargs['details']
+                            
+                            # if there's no file, remove it to avoid an NoneType error
+                            if followup_kwargs['file'] is None:
+                                del followup_kwargs['file']
+                            
+                            followup_message: discord.WebhookMessage = await inter.followup.send(**followup_kwargs)
+                            
+                            if button.followup.delete_after:
+                                await followup_message.delete(delay=button.followup.delete_after)
+            
+            elif button.custom_id.startswith(ViewButton.ID_SEND_MESSAGE): # type: ignore
+                if button.followup is None:
+                    raise ViewMenuException('ViewButton custom_id was set as ViewButton.ID_SEND_MESSAGE but the "followup" kwarg for that ViewButton was not set')
+                
+                # there must be at least 1. cannot send an empty message
+                if all((button.followup.content is None, button.followup.embed is None, button.followup.file is None)):
+                    raise ViewMenuException('When using a ViewButton with a custom_id of ViewButton.ID_SEND_MESSAGE, the followup message cannot be empty')
+                
+                followup_kwargs = button.followup._to_dict()
+
+                # inter.followup.send() has no kwarg "details"
+                del followup_kwargs['details']
+                
+                # files are ignored
+                del followup_kwargs['file']
+                
+                # inter.followup.send() has no kwarg "delete_after"
+                del followup_kwargs['delete_after']
+
+                # defer instead of inter.response.send_message() so `delete_after` and `allowed_mentions` can be used
+                # inter.followup.send() is used instead
+                await inter.response.defer()
+
+                sent_message: discord.WebhookMessage = await inter.followup.send(**followup_kwargs)
+                if button.followup.delete_after:
+                    await sent_message.delete(delay=button.followup.delete_after)
+            
+            elif button.custom_id.startswith(ViewButton.ID_CUSTOM_EMBED): # type: ignore
+                if self._menu_type not in (ViewMenu.TypeEmbed, ViewMenu.TypeEmbedDynamic):
+                    raise ViewMenuException('Buttons with custom_id ViewButton.ID_CUSTOM_EMBED can only be used when the menu_type is ViewMenu.TypeEmbed or ViewMenu.TypeEmbedDynamic')
+                else:
+                    if button.followup is None or button.followup.embed is None:
+                        raise ViewMenuException('ViewButton custom_id was set as ViewButton.ID_CUSTOM_EMBED but the "followup" kwargs for that ViewButton was not set or the "embed" kwarg for the followup was not set')
+                   
+                    await inter.response.edit_message(embed=button.followup.embed)            
+            
+            elif button.custom_id.startswith(ViewButton.ID_SKIP): # type: ignore
+                await inter.response.edit_message(**self._determine_kwargs(self._pc.skip(button.skip)))
+            
+            else:
+                # this shouldn't execute because of :meth:`_button_add_check`, but just in case i missed something, raise the appropriate error
+                raise ViewMenuException(f'ViewButton custom_id {button.custom_id!r} was not recognized')
+
+        await self._contact_relay(inter.user, button)
+
+    async def stop(self, *, delete_menu_message: bool=False, disable_items: bool=False, remove_items: bool=False) -> None:
+        """|coro|
+        
+        Stops the process of the menu with the option of deleting the menu's message, removing the buttons, or disabling the buttons upon stop
+        
+        Parameters
+        ----------
+        delete_menu_message: :class:`bool`
+            Delete the message the menu is operating from
+
+        disable_items: :class:`bool`
+            Disable the buttons & selects on the menu
+        
+        remove_items: :class:`bool`
+            Remove the buttons & selects from the menu
+
+        Parameter Hierarchy
+        -------------------
+        Only one option is available when stopping the menu. If you have multiple parameters as `True`, only one will execute
+        - `disable_items` > `remove_items`
+
+        Raises
+        ------
+        - `discord.DiscordException`: Any exception that can be raised when deleting or editing a message
+        """
+        if self._is_running:
+            self._stop_initiated = True
+            try:
+                if delete_menu_message:
+                    await self._msg.delete()
+                else:
+                    already_disabled = False
+                    if disable_items:
+                        self.disable_all_buttons()
+                        self.disable_all_selects()
+                        self.disable_all_go_to_selects()
+                        already_disabled = True
+                        await self._msg.edit(view=self.__view)
+                    
+                    if remove_items and not already_disabled:
+                        self.remove_all_buttons()
+                        self.remove_all_selects()
+                        self.remove_all_go_to_selects()
+                        await self._msg.edit(view=self.__view)
+            
+            except discord.DiscordException as dpy_error:
+                raise dpy_error
+            
+            finally:
+                self.__view.stop()
+                self._is_running = False
+
+                if self in ViewMenu._active_sessions:
+                    ViewMenu._active_sessions.remove(self)
+                
+                self._on_close_event.set()
+                await self._handle_on_timeout()
+    
+    def _override_dm_settings(self) -> None:
+        """If a menu session is in a direct message the following settings are disabled/changed because of discord limitations and resource/safety reasons
+        
+            .. added:: v3.1.0
+        """
+        if self.in_dms:
+            # Can't delete someone else's message in DMs
+            if self.delete_interactions:
+                self.delete_interactions = False
+            
+            # There are no roles in DMs
+            if self.only_roles:
+                self.only_roles = None
+            
+            # No point in having an *indefinite* menu in DMs
+            if self.timeout is None:
+                self.timeout = 60.0
+    
+    def __generate_viewmenu_payload(self) -> dict:
+        """Creates the parameters needed for :meth:`discord.Messageable.send()`
+        
+            .. added:: v3.1.0
+        """
+        return {
+            "content" : self._pages[0].content if self._pages else None,
+            "embed" : self._pages[0].embed if self._pages else discord.utils.MISSING,
+            "files" : self._pages[0].files if self._pages else discord.utils.MISSING,
+            "view" : self.__view,
+            "allowed_mentions" : self.allowed_mentions
+        }
+    
+    def __refresh_select_pages(self, menu_type: MenuType) -> None:
+        if self.__selects:
+            for vm_select in self.__selects:
+                for pages in vm_select._view_select_options.values():
+                    self._refresh_page_director_info(menu_type, pages)
+
+    @overload
+    async def start(self, *, send_to: Optional[str]=None, reply: bool=False) -> None:
+        ...
+    
+    @overload
+    async def start(self, *, send_to: Optional[int]=None, reply: bool=False) -> None:
+        ...
+    
+    @overload
+    async def start(self, *, send_to: Optional[discord.TextChannel]=None, reply: bool=False) -> None:
+        ...
+    
+    @overload
+    async def start(self, *, send_to: Optional[discord.VoiceChannel]=None, reply: bool=False) -> None:
+        ...
+    
+    @overload
+    async def start(self, *, send_to: Optional[discord.Thread]=None, reply: bool=False) -> None:
+        ...
+    
+    @ensure_not_primed
+    async def start(self, *, send_to: Optional[Union[str, int, discord.TextChannel, discord.VoiceChannel, discord.Thread]]=None, reply: bool=False) -> None:
+        """|coro|
+        
+        Start the menu
+        
+        Parameters
+        ----------
+        send_to: Optional[Union[:class:`str`, :class:`int`, :class:`discord.TextChannel`, :class:`discord.VoiceChannel`, :class:`discord.Thread`]]
+			The channel/thread you'd like the menu to start in. Use the channel/threads name, ID, or it's object. Please note that if you intend to use a channel/thread object, using
+			method :meth:`discord.Client.get_channel()` (or any other related methods), that channel should be in the same list as if you were to use `ctx.guild.text_channels`
+			or `ctx.guild.threads`. This only works on a context guild channel basis. That means a menu instance cannot be created in one guild and the menu itself (:param:`send_to`)
+			be sent to another. Whichever guild context the menu was instantiated in, the channels/threads of that guild are the only options for :param:`send_to`
+
+            Note: This parameter is not available if your `method` is a :class:`discord.Interaction`, aka a slash command
+        
+        reply: :class:`bool`
+            Enables the menu message to reply to the message that triggered it. Parameter :param:`send_to` must be :class:`None` if this is `True`. This only pertains to a non-interaction based menu.
+        
+        Raises
+        ------
+        - `MenuAlreadyRunning`: Attempted to call method after the menu has already started
+        - `NoPages`: The menu was started when no pages have been added
+        - `NoButtons`: Attempted to start the menu when no Buttons have been registered
+        - `ViewMenuException`: The :class:`ViewMenu`'s `menu_type` was not recognized. There were more than one base navigation buttons. Or a :attr:`ViewButton.ID_CUSTOM_EMBED` button was not correctly formatted
+        - `DescriptionOversized`: When using a `menu_type` of :attr:`ViewMenu.TypeEmbedDynamic`, the embed description was over discords size limit
+        - `IncorrectType`: Parameter :param:`send_to` was not of the expected type
+        - `MenuException`: The channel set in :param:`send_to` was not found
+        """
+        if ViewMenu._sessions_limit_details.set_by_user:
+            can_proceed = await self._handle_session_limits()
+            if not can_proceed:
+                return
+        
+        self._override_dm_settings()
+        
+        # checks
+        # Note 1: each at least 1 page check is done in it's own if statement to avoid clashing between pages and custom embeds
+        # Note 2: at least 1 page check for add_row is done in "(dynamic menu)"
+        
+        # ensure at least 1 button exists before starting the menu
+        if not self.__buttons: raise NoButtons
+        if self._menu_type not in ViewMenu._all_menu_types(): raise ViewMenuException('ViewMenu menu_type not recognized')
+
+        reply_kwargs = self._handle_reply_kwargs(send_to, reply)
+        menu_payload = self.__generate_viewmenu_payload()
+        
+        if isinstance(self._method, Context):
+            menu_payload.update(reply_kwargs)
+
+        # add page (normal menu)
+        if self._menu_type == ViewMenu.TypeEmbed:
+            self._refresh_page_director_info(ViewMenu.TypeEmbed, self._pages)
+
+            navigation_btns = [btn for btn in self.__buttons if btn.custom_id in ViewButton._base_nav_buttons()]
+
+            # an re search is required here because buttons with ID_CUSTOM_EMBED dont have a normal ID, the ID is "8_[unique ID]"
+            custom_embed_btns = [btn for btn in self.__buttons if btn.style != discord.ButtonStyle.link and re.search(r'8_\d+', btn.custom_id)] # type: ignore / raw string is compatible
+
+            if all([not self._pages, not custom_embed_btns]):
+                raise NoPages
+
+            # normal pages, no custom embeds
+            if self._pages and not custom_embed_btns:
+                await self._handle_send_to(send_to, menu_payload)
+            
+            # only custom embeds
+            elif not self._pages and custom_embed_btns:
+                # since there are only custom embeds, there is no need for base navigation buttons, so remove them if any
+                for nav_btn in navigation_btns:
+                    if nav_btn in self.__buttons:
+                        self.__buttons.remove(nav_btn)
+                
+                # ensure all custom embed buttons have the proper values set
+                for custom_btn in custom_embed_btns:
+                    if custom_btn.followup is None or custom_btn.followup.embed is None:
+                        raise ViewMenuException('ViewButton custom_id was set as ViewButton.ID_CUSTOM_EMBED but the "followup" kwargs for that ViewButton was not set or the "embed" kwarg for the followup was not set')
+                
+                # since there are only custom embeds, self._pages is still set to :class:`None`, so set the embed in `.send()` to the first custom embed in the list
+                menu_payload['embed'] = custom_embed_btns[0].followup.embed # type: ignore
+                await self._handle_send_to(send_to, menu_payload)
+            
+            # normal pages and custom embeds
+            else:
+                # since there are custom embeds, ensure there is at least one base navigation button so they can switch between the normal pages and custom embeds
+                if not navigation_btns:
+                    error_msg = inspect.cleandoc(
+                        """
+                        Since you've added pages and custom embeds, there needs to be at least one base navigation button. Without one, there's no way to go back to the normal pages in the menu if a custom embed button is pressed.
+                        The available base navigation buttons are buttons with the custom_id:
+                        - ViewButton.ID_PREVIOUS_PAGE
+                        - ViewButton.ID_NEXT_PAGE
+                        - ViewButton.ID_GO_TO_FIRST_PAGE
+                        - ViewButton.ID_GO_TO_LAST_PAGE
+                        - ViewButton.ID_GO_TO_PAGE
+                        """
+                    )
+                    raise ViewMenuException(error_msg)
+                else:
+                    await self._handle_send_to(send_to, menu_payload)
+            
+            self.__refresh_select_pages(ViewMenu.TypeEmbed)
+
+        # add row (dynamic menu)
+        elif self._menu_type == ViewMenu.TypeEmbedDynamic:
+            await self._build_dynamic_pages(send_to, view=self.__view, payload=menu_payload)
+        
+        # add page (text menu)
+        else:
+            if not self._pages:
+                raise NoPages
+            
+            self._refresh_page_director_info(ViewMenu.TypeText, self._pages)
+            menu_payload['content'] = self._pages[0].content # reassign the first page to show to director information
+            await self._handle_send_to(send_to, menu_payload)
+        
+        self._pc = _PageController(self._pages)
+        self._is_running = True
+        ViewMenu._active_sessions.append(self)
```

### Comparing `reactionmenu-3.1.3/reactionmenu.egg-info/PKG-INFO` & `reactionmenu-3.1.4/reactionmenu.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,1015 +1,1015 @@
-Metadata-Version: 2.1
-Name: reactionmenu
-Version: 3.1.3
-Summary: A library to create a discord.py 2.0+ paginator. Supports pagination with buttons, reactions, and category selection using selects.
-Author: Defxult#8269
-License: MIT
-Project-URL: Homepage, https://github.com/Defxult/reactionmenu
-Project-URL: Changelog, https://github.com/Defxult/reactionmenu/blob/main/CHANGELOG.md
-Keywords: buttons,buttons paginator,buttons menu,discord,discord.py,discord.py 2.0,d.py,components,components paginator,components menu,discord components,discord components menu,discord buttons,discord buttons paginator,discord buttons menu,discord paginator,discord pagination,discord reaction menu,discord reactions,discord embed,discord menu,discord interactions,embed menu,embed reaction menu,embed paginator,interactions,interactions menu,interactions paginator,menus,paginator,pagination,pagination menu,reaction menu
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![logo](https://cdn.discordapp.com/attachments/655186216060321816/820162226316378162/discord.jpg)
-<div align="center">
-
-[![Downloads](https://pepy.tech/badge/reactionmenu)](https://pepy.tech/project/reactionmenu) 
-[![Downloads](https://pepy.tech/badge/reactionmenu/month)](https://pepy.tech/project/reactionmenu)
-[![Downloads](https://pepy.tech/badge/reactionmenu/week)](https://pepy.tech/project/reactionmenu)
-
-![python_version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
-</div>
-
-## How to install
-You can install the latest [PyPI](https://pypi.org/project/reactionmenu/) version of the library by doing:
-```
-$ pip install reactionmenu
-```
-Or the development version:
-```
-$ pip install git+https://github.com/Defxult/reactionmenu
-```
-
-## Intents
-Minimum intents needed
-```py
-bot = commands.Bot(..., intents=discord.Intents(messages=True, guilds=True, reactions=True, members=True))
-```
----
-## ReactionMenu
-
-```
-class reactionmenu.ReactionMenu(method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs)
-```
-
-A `ReactionMenu` is a menu that uses emojis which are either custom guild emojis or a normal emoji to control the pagination process. If you're not looking for any of the fancy features and just want something simple, this is the one to use.
-
-![showcase](https://cdn.discordapp.com/attachments/655186216060321816/819885696176226314/showcase.gif)
-
-<details>
-  <summary><b>Click to show ReactionMenu documentation</b></summary>
-
-### How to import
-```py
-from reactionmenu import ReactionMenu, ReactionButton
-```
-This library comes with several methods and options in order to make a discord reaction menu simple. Once you have imported the proper classes, you will initialize the constructor like so:
-```py
-menu = ReactionMenu(method, menu_type=ReactionMenu.TypeEmbed)
-```
-
-
-### Parameters of the ReactionMenu constructor
-* `method` (`Union[discord.ext.commands.Context, discord.Interaction]`) A context or interaction object
-* `menu_type` (`MenuType`) The configuration of the menu
-  * `ReactionMenu.TypeEmbed`, a normal embed pagination menu
-  * `ReactionMenu.TypeEmbedDynamic`, an embed pagination menu with dynamic data
-  * `ReactionMenu.TypeText`, a text only pagination menu
-
-
-### Kwargs of the ReactionMenu constructor
-| Name | Type | Default Value | Used for | Info 
--------|------|---------------|----------|------
-| `wrap_in_codeblock` | `str` | `None` | `ReactionMenu.TypeEmbedDynamic` | The discord codeblock language identifier to wrap your data in. Example: `ReactionMenu(ctx, ..., wrap_in_codeblock='py')`
-| `custom_embed` | `discord.Embed` | `None` | `ReactionMenu.TypeEmbedDynamic` | Embed object to use when adding data with `ReactionMenu.add_row()`. Used for styling purposes
-| `delete_on_timeout` | `bool` | `False` | `All menu types` | Delete the menu when it times out
-| `clear_reactions_after` | `bool` | `True` | `All menu types` | delete all reactions after the menu times out
-| `navigation_speed` | `str` | `ReactionMenu.NORMAL` | `All menu types` | Sets if the user needs to wait for the reaction to be removed by the bot before "turning" the page. Setting the speed to `ReactionMenu.FAST` makes it so that there is no need to wait (reactions are not removed on each press) and can navigate lengthy menu's more quickly
-| `only_roles` | `List[discord.Role]` | `None` | `All menu types` | If set, only members with any of the given roles are allowed to control the menu. The menu owner can always control the menu
-| `timeout` | `Union[int, float, None]` | `60.0` | `All menu types` | The timer for when the menu times out. Can be `None` for no timeout
-| `show_page_director` | `bool` | `True` | `All menu types` | Shown at the bottom of each embed page. "Page 1/20"
-| `name` | `str` | `None` | `All menu types` | A name you can set for the menu
-| `style` | `str` | `"Page $/&"` | `All menu types` | A custom page director style you can select. "$" represents the current page, "&" represents the total amount of pages. Example: `ReactionMenu(ctx, ..., style='On $ out of &')`
-| `all_can_click` | `bool` | `False` | `All menu types` | Sets if everyone is allowed to control when pages are 'turned' when buttons are clicked
-| `delete_interactions` | `bool` | `True` | `All menu types` | Delete the prompt message by the bot and response message by the user when asked what page they would like to go to when using `ReactionButton.Type.GO_TO_PAGE`
-| `rows_requested` | `int` | `None` | `ReactionMenu.TypeEmbedDynamic` | The amount of information per `ReactionMenu.add_row()` you would like applied to each embed page
-| `remove_extra_emojis` | `bool` | `False` | `All menu types` | If `True`, all emojis (reactions) added to the menu message that were not originally added to the menu will be removed
----
-
-### Pages for ReactionMenu
-Depending on the `menu_type`, pages can either be a `str`, `discord.Embed`, or a combination of `content` and `files` ([example below](#stacked-pages))
-* If the `menu_type` is `ReactionMenu.TypeEmbed`, use embeds
-* If the `menu_type` is `ReactionMenu.TypeText` (text only menu) or `ReactionMenu.TypeEmbedDynamic` (embed only menu), use strings.
-* Associated methods
-  * `ReactionMenu.add_page(embed: discord.Embed=MISSING, content: Optional[str]=None, files: Optional[Sequence[discord.File]]=None)`
-  * `ReactionMenu.add_pages(pages: Sequence[Union[discord.Embed, str]])`
-  * `ReactionMenu.add_row(data: str)`
-  * `ReactionMenu.remove_all_pages()`
-  * `ReactionMenu.clear_all_row_data()`
-  * `ReactionMenu.remove_page(page_number: int)`
-  * `ReactionMenu.set_main_pages(*embeds: Embed)`
-  * `ReactionMenu.set_last_pages(*embeds: Embed)`
-
-
-#### Adding Pages
-```py
-# ReactionMenu.TypeEmbed
-menu = ReactionMenu(method, menu_type=ReactionMenu.TypeEmbed)
-menu.add_page(summer_embed)
-menu.add_page(winter_embed)
-
-# ReactionMenu.TypeText
-menu = ReactionMenu(method, menu_type=ReactionMenu.TypeText)
-menu.add_page(content='Its so hot!')
-menu.add_page(content='Its so cold!')
-```
-
-#### ReactionMenu.TypeText
-A `TypeText` menu is a text based pagination menu. No embeds are involved in the pagination process, only plain text is used.
-
-![showcase-text](https://cdn.discordapp.com/attachments/655186216060321816/929172629947027466/text_showcase.gif)
-
-#### Stacked Pages
-With `v3.1.0+`, you can paginate with more than just an embed or text. You can combine text, embeds, as well as files. But depending on the `menu_type` the combination can be restricted. Here is an example of a menu with a `menu_type` of `TypeEmbed` that is stacked.
-
-```py
-# You can use regular commands as well
-@bot.tree.command(description="These are stacked pages", guild=discord.Object(id=...))
-async def stacked(interaction: discord.Interaction):
-    menu = ReactionMenu(interaction, menu_type=ReactionMenu.TypeEmbed)
-
-    menu.add_page(discord.Embed(title="My Embed"), content="This content is stacked on top of a file", files=[discord.File("stacked.py")])
-    menu.add_page(discord.Embed(title="Hey Wumpos, can you say hi to the person reading this? 😃"))
-    menu.add_page(discord.Embed(title="Hi, I'm Wumpos!"), files=[discord.File("wumpos.gif")])
-    
-    menu.add_button(ReactionButton.back())
-    menu.add_button(ReactionButton.next())
-    
-    await menu.start()
-```
-![stacked](https://cdn.discordapp.com/attachments/655186216060321816/955966821268332554/stacked.gif)
-
-Since the `menu_type` is `TypeEmbed`, there always has to be an embed on each page. If the `menu_type` was `TypeText`, embeds aren't allowed and you will be restricted to only using the `files` parameter.
-
-#### ReactionMenu.TypeEmbedDynamic
-A dynamic menu is used when you do not know how much information will be applied to the menu. For example, if you were to request information from a database, that information can always change. You query something and you might get 1,500 results back, and the next maybe only 800. A dynamic menu pieces all this information together for you and adds it to an embed page by rows of data. `ReactionMenu.add_row()` is best used in some sort of `Iterable` where everything can be looped through, but only add the amount of data you want to the menu page.
-> **NOTE:** In a dynamic menu, all added data is placed in the description section of an embed. If you choose to use a `custom_embed`, all text in the description will be overridden with the data you add
-* Associated methods
-    * `ReactionMenu.add_row(data: str)`
-    * `ReactionMenu.clear_all_row_data()`
-    * `ReactionMenu.set_main_pages(*embeds: Embed)`
-    * `ReactionMenu.set_last_pages(*embeds: Embed)`
-* The kwargs specifically made for a dynamic menu are:
-    * `rows_requested` - The amount of rows you would like on each embed page before making a new page
-        * `ReactionMenu(..., rows_requested=5)`
-    * `custom_embed` - An embed you have created to use as the embed pages. Used for your menu aesthetic
-        * `ReactionMenu(..., custom_embed=red_embed)`
-    * `wrap_in_codeblock` - The language identifier when wrapping your data in a discord codeblock. 
-        * `ReactionMenu(..., wrap_in_codeblock='py')`
-
-##### Adding Rows/data
-```py
-menu = ReactionMenu(ctx, menu_type=ReactionMenu.TypeEmbedDynamic, rows_requested=5)
-
-for data in database.request('SELECT * FROM customers'):
-    menu.add_row(data)
-```
-##### Deleting Data
-You can remove all the data you've added to a menu by using `menu.clear_all_row_data()`
-
-##### Main/Last Pages
-When using a dynamic menu, the only embed pages you see are from the data you've added. But if you would like to show more pages other than just the data, you can use methods `ReactionMenu.set_main_pages()` and `ReactionMenu.set_last_pages()`. Setting the main page(s), the embeds you set will be the first embeds that are shown when the menu starts. Setting the last page(s) are the last embeds shown
-```py
-menu.set_main_pages(welcome_embed, announcement_embed)
-
-for data in get_information():
-    menu.add_row(data)
-
-menu.set_last_pages(additional_info_embed)
-# NOTE: setting main/last pages can be set in any order
-```
-
-### ReactionButtons and ButtonTypes
-Buttons/button types are used when you want to add a reaction to the menu that does a certain function. Buttons and button types work together to achieve the desired action.
-```
-class reactionmenu.ReactionButton(*, emoji: str, linked_to: ButtonType, **kwargs)
-```
-### Parameters of the ReactionButton constructor
-* `emoji` (`str`) The emoji you would like to use as the reaction
-* `linked_to` (`ReactionButton.Type`) When the reaction is pressed, this is what determines what it will do
-
-### Kwargs of the ReactionButton constructor
-| Name | Type | Default Value | Used for
-|------|------|---------------|----------
-| `embed` | `discord.Embed` | `None` | When the reaction is pressed, go to the specified embed
-| `name` | `str` | `None` | The name of the button
-| `details` | [info below](#reactionbuttons-with-reactionbuttontypecaller) | `None` | Assigns the function and it's arguments to call when a `ReactionButton` with `ReactionButton.Type.CALLER` is pressed
-| `event` | `ReactionButton.Event` | `None` | Determine when a button should be removed depending on how many times it has been pressed
-| `skip` | `ReactionButton.Skip` | `None` | Set the action and the amount of pages to skip when using a `linked_to` of `ReactionButton.Type.SKIP`. For example using this button type, setting the action to "+" and the amount 3. If you are on "Page 1/20", pressing that button will bring you to "Page 4/20"
-
-### Attributes for ReactionButton
-| Property | Return Type | Info
-|----------|-------------|------
-| `clicked_by` | `Set[discord.Member]` | The members who clicked the button
-| `total_clicks` | `int` | Amount of clicks from the button
-| `last_clicked` | `Optional[datetime.datetime]` | The time in UTC for when the button was last clicked
-| `menu` | `Optional[ReactionMenu]` | The menu the button is attached to
-
-* Associated methods
-    * `ReactionMenu.add_button(button: ReactionButton)`
-    * `ReactionMenu.remove_all_buttons()`
-    * `ReactionMenu.remove_button(button: ReactionButton)`
-    * `ReactionMenu.get_button(identity: Union[str, int], *, search_by='name')`
-    * `ReactionButton.set_caller_details(func: Callable[..., None], *args, **kwargs)`
-
-
-### All ButtonTypes
-| Type | Info |
-|-------|------|
-| `ReactionButton.Type.NEXT_PAGE` | Go to the next page in the menu session
-| `ReactionButton.Type.PREVIOUS_PAGE` | Go to the previous page in the menu session
-| `ReactionButton.Type.GO_TO_FIRST_PAGE` | Go to the first page in the menu session
-| `ReactionButton.Type.GO_TO_LAST_PAGE` | Go to the last page in the menu session
-| `ReactionButton.Type.GO_TO_PAGE` | Prompts you to type in the page you'd like to go to
-| `ReactionButton.Type.END_SESSION` | Stops the session and deletes the menu message
-| `ReactionButton.Type.CUSTOM_EMBED` | Used separately from the navigation buttons. Once pressed, go to the specified embed 
-| `ReactionButton.Type.CALLER` | Used when specifying the function to call and it's arguments when the button is pressed
-| `ReactionButton.Type.SKIP` | Used to paginate through multiple pages in a single button press
-
-
-### Adding Buttons
-You can add buttons (reactions) to the menu using a `ReactionButton`. Below are examples on how to use each `ButtonType`. 
-> **NOTE:** ReactionButtons with `ReactionButton.Type.CALLER` are a little different, so there is a dedicated section explaining how they work and how to implement them further below
-
-```py
-menu = ReactionMenu(...)
-
-# first and last pages
-fpb = ReactionButton(emoji='⏪', linked_to=ReactionButton.Type.GO_TO_FIRST_PAGE)
-lpb = ReactionButton(emoji='⏩', linked_to=ReactionButton.Type.GO_TO_LAST_PAGE)
-
-# go to page
-gtpb = ReactionButton(emoji='🔢', linked_to=ReactionButton.Type.GO_TO_PAGE)
-
-# end session
-esb = ReactionButton(emoji='⏹️', linked_to=ReactionButton.Type.END_SESSION)
-
-# custom embed
-ceb = ReactionButton(emoji='😎', linked_to=ReactionButton.Type.CUSTOM_EMBED, embed=discord.Embed(title='Hello'))
-
-# skip button
-sb = ReactionButton(emoji='5️⃣', linked_to=ReactionButton.Type.SKIP, skip=ReactionButton.Skip(action='+', amount=5))
-
-menu.add_button(fpb)
-...
-```
-### Deleting Buttons
-Remove all buttons with `menu.remove_all_buttons()`. You can also remove an individual button using its name if you have it set, or the button object itself with `menu.remove_button()`
-
-### ReactionButtons with ReactionButton.Type.CALLER
-`ReactionButton.Type.CALLER` buttons are used to implement your own functionality into the menu. Maybe you want to add a button that creates a text channel, sends a message, or add something to a database, whatever it may be. In order to work with `ReactionButton.Type.CALLER`, use the class method below.
-
-* `ReactionButton.set_caller_details(func: Callable[..., None], *args, **kwargs)`
-  
-This class method is used to setup a function and it's arguments that are later called when the button is pressed. The `ReactionButton` constructor has the kwarg `details`, and that's what you'll use with `.set_caller_details()` to assign the values needed. Some examples are below on how to properly implement `ReactionButton.Type.CALLER`
-
-```py
-@bot.command()
-async def user(ctx, name, *, message):
-    await ctx.send(f"Hi {name}! {message}. We're glad you're here!")
-
-def car(year, make, model):
-    print(f"I have a {year} {make} {model}")
-
-ub = ReactionButton(emoji='👋', linked_to=ReactionButton.Type.CALLER, details=ReactionButton.set_caller_details(user, ctx, 'Defxult', message='Welcome to the server'))
-cb = ReactionButton(emoji='🚗', linked_to=ReactionButton.Type.CALLER, details=ReactionButton.set_caller_details(car, 2021, 'Ford', 'Mustang'))
-```
-> **NOTE:** The function you pass in should not return anything. Calling functions with `ReactionButton.Type.CALLER` does not store or handle anything returned by that function
----
-
-### ReactionButton Methods
-The `ReactionButton` class comes with a set factory methods (class methods) that returns a `ReactionButton` with parameters set according to their `linked_to`.
-
-* `ReactionButton.back()`
-  * `emoji`: "◀️"
-  * `linked_to`: `ReactionButton.Type.PREVIOUS_PAGE`
-* `ReactionButton.next()`
-	* `emoji`: "▶️"
-	* `linked_to`: `ReactionButton.Type.NEXT_PAGE`
-* `ReactionButton.go_to_first_page()`
-	* `emoji`: "⏪"
-	* `linked_to`: `ReactionButton.Type.GO_TO_FIRST_PAGE`
-* `ReactionButton.go_to_last_page()`
-	* `emoji`: "⏩"
-	* `linked_to`: `ReactionButton.Type.GO_TO_LAST_PAGE`
-* `ReactionButton.go_to_page()`
-	* `emoji`: "🔢"
-	* `linked_to`: `ReactionButton.Type.GO_TO_PAGE`
-* `ReactionButton.end_session()`
-	* `emoji`: "⏹️"
-	* `linked_to`: `ReactionButton.Type.END_SESSION`
-* `ReactionButton.all()`
-  * Returns a `list` of `ReactionButton` in the following order
-  * `.go_to_first_page()` `.back()` `.next()` `.go_to_last_page()` `.go_to_page()` `.end_session()`
-* `ReactionButton.generate_skip(emoji: str, action: str, amount: int)`
-  * `emoji`: `<emoji>`
-  * `linked_to`: `ReactionButton.Type.SKIP`
-  * `skip`: `ReactionButton.Skip(<action>, <amount>)`
-
----
-### Setting Limits
-If you'd like, you can limit the amount of reaction menus that can be active at the same time *per* "guild", "member", or "channel" 
-* Associated CLASS Methods
-    * `ReactionMenu.set_sessions_limit(limit: int, per='guild', message='Too many active menus. Wait for other menus to be finished.')` 
-    * `ReactionMenu.remove_limit()`
-
-Example:
-```py
-@bot.command()
-async def limit(ctx):
-    ReactionMenu.set_sessions_limit(3, per='member', message='Sessions are limited to 3 per member')
-```
-
-With the above example, only 3 menus can be active at once for each member, and if they try to create more before their other menu's are finished, they will get an error message saying "Sessions are limited to 3 per member".
-
-### ReactionButton Events
-You can set a `ReactionButton` to be removed when it has been pressed a certain amount of times
-
-```
-class ReactionButton.Event(event_type: str, value: int)
-```
-
-#### Parameters for ReactionButton.Event
-* `event_type` (`str`) The action to take. The only available option is "remove"
-* `value` (`int`) The amount set for the specified event. Must be >= 1. If value is <= 0, it is implicitly set to 1
-
-Example:
-```py
-menu = ReactionMenu(ctx, ...)
-
-# remove a button after 10 clicks
-button = ReactionButton(..., event=ReactionButton.Event('remove', 10))
-menu.add_button(button)
-```
-> **NOTE:** Not ideal for buttons with a `linked_to` of `ReactionButton.Type.END_SESSION`
----
-### ReactionMenu Relays
-Menu relays are functions that are called anytime a button that is apart of a menu is pressed. It is considered as an extension of a `ReactionButton` with a `linked_to` of `ReactionButton.Type.CALLER`. Unlike caller buttons which provides no details about the interactions on the menu, relays do.
-* Associated methods
-  * `ReactionMenu.set_relay(func: Callable[[NamedTuple], None], *, only: Optional[List[ReactionButton]]=None)`
-  * `ReactionMenu.remove_relay()`
-
-When creating a function for your relay, that function must contain a single positional argument. When a button is pressed, a `RelayPayload` object (a named tuple) is passed to that function. The attributes of `RelayPayload` are:
-* `member` (`discord.Member`) The person who pressed the button
-* `button` (`ReactionButton`) The button that was pressed
-
-Example:
-```py
-async def enter_giveaway(payload):
-    member = payload.member
-    channel = payload.button.menu.message.channel
-    await channel.send(f"{member.mention}, you've entered the giveaway!")
-
-menu = ReactionMenu(ctx, ...)
-menu.set_relay(enter_giveaway)
-```
-The `set_relay` method comes with the `only` parameter. If that parameter is `None`, all buttons that are pressed will be relayed. You can provide a `list` of buttons to that parameter so only button presses from those specified buttons will be relayed.
-```py
-def example(payload):
-    ...
-
-menu = ReactionMenu(ctx, ...)
-
-back_button = ReactionButton.back()
-next_button = ReactionButton.next()
-
-menu.set_relay(example, only=[back_button])
-```
-
----
-### Starting/Stopping the ReactionMenu
-* Associated methods
-  * `await ReactionMenu.start(*, send_to=None, reply=False)`
-  * `await ReactionMenu.stop(*, delete_menu_message=False, clear_reactions=False)`
-
-When starting the menu, you have the option to send the menu to a certain channel. Parameter `send_to` is the channel you'd like to send the menu to. You can set `send_to` as the channel name (`str`), channel ID (`int`), or channel object (`discord.TextChannel` / `discord.Thread`). Example:
-```py
-menu = ReactionMenu(...)
-# channel name
-await menu.start(send_to='bot-commands')
-
-# channel ID
-await menu.start(send_to=1234567890123456)
-
-# channel object
-channel = guild.get_channel(1234567890123456)
-await menu.start(send_to=channel)
-
-# there's no need to specify send_to unless you want the menu to be sent to a different channel
-# from the one you're sending the initial message/using the command in. the menu can be started
-# in the current channel by omitting the send_to parameter
-await menu.start()
-```
-> **NOTE:** `send_to` is not valid if a menu was started in DM's
-
-### Full Example
-Here is a basic implementation of `ReactionMenu` that you can copy & paste for a quick demonstration.
-```py
-import asyncio
-import discord
-from discord.ext import commands
-from reactionmenu import ReactionMenu, ReactionButton
-
-bot = commands.Bot(command_prefix='!', intents=discord.Intents.all())
-
-async def start_bot():
-    async with bot:
-        await bot.start('...')
-
-@bot.command()
-async def example(ctx):
-    menu = ReactionMenu(ctx, menu_type=ReactionMenu.TypeEmbed)
-    
-    for member in ctx.guild.members:
-        if member.avatar:
-            embed = discord.Embed(description=f'Joined {member.joined_at.strftime("%b. %d, %Y")}')
-            embed.set_author(name=member.name, icon_url=member.avatar.url)
-            menu.add_page(embed)
-    
-    menu.add_button(ReactionButton.back())
-    menu.add_button(ReactionButton.next())
-    menu.add_button(ReactionButton.end_session())
-    
-    await menu.start()
-
-asyncio.run(start_bot())
-```
-</details>
-
-
-
-
-
-
-
-
-
-
----
-
-
-
-
-
-
-
-
-
-
-## ViewMenu
-```
-class reactionmenu.ViewMenu(method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs)
-```
-
-A `ViewMenu` is a menu that uses discords Buttons feature. With buttons, you can enable and disable them, set a certain color for them with emojis, have buttons that send hidden messages, and add hyperlinks. This library offers a broader range of functionalities such as who pressed the button, how many times it was pressed and more. It uses views (`discord.ui.View`) to implement the Buttons functionality, but uses some of its own methods in order to make a Button pagination menu simple.
-
-![image](https://cdn.discordapp.com/attachments/655186216060321816/855818139450081280/buttons_showcase_reduced.gif)
-
-<details>
-  <summary><b>Click to show ViewMenu documentation</b></summary>
-
-
-### How to import
-```py
-from reactionmenu import ViewMenu, ViewButton
-```
----
-
-### Parameters of the ViewMenu constructor
-* `method` (`Union[discord.ext.commands.Context, discord.Interaction]`) A context or interaction object
-* `menu_type` (`MenuType`) The configuration of the menu
-  * `ViewMenu.TypeEmbed`, a normal embed pagination menu
-  * `ViewMenu.TypeEmbedDynamic`, an embed pagination menu with dynamic data
-  * `ViewMenu.TypeText`, a text only pagination menu
-
----
-### Kwargs of the ViewMenu constructor
-| Name | Type | Default Value | Used for | Info 
--------|------|---------------|----------|------
-| `wrap_in_codeblock` | `str` | `None` | `ViewMenu.TypeEmbedDynamic` | The discord codeblock language identifier to wrap your data in. Example: `ViewMenu(ctx, ..., wrap_in_codeblock='py')`
-| `custom_embed` | `discord.Embed` | `None` | `ViewMenu.TypeEmbedDynamic` | Embed object to use when adding data with `ViewMenu.add_row()`. Used for styling purposes
-| `delete_on_timeout` | `bool` | `False` | `All menu types` | Delete the menu when it times out
-| `disable_items_on_timeout` | `bool` | `True` | `All menu types` | Disable the items on the menu when the menu times out
-| `remove_items_on_timeout` | `bool` | `False` | `All menu types` | Remove the items on the menu when the menu times out
-| `only_roles` | `List[discord.Role]` | `None` | `All menu types` | If set, only members with any of the given roles are allowed to control the menu. The menu owner can always control the menu
-| `timeout` | `Union[int, float, None]` | `60.0` | `All menu types` | The timer for when the menu times out. Can be `None` for no timeout
-| `show_page_director` | `bool` | `True` | `All menu types` | Shown at the bottom of each embed page. "Page 1/20"
-| `name` | `str` | `None` | `All menu types` | A name you can set for the menu
-| `style` | `str` | `"Page $/&"` | `All menu types` | A custom page director style you can select. "$" represents the current page, "&" represents the total amount of pages. Example: `ViewMenu(ctx, ..., style='On $ out of &')`
-| `all_can_click` | `bool` | `False` | `All menu types` | Sets if everyone is allowed to control when pages are 'turned' when buttons are clicked
-| `delete_interactions` | `bool` | `True` | `All menu types` | Delete the prompt message by the bot and response message by the user when asked what page they would like to go to when using `ViewButton.ID_GO_TO_PAGE`
-| `rows_requested` | `int` | `None` | `ViewMenu.TypeEmbedDynamic` | The amount of information per `ViewMenu.add_row()` you would like applied to each embed page
----
-
-### Pages for ViewMenu
-Depending on the `menu_type`, pages can either be a `str`, `discord.Embed`, or a combination of `content` or `files` ([example below](#stacked-pages-1))
-* If the `menu_type` is `ViewMenu.TypeEmbed`, use embeds
-* If the `menu_type` is `ViewMenu.TypeText` (text only menu) or `ViewMenu.TypeEmbedDynamic` (embed only menu), use strings.
-* Associated methods
-  * `ViewMenu.add_page(embed: discord.Embed=MISSING, content: Optional[str]=None, files: Optional[Sequence[discord.File]]=None)`
-  * `ViewMenu.add_pages(pages: Sequence[Union[discord.Embed, str]])`
-  * `ViewMenu.add_row(data: str)`
-  * `ViewMenu.remove_all_pages()`
-  * `ViewMenu.clear_all_row_data()`
-  * `ViewMenu.remove_page(page_number: int)`
-  * `ViewMenu.set_main_pages(*embeds: Embed)`
-  * `ViewMenu.set_last_pages(*embeds: Embed)`
-
-#### Adding Pages
-```py
-# ViewMenu.TypeEmbed
-menu = ViewMenu(method, menu_type=ViewMenu.TypeEmbed)
-menu.add_page(summer_embed)
-menu.add_page(winter_embed)
-
-# ViewMenu.TypeText
-menu = ViewMenu(method, menu_type=ViewMenu.TypeText)
-menu.add_page(content='Its so hot!')
-menu.add_page(content='Its so cold!')
-```
-
-#### ViewMenu.TypeText
-A `TypeText` menu is a text based pagination menu. No embeds are involved in the pagination process, only plain text is used.
-
-![text_view_showcase](https://cdn.discordapp.com/attachments/655186216060321816/929744985656549386/text_view_showcase.gif)
-
-#### Stacked Pages
-With `v3.1.0+`, you can paginate with more than just an embed or text. You can combine text, embeds, as well as files. But depending on the `menu_type` the combination can be restricted. Here is an example of a menu with a `menu_type` of `TypeEmbed` that is stacked.
-
-```py
-# You can use regular commands as well
-@bot.tree.command(description="These are stacked pages", guild=discord.Object(id=...))
-async def stacked(interaction: discord.Interaction):
-    menu = ViewMenu(interaction, menu_type=ViewMenu.TypeEmbed)
-
-    menu.add_page(discord.Embed(title="My Embed"), content="This content is stacked on top of a file", files=[discord.File("stacked.py")])
-    menu.add_page(discord.Embed(title="Hey Wumpos, can you say hi to the person reading this? 😃"))
-    menu.add_page(discord.Embed(title="Hi, I'm Wumpos!"), files=[discord.File("wumpos.gif")])
-    
-    menu.add_button(ViewButton.back())
-    menu.add_button(ViewButton.next())
-    
-    await menu.start()
-```
-![stacked_view](https://cdn.discordapp.com/attachments/655186216060321816/955983620038860910/stacked_view.gif)
-
-Since the `menu_type` is `TypeEmbed`, there always has to be an embed on each page. If the `menu_type` was `TypeText`, embeds aren't allowed and you will be restricted to only using the `files` parameter.
-
-#### ViewMenu.TypeEmbedDynamic
-A dynamic menu is used when you do not know how much information will be applied to the menu. For example, if you were to request information from a database, that information can always change. You query something and you might get 1,500 results back, and the next maybe only 800. A dynamic menu pieces all this information together for you and adds it to an embed page by rows of data. `ViewMenu.add_row()` is best used in some sort of `Iterable` where everything can be looped through, but only add the amount of data you want to the menu page.
-> **NOTE:** In a dynamic menu, all added data is placed in the description section of an embed. If you choose to use a `custom_embed`, all text in the description will be overridden with the data you add
-* Associated methods
-    * `ViewMenu.add_row(data: str)`
-    * `ViewMenu.clear_all_row_data()`
-    * `ViewMenu.set_main_pages(*embeds: Embed)`
-    * `ViewMenu.set_last_pages(*embeds: Embed)`
-* The kwargs specifically made for a dynamic menu are:
-    * `rows_requested` - The amount of rows you would like on each embed page before making a new page
-        * `ViewMenu(..., rows_requested=5)`
-    * `custom_embed` - An embed you have created to use as the embed pages. Used for your menu aesthetic
-        * `ViewMenu(..., custom_embed=red_embed)`
-    * `wrap_in_codeblock` - The language identifier when wrapping your data in a discord codeblock. 
-        * `ViewMenu(..., wrap_in_codeblock='py')`
-
-##### Adding Rows/data
-```py
-menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbedDynamic, rows_requested=5)
-
-for data in database.request('SELECT * FROM customers'):
-    menu.add_row(data)
-```
-##### Deleting Data
-You can remove all the data you've added to a menu by using `menu.clear_all_row_data()`
-
-##### Main/Last Pages
-When using a dynamic menu, the only embed pages you see are from the data you've added. But if you would like to show more pages other than just the data, you can use methods `ViewMenu.set_main_pages()` and `ViewMenu.set_last_pages()`. Setting the main page(s), the embeds you set will be the first embeds that are shown when the menu starts. Setting the last page(s) are the last embeds shown
-```py
-menu.set_main_pages(welcome_embed, announcement_embed)
-
-for data in get_information():
-    menu.add_row(data)
-
-menu.set_last_pages(additional_info_embed)
-# NOTE: setting main/last pages can be set in any order
-```
-
-### Buttons for ViewMenu
-Buttons are what you use to interact with the menu. Unlike reactions, they look cleaner, provides less rate limit issues, and offer more in terms of interactions. Enable and disable buttons, use markdown hyperlinks in it's messages, and even send hidden messages.
-
-![discord_buttons](https://discord.com/assets/7bb017ce52cfd6575e21c058feb3883b.png)
-
-
-* Associated methods
-  * `ViewMenu.add_button(button: ViewButton)`
-  * `ViewMenu.disable_all_buttons()`
-  * `ViewMenu.disable_button(button: ViewButton)`
-  * `ViewMenu.enable_all_buttons()`
-  * `ViewMenu.enable_button(button: ViewButton)`
-  * `ViewMenu.get_button(identity: str, *, search_by='label')`
-  * `ViewMenu.remove_all_buttons()`
-  * `ViewMenu.remove_button(button: ViewButton)`
-  * `await ViewMenu.refresh_menu_items()`
-
-#### ViewButton
-```
-class reactionmenu.ViewButton(*, style=discord.ButtonStyle.secondary, label=None, disabled=False, custom_id=None, url=None, emoji=None, followup=None, event=None, **kwargs)
-```
-
-A `ViewButton` is a class that represents the discord button. It is a subclass of `discord.ui.Button`.
-
-The following are the rules set by Discord for Buttons:
-* Link buttons don't send interactions to the Discord App, so link button statistics (it's properties) are not tracked
-* Non-link buttons **must** have a `custom_id`, and cannot have a `url`
-* Link buttons **must** have a `url`, and cannot have a `custom_id`
-* There cannot be more than 25 buttons per message
----
-#### Parameters of the ViewButton constructor
-* `style` (`discord.ButtonStyle`) The button style
-* `label` (`str`) The text on the button
-* `custom_id` (`str`) An ID to determine what action that button should take. Available IDs:
-  * `ViewButton.ID_NEXT_PAGE`
-  * `ViewButton.ID_PREVIOUS_PAGE`
-  * `ViewButton.ID_GO_TO_FIRST_PAGE` 
-  * `ViewButton.ID_GO_TO_LAST_PAGE`
-  * `ViewButton.ID_GO_TO_PAGE`
-  * `ViewButton.ID_END_SESSION`
-  * `ViewButton.ID_CALLER`
-  * `ViewButton.ID_SEND_MESSAGE`
-  * `ViewButton.ID_CUSTOM_EMBED`
-  * `ViewButton.ID_SKIP`
-* `emoji` (`Union[str, discord.PartialEmoji]`) Emoji used for the button
-  * `ViewButton(..., emoji='😄')` 
-  * `ViewButton(..., emoji='<:miscTwitter:705423192818450453>')`
-  * `ViewButton(..., emoji='\U000027a1')`
-  * `ViewButton(..., emoji='\N{winking face}')`
-* `url` (`str`) URL for a button with style `discord.ButtonStyle.link`
-* `disabled` (`bool`) If the button should be disabled
-* `followup` (`ViewButton.Followup`) The message sent after the button is pressed. Only available for buttons that have a `custom_id` of `ViewButton.ID_CALLER` or `ViewButton.ID_SEND_MESSAGE`. `ViewButton.Followup` is a class that has parameters similar to `discord.abc.Messageable.send()`, and is used to control if a message is ephemeral, contains a file, embed, tts, etc...
-* `event` (`ViewButton.Event`) Set a button to be disabled or removed when it has been pressed a certain amount of times
-
-#### Kwargs of the ViewButton constructor
-| Name | Type | Default Value | Used for
-|------|------|---------------|----------
-| `name` | `str` | `None` | The name of the button
-| `skip` | `ViewButton.Skip` | `None` | Set the action and the amount of pages to skip when using a `custom_id` of `ViewButton.ID_SKIP`. For example, setting the action to "+" and the amount 3. If you are on "Page 1/20", pressing that button will bring you to "Page 4/20"
-| `persist` | `bool` | `False` | Prevents link buttons from being disabled/removed when the menu times out or is stopped so they can remain clickable
-
-#### Attributes for ViewButton
-| Property | Return Type | Info
-|----------|-------------|------
-| `clicked_by` | `Set[discord.Member]` | The members who clicked the button
-| `total_clicks` | `int` | Amount of clicks from the button
-| `last_clicked` | `Optional[datetime.datetime]` | The time in UTC for when the button was last clicked
-| `menu` | `Optional[ViewMenu]` | The menu the button is attached to
-
-#### Adding a ViewButton
-```py
-from reactionmenu import ViewMenu, ViewButton
-
-menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
-
-# Link button
-link_button = ViewButton(style=discord.ButtonStyle.link, emoji='🌍', label='Link to Google', url='https://google.com')
-menu.add_button(link_button)
-
-# Skip button
-skip = ViewButton(style=discord.ButtonStyle.primary, label='+5', custom_id=ViewButton.ID_SKIP, skip=ViewButton.Skip(action='+', amount=5))
-menu.add_button(skip)
-
-# ViewButton.ID_PREVIOUS_PAGE
-back_button = ViewButton(style=discord.ButtonStyle.primary, label='Back', custom_id=ViewButton.ID_PREVIOUS_PAGE)
-menu.add_button(back_button)
-
-# ViewButton.ID_NEXT_PAGE
-next_button = ViewButton(style=discord.ButtonStyle.secondary, label='Next', custom_id=ViewButton.ID_NEXT_PAGE)
-menu.add_button(next_button)
-
-# All other ViewButton are created the same way as the last 2 EXCEPT
-# 1 - ViewButton.ID_CALLER
-# 2 - ViewButton.ID_SEND_MESSAGE
-# 3 - ViewButton.ID_CUSTOM_EMBED
-
-
-# ViewButton.ID_CALLER
-def say_hello(name: str):
-    print('Hello', name)
-
-call_followup = ViewButton.Followup(details=ViewButton.Followup.set_caller_details(say_hello, 'John'))
-menu.add_button(ViewButton(label='Say hi', custom_id=ViewButton.ID_CALLER, followup=call_followup))
-
-# ViewButton.ID_SEND_MESSAGE
-msg_followup = ViewButton.Followup('This message is hidden!', ephemeral=True)
-menu.add_button(ViewButton(style=discord.ButtonStyle.green, label='Message', custom_id=ViewButton.ID_SEND_MESSAGE, followup=msg_followup))
-
-# ViewButton.ID_CUSTOM_EMBED
-custom_embed_button = ViewButton(style=discord.ButtonStyle.blurple, label='Social Media Info', custom_id=ViewButton.ID_CUSTOM_EMBED, followup=ViewButton.Followup(embed=discord.Embed(...)))
-```
----
-> **NOTE:** When it comes to buttons with a `custom_id` of `ViewButton.ID_CALLER`, `ViewButton.ID_SEND_MESSAGE`, `ViewButton.ID_CUSTOM_EMBED`, or link buttons, you can add as many as you'd like as long as in total it's 25 buttons or less. For all other button ID's, each menu can only have one.
-
-### Using Selects
-Selects are used when you'd like to categorize information in your menu. Selects can only be used when the menu's `menu_type` is `TypeEmbed`. You should keep in mind that discords limitations on how many menu UI items (rows) can be applied to each message.
-
-![select_showcase](https://cdn.discordapp.com/attachments/655186216060321816/971361708121653268/select_showcase.gif)
-
-* Associated Methods
-  * `ViewMenu.add_select(select: ViewSelect)`
-  * `ViewMenu.remove_select(select: ViewSelect)`
-  * `ViewMenu.remove_all_selects()`
-  * `ViewMenu.disable_select(select: ViewSelect)`
-  * `ViewMenu.disable_all_selects()`
-  * `ViewMenu.enable_select(select: ViewSelect)`
-  * `ViewMenu.enable_all_selects()`
-  * `ViewMenu.get_select(title: Union[str, None])`
-
-Example:
-```py
-from reactionmenu import ViewMenu, ViewSelect, Page
-
-menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
-menu.add_page(discord.Embed(title="A showcase of console video games", color=discord.Color.blurple()))
-
-menu.add_select(ViewSelect(title="Console Video Games", options={
-    discord.SelectOption(label="PlayStation", emoji="<:PlayStation:549638412538478602>") : [
-        Page(embed=discord.Embed(title="Ratchet & Clank", description=..., color=discord.Color.yellow()).set_image(url=...)),
-        Page(embed=discord.Embed(title="God of War", description=..., color=discord.Color.blue()).set_image(url=...))
-    ],
-    discord.SelectOption(label="Xbox", emoji="<:Xbox:501880493285834752>") : [
-        Page(embed=discord.Embed(title="Halo Infinite", description=..., color=discord.Color.green()).set_image(url=...)),
-        Page(embed=discord.Embed(title="Gears of War 4", description=..., color=discord.Color.red()).set_image(url=...))
-    ]
-}))
-
-menu.add_button(ViewButton.back())
-menu.add_button(ViewButton.next())
-await menu.start()
-```
-
-#### Go to page navigation
-You can use this type of select when you'd like to use the UI to select a page to go to.
-
-![goto_showcase](https://cdn.discordapp.com/attachments/655186216060321816/973629631905300501/Discord_6SP5AjoOOM.gif)
-
-* Associated methods
-  * `ViewMenu.add_go_to_select(goto: ViewSelect.GoTo)`
-  * `ViewMenu.enable_go_to_select(goto: ViewSelect.GoTo)`
-  * `ViewMenu.enable_all_go_to_selects()`
-  * `ViewMenu.disable_go_to_select(goto: ViewSelect.GoTo)`
-  * `ViewMenu.disable_all_go_to_selects()`
-  * `ViewMenu.remove_go_to_select(goto: ViewSelect.GoTo)`
-  * `ViewMenu.remove_all_go_to_selects()`
-
-The `page_numbers` parameter for `ViewSelect.GoTo` can be used with 3 different types
-
-1. `List[int]` If set to a list of integers, those specified values are the only options that are available when the select is clicked
-   1. `page_numbers=[1, 5, 10]`
-2. `Dict[int, Union[str, discord.Emoji, discord.PartialEmoji]]` You can use this type if you'd like to utilize emojis in your select
-   1. `page_numbers={1 : "🗯️", 2 : "📺"}`
-3. `ellipsis` You can set a *literal* ellipsis to have the library automatically assign all page numbers to the amount of pages that you've added to the menu. This can come in handy if you have 25 pages or less
-   1. `page_numbers=...`
-> **NOTE**: Setting the `page_numbers` parameter to an ellipsis (...) only works as intended if you've added the go to select AFTER you've added pages to the menu
-
-```py
-@bot.command()
-async def navigate(ctx):
-    menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
-
-    menu.add_page(discord.Embed(title="Twitter").set_image(url="..."))
-    menu.add_page(discord.Embed(title="YouTube").set_image(url="..."))
-    menu.add_page(discord.Embed(title="Discord").set_image(url="..."))
-    # ...
-    
-    menu.add_go_to_select(ViewSelect.GoTo(title="Go to page...", page_numbers=...))
-
-    menu.add_button(ViewButton.back())
-    menu.add_button(ViewButton.next())
-
-    await menu.start()
-```
-
-### Updating ViewButton and Pages
-* Associated methods
-  * `await ViewMenu.refresh_menu_items()`
-  * `await ViewMenu.update(*, new_pages: Union[List[Union[Embed, str]], None], new_buttons: Union[List[ViewButton], None])`
-
-When the menu is running, you can update the pages or buttons on the menu. Using `ViewMenu.update()`, you can replace the pages and buttons. Using `ViewMenu.refresh_menu_items()` updates the buttons you have changed.
-
-#### Updating a Button
-```py
-@bot.command()
-async def menu(ctx):
-    menu = ViewMenu(..., name='test')
-    link_button = ViewButton(..., label='Link')
-    
-    menu.add_button(link_button)
-    menu.add_page(...)
-
-    await menu.start()
-
-
-@bot.command()
-async def disable(ctx):
-    menu = ViewMenu.get_session('test')
-    link_button = menu[0].get_button('Link', search_by='label')
-    
-    menu.disable_button(link_button)
-    await menu.refresh_menu_items()
-```
-If the buttons are not refreshed with `ViewMenu.refresh_menu_items()`, the menu will not be updated when changing a button.
-
-#### Updating Pages and Buttons
-Method `ViewMenu.update(...)` is used when you want to replace all or a few of the buttons on the menu. 
-```py
-menu = ViewMenu(...)
-
-# in a different .command()
-await menu.update(new_pages=[hello_embed, goodbye_embed], new_buttons=[link_button, next_button])
-```
-
-> **NOTE**: When using `ViewMenu.update(...)`, there is no need to use `ViewMenu.refresh_menu_items()` because they are updated during the update call. 
-
----
-#### ViewButton Methods
-The `ViewButton` class comes with a set factory methods (class methods) that returns a `ViewButton` with parameters set according to their `custom_id` (excluding link buttons).
-
-* `ViewButton.link(label: str, url: str)`
-  * `style`: `discord.ButtonStyle.link`
-  * `label`: `<label>`
-  * `url`: `<url>`
-* `ViewButton.back()`
-  * `style`: `discord.ButtonStyle.gray`
-  * `label`: "Back"
-  * `custom_id`: `ViewButton.ID_PREVIOUS_PAGE`
-* `ViewButton.next()`
-	* `style`: `discord.ButtonStyle.gray`
-	* `label`: "Next"
-	* `custom_id`: `ViewButton.ID_NEXT_PAGE`
-* `ViewButton.go_to_first_page()`
-	* `style`: `discord.ButtonStyle.gray`
-	* `label`: "First Page"
-	* `custom_id`: `ViewButton.ID_GO_TO_FIRST_PAGE`
-* `ViewButton.go_to_last_page()`
-	* `style`: `discord.ButtonStyle.gray`
-	* `label`: "Last Page"
-	* `custom_id`: `ViewButton.ID_GO_TO_LAST_PAGE`
-* `ViewButton.go_to_page()`
-	* `style`: `discord.ButtonStyle.gray`
-	* `label`: "Page Selection"
-	* `custom_id`: `ViewButton.ID_GO_TO_PAGE`
-* `ViewButton.end_session()`
-	* style: `discord.ButtonStyle.gray`
-	* label: "Close"
-	* custom_id: `ViewButton.ID_END_SESSION`
-* `ViewButton.all()`
-  * Returns a `list` of `ViewButton` in the following order
-  * `.go_to_first_page()` `.back()` `.next()` `.go_to_last_page()` `.go_to_page()` `.end_session()`
-* `ViewButton.all_with_emojis()`
-  * Returns a `list` of `ViewButton` with their `emoji` parameters already set in the following order
-  * `.go_to_first_page()` `.back()` `.next()` `.go_to_last_page()` `.go_to_page()` `.end_session()`
-* `ViewButton.generate_skip(label: str, action: str, amount: int)`
-  * `style`: `discord.ButtonStyle.gray`
-  * `label`: `<label>`
-  * `custom_id`: `ViewButton.ID_SKIP`
-  * `skip`: `ViewButton.Skip(<action>, <amount>)`
-
-```py
-menu = ViewMenu(ctx, ...)
-menu.add_page(...)
-menu.add_page(...)
-
-menu.add_button(ViewButton.back())
-menu.add_button(ViewButton.next())
-
-await menu.start()
-```
----
-### ViewButton Events
-You can set a `ViewButton` to be disabled or removed when it has been pressed a certain amount of times
-
-```
-class ViewButton.Event(event_type: str, value: int)
-```
-
-#### Parameters for ViewButton.Event
-* `event_type` (`str`) The action to take. Can either be "disable" or "remove"
-* `value` (`int`) The amount set for the specified event. Must be >= 1. If value is <= 0, it is implicitly set to 1
-
-Example:
-```py
-menu = ViewMenu(ctx, ...)
-
-# disable a button after 5 clicks
-button_1 = ViewButton(..., event=ViewButton.Event('disable', 5))
-menu.add_button(button_1)
-
-# remove a button after 10 clicks
-button_2 = ViewButton(..., event=ViewButton.Event('remove', 10))
-menu.add_button(button_2)
-```
-> **NOTE:** Not valid for link buttons. Also not ideal for buttons with a `custom_id` of `ViewButton.ID_END_SESSION`
----
-### ViewMenu Relays
-Menu relays are functions that are called anytime a button that is apart of a menu is pressed. It is considered as an extension of a `ViewButton` with an ID of `ViewButton.ID_CALLER`. Unlike caller buttons which provides no details about the interactions on the menu, relays do.
-* Associated methods
-  * `ViewMenu.set_relay(func: Callable[[NamedTuple], None], *, only: Optional[List[ViewButton]]=None)`
-  * `ViewMenu.remove_relay()`
-
-When creating a function for your relay, that function must contain a single positional argument. When a button is pressed, a `RelayPayload` object (a named tuple) is passed to that function. The attributes of `RelayPayload` are:
-* `member` (`discord.Member`) The person who pressed the button
-* `button` (`ViewButton`) The button that was pressed
-
-Example:
-```py
-async def enter_giveaway(payload):
-    member = payload.member
-    channel = payload.button.menu.message.channel
-    await channel.send(f"{member.mention}, you've entered the giveaway!")
-
-menu = ViewMenu(ctx, ...)
-menu.set_relay(enter_giveaway)
-```
-The `set_relay` method comes with the `only` parameter. If that parameter is `None`, all buttons that are pressed will be relayed (except link buttons because they don't send interaction events). You can provide a `list` of buttons to that parameter so only button presses from those specified buttons will be relayed.
-```py
-def example(payload):
-    ...
-
-menu = ViewMenu(ctx, ...)
-
-back_button = ViewButton.back()
-next_button = ViewButton.next()
-
-menu.set_relay(example, only=[back_button])
-```
-
----
-### Starting/Stopping the ViewMenu
-* Associated methods
-  * `await ViewMenu.start(*, send_to=None, reply=False)`
-  * `await ViewMenu.stop(*, delete_menu_message=False, remove_buttons=False, disable_buttons=False)`
-
-When starting the menu, you have the option to send the menu to a certain channel. Parameter `send_to` is the channel you'd like to send the menu to. You can set `send_to` as the channel name (`str`), channel ID (`int`), or channel object (`discord.TextChannel` / `discord.Thread`). Example:
-```py
-menu = ViewMenu(...)
-# channel name
-await menu.start(send_to='bot-commands')
-
-# channel ID
-await menu.start(send_to=1234567890123456)
-
-# channel object
-channel = guild.get_channel(1234567890123456)
-await menu.start(send_to=channel)
-
-# there's no need to specify send_to unless you want the menu to be sent to a different channel
-# from the one you're sending the initial message/using the command in. the menu can be started
-# in the current channel by omitting the send_to parameter
-await menu.start()
-```
-> **NOTE:** `send_to` is not valid if a menu was started in DM's
-
-Only one option is available when stopping the menu. If you have multiple parameters as `True`, only one will execute
-- `delete_menu_message` > `disable_buttons`
-- `disable_buttons` > `remove_buttons`
----
-
-### Full Example
-Here is a basic implementation of `ViewMenu` that you can copy & paste for a quick demonstration.
-```py
-import asyncio
-import discord
-from discord.ext import commands
-from reactionmenu import ViewMenu, ViewButton
-
-bot = commands.Bot(command_prefix='!', intents=discord.Intents.all())
-
-async def start_bot():
-    async with bot:
-        await bot.start('...')
-
-@bot.command()
-async def example(ctx):
-    menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
-    
-    for member in ctx.guild.members:
-        if member.avatar:
-            embed = discord.Embed(description=f'Joined {member.joined_at.strftime("%b. %d, %Y")}')
-            embed.set_author(name=member.name, icon_url=member.avatar.url)
-            menu.add_page(embed)
-    
-    menu.add_button(ViewButton.back())
-    menu.add_button(ViewButton.next())
-    menu.add_button(ViewButton.end_session())
-    
-    await menu.start()
-
-asyncio.run(start_bot())
-```
-</details>
+Metadata-Version: 2.1
+Name: reactionmenu
+Version: 3.1.4
+Summary: A library to create a discord.py 2.0+ paginator. Supports pagination with buttons, reactions, and category selection using selects.
+Author: Defxult
+License: MIT
+Project-URL: Homepage, https://github.com/Defxult/reactionmenu
+Project-URL: Changelog, https://github.com/Defxult/reactionmenu/blob/main/CHANGELOG.md
+Keywords: buttons,buttons paginator,buttons menu,discord,discord.py,discord.py 2.0,d.py,components,components paginator,components menu,discord components,discord components menu,discord buttons,discord buttons paginator,discord buttons menu,discord paginator,discord pagination,discord reaction menu,discord reactions,discord embed,discord menu,discord interactions,embed menu,embed reaction menu,embed paginator,interactions,interactions menu,interactions paginator,menus,paginator,pagination,pagination menu,reaction menu
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![logo](https://cdn.discordapp.com/attachments/655186216060321816/820162226316378162/discord.jpg)
+<div align="center">
+
+[![Downloads](https://pepy.tech/badge/reactionmenu)](https://pepy.tech/project/reactionmenu) 
+[![Downloads](https://pepy.tech/badge/reactionmenu/month)](https://pepy.tech/project/reactionmenu)
+[![Downloads](https://pepy.tech/badge/reactionmenu/week)](https://pepy.tech/project/reactionmenu)
+
+![python_version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
+</div>
+
+## How to install
+You can install the latest [PyPI](https://pypi.org/project/reactionmenu/) version of the library by doing:
+```
+$ pip install reactionmenu
+```
+Or the development version:
+```
+$ pip install git+https://github.com/Defxult/reactionmenu
+```
+
+## Intents
+Minimum intents needed
+```py
+bot = commands.Bot(..., intents=discord.Intents(messages=True, guilds=True, reactions=True, members=True))
+```
+---
+## ReactionMenu
+
+```
+class reactionmenu.ReactionMenu(method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs)
+```
+
+A `ReactionMenu` is a menu that uses emojis which are either custom guild emojis or a normal emoji to control the pagination process. If you're not looking for any of the fancy features and just want something simple, this is the one to use.
+
+![showcase](https://cdn.discordapp.com/attachments/655186216060321816/819885696176226314/showcase.gif)
+
+<details>
+  <summary><b>Click to show ReactionMenu documentation</b></summary>
+
+### How to import
+```py
+from reactionmenu import ReactionMenu, ReactionButton
+```
+This library comes with several methods and options in order to make a discord reaction menu simple. Once you have imported the proper classes, you will initialize the constructor like so:
+```py
+menu = ReactionMenu(method, menu_type=ReactionMenu.TypeEmbed)
+```
+
+
+### Parameters of the ReactionMenu constructor
+* `method` (`Union[discord.ext.commands.Context, discord.Interaction]`) A context or interaction object
+* `menu_type` (`MenuType`) The configuration of the menu
+  * `ReactionMenu.TypeEmbed`, a normal embed pagination menu
+  * `ReactionMenu.TypeEmbedDynamic`, an embed pagination menu with dynamic data
+  * `ReactionMenu.TypeText`, a text only pagination menu
+
+
+### Kwargs of the ReactionMenu constructor
+| Name | Type | Default Value | Used for | Info 
+-------|------|---------------|----------|------
+| `wrap_in_codeblock` | `str` | `None` | `ReactionMenu.TypeEmbedDynamic` | The discord codeblock language identifier to wrap your data in. Example: `ReactionMenu(ctx, ..., wrap_in_codeblock='py')`
+| `custom_embed` | `discord.Embed` | `None` | `ReactionMenu.TypeEmbedDynamic` | Embed object to use when adding data with `ReactionMenu.add_row()`. Used for styling purposes
+| `delete_on_timeout` | `bool` | `False` | `All menu types` | Delete the menu when it times out
+| `clear_reactions_after` | `bool` | `True` | `All menu types` | delete all reactions after the menu times out
+| `navigation_speed` | `str` | `ReactionMenu.NORMAL` | `All menu types` | Sets if the user needs to wait for the reaction to be removed by the bot before "turning" the page. Setting the speed to `ReactionMenu.FAST` makes it so that there is no need to wait (reactions are not removed on each press) and can navigate lengthy menu's more quickly
+| `only_roles` | `List[discord.Role]` | `None` | `All menu types` | If set, only members with any of the given roles are allowed to control the menu. The menu owner can always control the menu
+| `timeout` | `Union[int, float, None]` | `60.0` | `All menu types` | The timer for when the menu times out. Can be `None` for no timeout
+| `show_page_director` | `bool` | `True` | `All menu types` | Shown at the bottom of each embed page. "Page 1/20"
+| `name` | `str` | `None` | `All menu types` | A name you can set for the menu
+| `style` | `str` | `"Page $/&"` | `All menu types` | A custom page director style you can select. "$" represents the current page, "&" represents the total amount of pages. Example: `ReactionMenu(ctx, ..., style='On $ out of &')`
+| `all_can_click` | `bool` | `False` | `All menu types` | Sets if everyone is allowed to control when pages are 'turned' when buttons are clicked
+| `delete_interactions` | `bool` | `True` | `All menu types` | Delete the prompt message by the bot and response message by the user when asked what page they would like to go to when using `ReactionButton.Type.GO_TO_PAGE`
+| `rows_requested` | `int` | `None` | `ReactionMenu.TypeEmbedDynamic` | The amount of information per `ReactionMenu.add_row()` you would like applied to each embed page
+| `remove_extra_emojis` | `bool` | `False` | `All menu types` | If `True`, all emojis (reactions) added to the menu message that were not originally added to the menu will be removed
+---
+
+### Pages for ReactionMenu
+Depending on the `menu_type`, pages can either be a `str`, `discord.Embed`, or a combination of `content` and `files` ([example below](#stacked-pages))
+* If the `menu_type` is `ReactionMenu.TypeEmbed`, use embeds
+* If the `menu_type` is `ReactionMenu.TypeText` (text only menu) or `ReactionMenu.TypeEmbedDynamic` (embed only menu), use strings.
+* Associated methods
+  * `ReactionMenu.add_page(embed: discord.Embed=MISSING, content: Optional[str]=None, files: Optional[Sequence[discord.File]]=None)`
+  * `ReactionMenu.add_pages(pages: Sequence[Union[discord.Embed, str]])`
+  * `ReactionMenu.add_row(data: str)`
+  * `ReactionMenu.remove_all_pages()`
+  * `ReactionMenu.clear_all_row_data()`
+  * `ReactionMenu.remove_page(page_number: int)`
+  * `ReactionMenu.set_main_pages(*embeds: Embed)`
+  * `ReactionMenu.set_last_pages(*embeds: Embed)`
+
+
+#### Adding Pages
+```py
+# ReactionMenu.TypeEmbed
+menu = ReactionMenu(method, menu_type=ReactionMenu.TypeEmbed)
+menu.add_page(summer_embed)
+menu.add_page(winter_embed)
+
+# ReactionMenu.TypeText
+menu = ReactionMenu(method, menu_type=ReactionMenu.TypeText)
+menu.add_page(content='Its so hot!')
+menu.add_page(content='Its so cold!')
+```
+
+#### ReactionMenu.TypeText
+A `TypeText` menu is a text based pagination menu. No embeds are involved in the pagination process, only plain text is used.
+
+![showcase-text](https://cdn.discordapp.com/attachments/655186216060321816/929172629947027466/text_showcase.gif)
+
+#### Stacked Pages
+With `v3.1.0+`, you can paginate with more than just an embed or text. You can combine text, embeds, as well as files. But depending on the `menu_type` the combination can be restricted. Here is an example of a menu with a `menu_type` of `TypeEmbed` that is stacked.
+
+```py
+# You can use regular commands as well
+@bot.tree.command(description="These are stacked pages", guild=discord.Object(id=...))
+async def stacked(interaction: discord.Interaction):
+    menu = ReactionMenu(interaction, menu_type=ReactionMenu.TypeEmbed)
+
+    menu.add_page(discord.Embed(title="My Embed"), content="This content is stacked on top of a file", files=[discord.File("stacked.py")])
+    menu.add_page(discord.Embed(title="Hey Wumpos, can you say hi to the person reading this? 😃"))
+    menu.add_page(discord.Embed(title="Hi, I'm Wumpos!"), files=[discord.File("wumpos.gif")])
+    
+    menu.add_button(ReactionButton.back())
+    menu.add_button(ReactionButton.next())
+    
+    await menu.start()
+```
+![stacked](https://cdn.discordapp.com/attachments/655186216060321816/955966821268332554/stacked.gif)
+
+Since the `menu_type` is `TypeEmbed`, there always has to be an embed on each page. If the `menu_type` was `TypeText`, embeds aren't allowed and you will be restricted to only using the `files` parameter.
+
+#### ReactionMenu.TypeEmbedDynamic
+A dynamic menu is used when you do not know how much information will be applied to the menu. For example, if you were to request information from a database, that information can always change. You query something and you might get 1,500 results back, and the next maybe only 800. A dynamic menu pieces all this information together for you and adds it to an embed page by rows of data. `ReactionMenu.add_row()` is best used in some sort of `Iterable` where everything can be looped through, but only add the amount of data you want to the menu page.
+> **NOTE:** In a dynamic menu, all added data is placed in the description section of an embed. If you choose to use a `custom_embed`, all text in the description will be overridden with the data you add
+* Associated methods
+    * `ReactionMenu.add_row(data: str)`
+    * `ReactionMenu.clear_all_row_data()`
+    * `ReactionMenu.set_main_pages(*embeds: Embed)`
+    * `ReactionMenu.set_last_pages(*embeds: Embed)`
+* The kwargs specifically made for a dynamic menu are:
+    * `rows_requested` - The amount of rows you would like on each embed page before making a new page
+        * `ReactionMenu(..., rows_requested=5)`
+    * `custom_embed` - An embed you have created to use as the embed pages. Used for your menu aesthetic
+        * `ReactionMenu(..., custom_embed=red_embed)`
+    * `wrap_in_codeblock` - The language identifier when wrapping your data in a discord codeblock. 
+        * `ReactionMenu(..., wrap_in_codeblock='py')`
+
+##### Adding Rows/data
+```py
+menu = ReactionMenu(ctx, menu_type=ReactionMenu.TypeEmbedDynamic, rows_requested=5)
+
+for data in database.request('SELECT * FROM customers'):
+    menu.add_row(data)
+```
+##### Deleting Data
+You can remove all the data you've added to a menu by using `menu.clear_all_row_data()`
+
+##### Main/Last Pages
+When using a dynamic menu, the only embed pages you see are from the data you've added. But if you would like to show more pages other than just the data, you can use methods `ReactionMenu.set_main_pages()` and `ReactionMenu.set_last_pages()`. Setting the main page(s), the embeds you set will be the first embeds that are shown when the menu starts. Setting the last page(s) are the last embeds shown
+```py
+menu.set_main_pages(welcome_embed, announcement_embed)
+
+for data in get_information():
+    menu.add_row(data)
+
+menu.set_last_pages(additional_info_embed)
+# NOTE: setting main/last pages can be set in any order
+```
+
+### ReactionButtons and ButtonTypes
+Buttons/button types are used when you want to add a reaction to the menu that does a certain function. Buttons and button types work together to achieve the desired action.
+```
+class reactionmenu.ReactionButton(*, emoji: str, linked_to: ButtonType, **kwargs)
+```
+### Parameters of the ReactionButton constructor
+* `emoji` (`str`) The emoji you would like to use as the reaction
+* `linked_to` (`ReactionButton.Type`) When the reaction is pressed, this is what determines what it will do
+
+### Kwargs of the ReactionButton constructor
+| Name | Type | Default Value | Used for
+|------|------|---------------|----------
+| `embed` | `discord.Embed` | `None` | When the reaction is pressed, go to the specified embed
+| `name` | `str` | `None` | The name of the button
+| `details` | [info below](#reactionbuttons-with-reactionbuttontypecaller) | `None` | Assigns the function and it's arguments to call when a `ReactionButton` with `ReactionButton.Type.CALLER` is pressed
+| `event` | `ReactionButton.Event` | `None` | Determine when a button should be removed depending on how many times it has been pressed
+| `skip` | `ReactionButton.Skip` | `None` | Set the action and the amount of pages to skip when using a `linked_to` of `ReactionButton.Type.SKIP`. For example using this button type, setting the action to "+" and the amount 3. If you are on "Page 1/20", pressing that button will bring you to "Page 4/20"
+
+### Attributes for ReactionButton
+| Property | Return Type | Info
+|----------|-------------|------
+| `clicked_by` | `Set[discord.Member]` | The members who clicked the button
+| `total_clicks` | `int` | Amount of clicks from the button
+| `last_clicked` | `Optional[datetime.datetime]` | The time in UTC for when the button was last clicked
+| `menu` | `Optional[ReactionMenu]` | The menu the button is attached to
+
+* Associated methods
+    * `ReactionMenu.add_button(button: ReactionButton)`
+    * `ReactionMenu.remove_all_buttons()`
+    * `ReactionMenu.remove_button(button: ReactionButton)`
+    * `ReactionMenu.get_button(identity: Union[str, int], *, search_by='name')`
+    * `ReactionButton.set_caller_details(func: Callable[..., None], *args, **kwargs)`
+
+
+### All ButtonTypes
+| Type | Info |
+|-------|------|
+| `ReactionButton.Type.NEXT_PAGE` | Go to the next page in the menu session
+| `ReactionButton.Type.PREVIOUS_PAGE` | Go to the previous page in the menu session
+| `ReactionButton.Type.GO_TO_FIRST_PAGE` | Go to the first page in the menu session
+| `ReactionButton.Type.GO_TO_LAST_PAGE` | Go to the last page in the menu session
+| `ReactionButton.Type.GO_TO_PAGE` | Prompts you to type in the page you'd like to go to
+| `ReactionButton.Type.END_SESSION` | Stops the session and deletes the menu message
+| `ReactionButton.Type.CUSTOM_EMBED` | Used separately from the navigation buttons. Once pressed, go to the specified embed 
+| `ReactionButton.Type.CALLER` | Used when specifying the function to call and it's arguments when the button is pressed
+| `ReactionButton.Type.SKIP` | Used to paginate through multiple pages in a single button press
+
+
+### Adding Buttons
+You can add buttons (reactions) to the menu using a `ReactionButton`. Below are examples on how to use each `ButtonType`. 
+> **NOTE:** ReactionButtons with `ReactionButton.Type.CALLER` are a little different, so there is a dedicated section explaining how they work and how to implement them further below
+
+```py
+menu = ReactionMenu(...)
+
+# first and last pages
+fpb = ReactionButton(emoji='⏪', linked_to=ReactionButton.Type.GO_TO_FIRST_PAGE)
+lpb = ReactionButton(emoji='⏩', linked_to=ReactionButton.Type.GO_TO_LAST_PAGE)
+
+# go to page
+gtpb = ReactionButton(emoji='🔢', linked_to=ReactionButton.Type.GO_TO_PAGE)
+
+# end session
+esb = ReactionButton(emoji='⏹️', linked_to=ReactionButton.Type.END_SESSION)
+
+# custom embed
+ceb = ReactionButton(emoji='😎', linked_to=ReactionButton.Type.CUSTOM_EMBED, embed=discord.Embed(title='Hello'))
+
+# skip button
+sb = ReactionButton(emoji='5️⃣', linked_to=ReactionButton.Type.SKIP, skip=ReactionButton.Skip(action='+', amount=5))
+
+menu.add_button(fpb)
+...
+```
+### Deleting Buttons
+Remove all buttons with `menu.remove_all_buttons()`. You can also remove an individual button using its name if you have it set, or the button object itself with `menu.remove_button()`
+
+### ReactionButtons with ReactionButton.Type.CALLER
+`ReactionButton.Type.CALLER` buttons are used to implement your own functionality into the menu. Maybe you want to add a button that creates a text channel, sends a message, or add something to a database, whatever it may be. In order to work with `ReactionButton.Type.CALLER`, use the class method below.
+
+* `ReactionButton.set_caller_details(func: Callable[..., None], *args, **kwargs)`
+  
+This class method is used to setup a function and it's arguments that are later called when the button is pressed. The `ReactionButton` constructor has the kwarg `details`, and that's what you'll use with `.set_caller_details()` to assign the values needed. Some examples are below on how to properly implement `ReactionButton.Type.CALLER`
+
+```py
+@bot.command()
+async def user(ctx, name, *, message):
+    await ctx.send(f"Hi {name}! {message}. We're glad you're here!")
+
+def car(year, make, model):
+    print(f"I have a {year} {make} {model}")
+
+ub = ReactionButton(emoji='👋', linked_to=ReactionButton.Type.CALLER, details=ReactionButton.set_caller_details(user, ctx, 'Defxult', message='Welcome to the server'))
+cb = ReactionButton(emoji='🚗', linked_to=ReactionButton.Type.CALLER, details=ReactionButton.set_caller_details(car, 2021, 'Ford', 'Mustang'))
+```
+> **NOTE:** The function you pass in should not return anything. Calling functions with `ReactionButton.Type.CALLER` does not store or handle anything returned by that function
+---
+
+### ReactionButton Methods
+The `ReactionButton` class comes with a set factory methods (class methods) that returns a `ReactionButton` with parameters set according to their `linked_to`.
+
+* `ReactionButton.back()`
+  * `emoji`: "◀️"
+  * `linked_to`: `ReactionButton.Type.PREVIOUS_PAGE`
+* `ReactionButton.next()`
+	* `emoji`: "▶️"
+	* `linked_to`: `ReactionButton.Type.NEXT_PAGE`
+* `ReactionButton.go_to_first_page()`
+	* `emoji`: "⏪"
+	* `linked_to`: `ReactionButton.Type.GO_TO_FIRST_PAGE`
+* `ReactionButton.go_to_last_page()`
+	* `emoji`: "⏩"
+	* `linked_to`: `ReactionButton.Type.GO_TO_LAST_PAGE`
+* `ReactionButton.go_to_page()`
+	* `emoji`: "🔢"
+	* `linked_to`: `ReactionButton.Type.GO_TO_PAGE`
+* `ReactionButton.end_session()`
+	* `emoji`: "⏹️"
+	* `linked_to`: `ReactionButton.Type.END_SESSION`
+* `ReactionButton.all()`
+  * Returns a `list` of `ReactionButton` in the following order
+  * `.go_to_first_page()` `.back()` `.next()` `.go_to_last_page()` `.go_to_page()` `.end_session()`
+* `ReactionButton.generate_skip(emoji: str, action: str, amount: int)`
+  * `emoji`: `<emoji>`
+  * `linked_to`: `ReactionButton.Type.SKIP`
+  * `skip`: `ReactionButton.Skip(<action>, <amount>)`
+
+---
+### Setting Limits
+If you'd like, you can limit the amount of reaction menus that can be active at the same time *per* "guild", "member", or "channel" 
+* Associated CLASS Methods
+    * `ReactionMenu.set_sessions_limit(limit: int, per='guild', message='Too many active menus. Wait for other menus to be finished.')` 
+    * `ReactionMenu.remove_limit()`
+
+Example:
+```py
+@bot.command()
+async def limit(ctx):
+    ReactionMenu.set_sessions_limit(3, per='member', message='Sessions are limited to 3 per member')
+```
+
+With the above example, only 3 menus can be active at once for each member, and if they try to create more before their other menu's are finished, they will get an error message saying "Sessions are limited to 3 per member".
+
+### ReactionButton Events
+You can set a `ReactionButton` to be removed when it has been pressed a certain amount of times
+
+```
+class ReactionButton.Event(event_type: str, value: int)
+```
+
+#### Parameters for ReactionButton.Event
+* `event_type` (`str`) The action to take. The only available option is "remove"
+* `value` (`int`) The amount set for the specified event. Must be >= 1. If value is <= 0, it is implicitly set to 1
+
+Example:
+```py
+menu = ReactionMenu(ctx, ...)
+
+# remove a button after 10 clicks
+button = ReactionButton(..., event=ReactionButton.Event('remove', 10))
+menu.add_button(button)
+```
+> **NOTE:** Not ideal for buttons with a `linked_to` of `ReactionButton.Type.END_SESSION`
+---
+### ReactionMenu Relays
+Menu relays are functions that are called anytime a button that is apart of a menu is pressed. It is considered as an extension of a `ReactionButton` with a `linked_to` of `ReactionButton.Type.CALLER`. Unlike caller buttons which provides no details about the interactions on the menu, relays do.
+* Associated methods
+  * `ReactionMenu.set_relay(func: Callable[[NamedTuple], None], *, only: Optional[List[ReactionButton]]=None)`
+  * `ReactionMenu.remove_relay()`
+
+When creating a function for your relay, that function must contain a single positional argument. When a button is pressed, a `RelayPayload` object (a named tuple) is passed to that function. The attributes of `RelayPayload` are:
+* `member` (`discord.Member`) The person who pressed the button
+* `button` (`ReactionButton`) The button that was pressed
+
+Example:
+```py
+async def enter_giveaway(payload):
+    member = payload.member
+    channel = payload.button.menu.message.channel
+    await channel.send(f"{member.mention}, you've entered the giveaway!")
+
+menu = ReactionMenu(ctx, ...)
+menu.set_relay(enter_giveaway)
+```
+The `set_relay` method comes with the `only` parameter. If that parameter is `None`, all buttons that are pressed will be relayed. You can provide a `list` of buttons to that parameter so only button presses from those specified buttons will be relayed.
+```py
+def example(payload):
+    ...
+
+menu = ReactionMenu(ctx, ...)
+
+back_button = ReactionButton.back()
+next_button = ReactionButton.next()
+
+menu.set_relay(example, only=[back_button])
+```
+
+---
+### Starting/Stopping the ReactionMenu
+* Associated methods
+  * `await ReactionMenu.start(*, send_to=None, reply=False)`
+  * `await ReactionMenu.stop(*, delete_menu_message=False, clear_reactions=False)`
+
+When starting the menu, you have the option to send the menu to a certain channel. Parameter `send_to` is the channel you'd like to send the menu to. You can set `send_to` as the channel name (`str`), channel ID (`int`), or channel object (`discord.TextChannel` / `discord.Thread`). Example:
+```py
+menu = ReactionMenu(...)
+# channel name
+await menu.start(send_to='bot-commands')
+
+# channel ID
+await menu.start(send_to=1234567890123456)
+
+# channel object
+channel = guild.get_channel(1234567890123456)
+await menu.start(send_to=channel)
+
+# there's no need to specify send_to unless you want the menu to be sent to a different channel
+# from the one you're sending the initial message/using the command in. the menu can be started
+# in the current channel by omitting the send_to parameter
+await menu.start()
+```
+> **NOTE:** `send_to` is not valid if a menu was started in DM's
+
+### Full Example
+Here is a basic implementation of `ReactionMenu` that you can copy & paste for a quick demonstration.
+```py
+import asyncio
+import discord
+from discord.ext import commands
+from reactionmenu import ReactionMenu, ReactionButton
+
+bot = commands.Bot(command_prefix='!', intents=discord.Intents.all())
+
+async def start_bot():
+    async with bot:
+        await bot.start('...')
+
+@bot.command()
+async def example(ctx):
+    menu = ReactionMenu(ctx, menu_type=ReactionMenu.TypeEmbed)
+    
+    for member in ctx.guild.members:
+        if member.avatar:
+            embed = discord.Embed(description=f'Joined {member.joined_at.strftime("%b. %d, %Y")}')
+            embed.set_author(name=member.name, icon_url=member.avatar.url)
+            menu.add_page(embed)
+    
+    menu.add_button(ReactionButton.back())
+    menu.add_button(ReactionButton.next())
+    menu.add_button(ReactionButton.end_session())
+    
+    await menu.start()
+
+asyncio.run(start_bot())
+```
+</details>
+
+
+
+
+
+
+
+
+
+
+---
+
+
+
+
+
+
+
+
+
+
+## ViewMenu
+```
+class reactionmenu.ViewMenu(method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs)
+```
+
+A `ViewMenu` is a menu that uses discords Buttons feature. With buttons, you can enable and disable them, set a certain color for them with emojis, have buttons that send hidden messages, and add hyperlinks. This library offers a broader range of functionalities such as who pressed the button, how many times it was pressed and more. It uses views (`discord.ui.View`) to implement the Buttons functionality, but uses some of its own methods in order to make a Button pagination menu simple.
+
+![image](https://cdn.discordapp.com/attachments/655186216060321816/855818139450081280/buttons_showcase_reduced.gif)
+
+<details>
+  <summary><b>Click to show ViewMenu documentation</b></summary>
+
+
+### How to import
+```py
+from reactionmenu import ViewMenu, ViewButton
+```
+---
+
+### Parameters of the ViewMenu constructor
+* `method` (`Union[discord.ext.commands.Context, discord.Interaction]`) A context or interaction object
+* `menu_type` (`MenuType`) The configuration of the menu
+  * `ViewMenu.TypeEmbed`, a normal embed pagination menu
+  * `ViewMenu.TypeEmbedDynamic`, an embed pagination menu with dynamic data
+  * `ViewMenu.TypeText`, a text only pagination menu
+
+---
+### Kwargs of the ViewMenu constructor
+| Name | Type | Default Value | Used for | Info 
+-------|------|---------------|----------|------
+| `wrap_in_codeblock` | `str` | `None` | `ViewMenu.TypeEmbedDynamic` | The discord codeblock language identifier to wrap your data in. Example: `ViewMenu(ctx, ..., wrap_in_codeblock='py')`
+| `custom_embed` | `discord.Embed` | `None` | `ViewMenu.TypeEmbedDynamic` | Embed object to use when adding data with `ViewMenu.add_row()`. Used for styling purposes
+| `delete_on_timeout` | `bool` | `False` | `All menu types` | Delete the menu when it times out
+| `disable_items_on_timeout` | `bool` | `True` | `All menu types` | Disable the items on the menu when the menu times out
+| `remove_items_on_timeout` | `bool` | `False` | `All menu types` | Remove the items on the menu when the menu times out
+| `only_roles` | `List[discord.Role]` | `None` | `All menu types` | If set, only members with any of the given roles are allowed to control the menu. The menu owner can always control the menu
+| `timeout` | `Union[int, float, None]` | `60.0` | `All menu types` | The timer for when the menu times out. Can be `None` for no timeout
+| `show_page_director` | `bool` | `True` | `All menu types` | Shown at the bottom of each embed page. "Page 1/20"
+| `name` | `str` | `None` | `All menu types` | A name you can set for the menu
+| `style` | `str` | `"Page $/&"` | `All menu types` | A custom page director style you can select. "$" represents the current page, "&" represents the total amount of pages. Example: `ViewMenu(ctx, ..., style='On $ out of &')`
+| `all_can_click` | `bool` | `False` | `All menu types` | Sets if everyone is allowed to control when pages are 'turned' when buttons are clicked
+| `delete_interactions` | `bool` | `True` | `All menu types` | Delete the prompt message by the bot and response message by the user when asked what page they would like to go to when using `ViewButton.ID_GO_TO_PAGE`
+| `rows_requested` | `int` | `None` | `ViewMenu.TypeEmbedDynamic` | The amount of information per `ViewMenu.add_row()` you would like applied to each embed page
+---
+
+### Pages for ViewMenu
+Depending on the `menu_type`, pages can either be a `str`, `discord.Embed`, or a combination of `content` or `files` ([example below](#stacked-pages-1))
+* If the `menu_type` is `ViewMenu.TypeEmbed`, use embeds
+* If the `menu_type` is `ViewMenu.TypeText` (text only menu) or `ViewMenu.TypeEmbedDynamic` (embed only menu), use strings.
+* Associated methods
+  * `ViewMenu.add_page(embed: discord.Embed=MISSING, content: Optional[str]=None, files: Optional[Sequence[discord.File]]=None)`
+  * `ViewMenu.add_pages(pages: Sequence[Union[discord.Embed, str]])`
+  * `ViewMenu.add_row(data: str)`
+  * `ViewMenu.remove_all_pages()`
+  * `ViewMenu.clear_all_row_data()`
+  * `ViewMenu.remove_page(page_number: int)`
+  * `ViewMenu.set_main_pages(*embeds: Embed)`
+  * `ViewMenu.set_last_pages(*embeds: Embed)`
+
+#### Adding Pages
+```py
+# ViewMenu.TypeEmbed
+menu = ViewMenu(method, menu_type=ViewMenu.TypeEmbed)
+menu.add_page(summer_embed)
+menu.add_page(winter_embed)
+
+# ViewMenu.TypeText
+menu = ViewMenu(method, menu_type=ViewMenu.TypeText)
+menu.add_page(content='Its so hot!')
+menu.add_page(content='Its so cold!')
+```
+
+#### ViewMenu.TypeText
+A `TypeText` menu is a text based pagination menu. No embeds are involved in the pagination process, only plain text is used.
+
+![text_view_showcase](https://cdn.discordapp.com/attachments/655186216060321816/929744985656549386/text_view_showcase.gif)
+
+#### Stacked Pages
+With `v3.1.0+`, you can paginate with more than just an embed or text. You can combine text, embeds, as well as files. But depending on the `menu_type` the combination can be restricted. Here is an example of a menu with a `menu_type` of `TypeEmbed` that is stacked.
+
+```py
+# You can use regular commands as well
+@bot.tree.command(description="These are stacked pages", guild=discord.Object(id=...))
+async def stacked(interaction: discord.Interaction):
+    menu = ViewMenu(interaction, menu_type=ViewMenu.TypeEmbed)
+
+    menu.add_page(discord.Embed(title="My Embed"), content="This content is stacked on top of a file", files=[discord.File("stacked.py")])
+    menu.add_page(discord.Embed(title="Hey Wumpos, can you say hi to the person reading this? 😃"))
+    menu.add_page(discord.Embed(title="Hi, I'm Wumpos!"), files=[discord.File("wumpos.gif")])
+    
+    menu.add_button(ViewButton.back())
+    menu.add_button(ViewButton.next())
+    
+    await menu.start()
+```
+![stacked_view](https://cdn.discordapp.com/attachments/655186216060321816/955983620038860910/stacked_view.gif)
+
+Since the `menu_type` is `TypeEmbed`, there always has to be an embed on each page. If the `menu_type` was `TypeText`, embeds aren't allowed and you will be restricted to only using the `files` parameter.
+
+#### ViewMenu.TypeEmbedDynamic
+A dynamic menu is used when you do not know how much information will be applied to the menu. For example, if you were to request information from a database, that information can always change. You query something and you might get 1,500 results back, and the next maybe only 800. A dynamic menu pieces all this information together for you and adds it to an embed page by rows of data. `ViewMenu.add_row()` is best used in some sort of `Iterable` where everything can be looped through, but only add the amount of data you want to the menu page.
+> **NOTE:** In a dynamic menu, all added data is placed in the description section of an embed. If you choose to use a `custom_embed`, all text in the description will be overridden with the data you add
+* Associated methods
+    * `ViewMenu.add_row(data: str)`
+    * `ViewMenu.clear_all_row_data()`
+    * `ViewMenu.set_main_pages(*embeds: Embed)`
+    * `ViewMenu.set_last_pages(*embeds: Embed)`
+* The kwargs specifically made for a dynamic menu are:
+    * `rows_requested` - The amount of rows you would like on each embed page before making a new page
+        * `ViewMenu(..., rows_requested=5)`
+    * `custom_embed` - An embed you have created to use as the embed pages. Used for your menu aesthetic
+        * `ViewMenu(..., custom_embed=red_embed)`
+    * `wrap_in_codeblock` - The language identifier when wrapping your data in a discord codeblock. 
+        * `ViewMenu(..., wrap_in_codeblock='py')`
+
+##### Adding Rows/data
+```py
+menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbedDynamic, rows_requested=5)
+
+for data in database.request('SELECT * FROM customers'):
+    menu.add_row(data)
+```
+##### Deleting Data
+You can remove all the data you've added to a menu by using `menu.clear_all_row_data()`
+
+##### Main/Last Pages
+When using a dynamic menu, the only embed pages you see are from the data you've added. But if you would like to show more pages other than just the data, you can use methods `ViewMenu.set_main_pages()` and `ViewMenu.set_last_pages()`. Setting the main page(s), the embeds you set will be the first embeds that are shown when the menu starts. Setting the last page(s) are the last embeds shown
+```py
+menu.set_main_pages(welcome_embed, announcement_embed)
+
+for data in get_information():
+    menu.add_row(data)
+
+menu.set_last_pages(additional_info_embed)
+# NOTE: setting main/last pages can be set in any order
+```
+
+### Buttons for ViewMenu
+Buttons are what you use to interact with the menu. Unlike reactions, they look cleaner, provides less rate limit issues, and offer more in terms of interactions. Enable and disable buttons, use markdown hyperlinks in it's messages, and even send hidden messages.
+
+![discord_buttons](https://discord.com/assets/7bb017ce52cfd6575e21c058feb3883b.png)
+
+
+* Associated methods
+  * `ViewMenu.add_button(button: ViewButton)`
+  * `ViewMenu.disable_all_buttons()`
+  * `ViewMenu.disable_button(button: ViewButton)`
+  * `ViewMenu.enable_all_buttons()`
+  * `ViewMenu.enable_button(button: ViewButton)`
+  * `ViewMenu.get_button(identity: str, *, search_by='label')`
+  * `ViewMenu.remove_all_buttons()`
+  * `ViewMenu.remove_button(button: ViewButton)`
+  * `await ViewMenu.refresh_menu_items()`
+
+#### ViewButton
+```
+class reactionmenu.ViewButton(*, style=discord.ButtonStyle.secondary, label=None, disabled=False, custom_id=None, url=None, emoji=None, followup=None, event=None, **kwargs)
+```
+
+A `ViewButton` is a class that represents the discord button. It is a subclass of `discord.ui.Button`.
+
+The following are the rules set by Discord for Buttons:
+* Link buttons don't send interactions to the Discord App, so link button statistics (it's properties) are not tracked
+* Non-link buttons **must** have a `custom_id`, and cannot have a `url`
+* Link buttons **must** have a `url`, and cannot have a `custom_id`
+* There cannot be more than 25 buttons per message
+---
+#### Parameters of the ViewButton constructor
+* `style` (`discord.ButtonStyle`) The button style
+* `label` (`str`) The text on the button
+* `custom_id` (`str`) An ID to determine what action that button should take. Available IDs:
+  * `ViewButton.ID_NEXT_PAGE`
+  * `ViewButton.ID_PREVIOUS_PAGE`
+  * `ViewButton.ID_GO_TO_FIRST_PAGE` 
+  * `ViewButton.ID_GO_TO_LAST_PAGE`
+  * `ViewButton.ID_GO_TO_PAGE`
+  * `ViewButton.ID_END_SESSION`
+  * `ViewButton.ID_CALLER`
+  * `ViewButton.ID_SEND_MESSAGE`
+  * `ViewButton.ID_CUSTOM_EMBED`
+  * `ViewButton.ID_SKIP`
+* `emoji` (`Union[str, discord.PartialEmoji]`) Emoji used for the button
+  * `ViewButton(..., emoji='😄')` 
+  * `ViewButton(..., emoji='<:miscTwitter:705423192818450453>')`
+  * `ViewButton(..., emoji='\U000027a1')`
+  * `ViewButton(..., emoji='\N{winking face}')`
+* `url` (`str`) URL for a button with style `discord.ButtonStyle.link`
+* `disabled` (`bool`) If the button should be disabled
+* `followup` (`ViewButton.Followup`) The message sent after the button is pressed. Only available for buttons that have a `custom_id` of `ViewButton.ID_CALLER` or `ViewButton.ID_SEND_MESSAGE`. `ViewButton.Followup` is a class that has parameters similar to `discord.abc.Messageable.send()`, and is used to control if a message is ephemeral, contains a file, embed, tts, etc...
+* `event` (`ViewButton.Event`) Set a button to be disabled or removed when it has been pressed a certain amount of times
+
+#### Kwargs of the ViewButton constructor
+| Name | Type | Default Value | Used for
+|------|------|---------------|----------
+| `name` | `str` | `None` | The name of the button
+| `skip` | `ViewButton.Skip` | `None` | Set the action and the amount of pages to skip when using a `custom_id` of `ViewButton.ID_SKIP`. For example, setting the action to "+" and the amount 3. If you are on "Page 1/20", pressing that button will bring you to "Page 4/20"
+| `persist` | `bool` | `False` | Prevents link buttons from being disabled/removed when the menu times out or is stopped so they can remain clickable
+
+#### Attributes for ViewButton
+| Property | Return Type | Info
+|----------|-------------|------
+| `clicked_by` | `Set[discord.Member]` | The members who clicked the button
+| `total_clicks` | `int` | Amount of clicks from the button
+| `last_clicked` | `Optional[datetime.datetime]` | The time in UTC for when the button was last clicked
+| `menu` | `Optional[ViewMenu]` | The menu the button is attached to
+
+#### Adding a ViewButton
+```py
+from reactionmenu import ViewMenu, ViewButton
+
+menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
+
+# Link button
+link_button = ViewButton(style=discord.ButtonStyle.link, emoji='🌍', label='Link to Google', url='https://google.com')
+menu.add_button(link_button)
+
+# Skip button
+skip = ViewButton(style=discord.ButtonStyle.primary, label='+5', custom_id=ViewButton.ID_SKIP, skip=ViewButton.Skip(action='+', amount=5))
+menu.add_button(skip)
+
+# ViewButton.ID_PREVIOUS_PAGE
+back_button = ViewButton(style=discord.ButtonStyle.primary, label='Back', custom_id=ViewButton.ID_PREVIOUS_PAGE)
+menu.add_button(back_button)
+
+# ViewButton.ID_NEXT_PAGE
+next_button = ViewButton(style=discord.ButtonStyle.secondary, label='Next', custom_id=ViewButton.ID_NEXT_PAGE)
+menu.add_button(next_button)
+
+# All other ViewButton are created the same way as the last 2 EXCEPT
+# 1 - ViewButton.ID_CALLER
+# 2 - ViewButton.ID_SEND_MESSAGE
+# 3 - ViewButton.ID_CUSTOM_EMBED
+
+
+# ViewButton.ID_CALLER
+def say_hello(name: str):
+    print('Hello', name)
+
+call_followup = ViewButton.Followup(details=ViewButton.Followup.set_caller_details(say_hello, 'John'))
+menu.add_button(ViewButton(label='Say hi', custom_id=ViewButton.ID_CALLER, followup=call_followup))
+
+# ViewButton.ID_SEND_MESSAGE
+msg_followup = ViewButton.Followup('This message is hidden!', ephemeral=True)
+menu.add_button(ViewButton(style=discord.ButtonStyle.green, label='Message', custom_id=ViewButton.ID_SEND_MESSAGE, followup=msg_followup))
+
+# ViewButton.ID_CUSTOM_EMBED
+custom_embed_button = ViewButton(style=discord.ButtonStyle.blurple, label='Social Media Info', custom_id=ViewButton.ID_CUSTOM_EMBED, followup=ViewButton.Followup(embed=discord.Embed(...)))
+```
+---
+> **NOTE:** When it comes to buttons with a `custom_id` of `ViewButton.ID_CALLER`, `ViewButton.ID_SEND_MESSAGE`, `ViewButton.ID_CUSTOM_EMBED`, or link buttons, you can add as many as you'd like as long as in total it's 25 buttons or less. For all other button ID's, each menu can only have one.
+
+### Using Selects
+Selects are used when you'd like to categorize information in your menu. Selects can only be used when the menu's `menu_type` is `TypeEmbed`. You should keep in mind that discords limitations on how many menu UI items (rows) can be applied to each message.
+
+![select_showcase](https://cdn.discordapp.com/attachments/655186216060321816/971361708121653268/select_showcase.gif)
+
+* Associated Methods
+  * `ViewMenu.add_select(select: ViewSelect)`
+  * `ViewMenu.remove_select(select: ViewSelect)`
+  * `ViewMenu.remove_all_selects()`
+  * `ViewMenu.disable_select(select: ViewSelect)`
+  * `ViewMenu.disable_all_selects()`
+  * `ViewMenu.enable_select(select: ViewSelect)`
+  * `ViewMenu.enable_all_selects()`
+  * `ViewMenu.get_select(title: Union[str, None])`
+
+Example:
+```py
+from reactionmenu import ViewMenu, ViewSelect, Page
+
+menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
+menu.add_page(discord.Embed(title="A showcase of console video games", color=discord.Color.blurple()))
+
+menu.add_select(ViewSelect(title="Console Video Games", options={
+    discord.SelectOption(label="PlayStation", emoji="<:PlayStation:549638412538478602>") : [
+        Page(embed=discord.Embed(title="Ratchet & Clank", description=..., color=discord.Color.yellow()).set_image(url=...)),
+        Page(embed=discord.Embed(title="God of War", description=..., color=discord.Color.blue()).set_image(url=...))
+    ],
+    discord.SelectOption(label="Xbox", emoji="<:Xbox:501880493285834752>") : [
+        Page(embed=discord.Embed(title="Halo Infinite", description=..., color=discord.Color.green()).set_image(url=...)),
+        Page(embed=discord.Embed(title="Gears of War 4", description=..., color=discord.Color.red()).set_image(url=...))
+    ]
+}))
+
+menu.add_button(ViewButton.back())
+menu.add_button(ViewButton.next())
+await menu.start()
+```
+
+#### Go to page navigation
+You can use this type of select when you'd like to use the UI to select a page to go to.
+
+![goto_showcase](https://cdn.discordapp.com/attachments/655186216060321816/973629631905300501/Discord_6SP5AjoOOM.gif)
+
+* Associated methods
+  * `ViewMenu.add_go_to_select(goto: ViewSelect.GoTo)`
+  * `ViewMenu.enable_go_to_select(goto: ViewSelect.GoTo)`
+  * `ViewMenu.enable_all_go_to_selects()`
+  * `ViewMenu.disable_go_to_select(goto: ViewSelect.GoTo)`
+  * `ViewMenu.disable_all_go_to_selects()`
+  * `ViewMenu.remove_go_to_select(goto: ViewSelect.GoTo)`
+  * `ViewMenu.remove_all_go_to_selects()`
+
+The `page_numbers` parameter for `ViewSelect.GoTo` can be used with 3 different types
+
+1. `List[int]` If set to a list of integers, those specified values are the only options that are available when the select is clicked
+   1. `page_numbers=[1, 5, 10]`
+2. `Dict[int, Union[str, discord.Emoji, discord.PartialEmoji]]` You can use this type if you'd like to utilize emojis in your select
+   1. `page_numbers={1 : "🗯️", 2 : "📺"}`
+3. `ellipsis` You can set a *literal* ellipsis to have the library automatically assign all page numbers to the amount of pages that you've added to the menu. This can come in handy if you have 25 pages or less
+   1. `page_numbers=...`
+> **NOTE**: Setting the `page_numbers` parameter to an ellipsis (...) only works as intended if you've added the go to select AFTER you've added pages to the menu
+
+```py
+@bot.command()
+async def navigate(ctx):
+    menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
+
+    menu.add_page(discord.Embed(title="Twitter").set_image(url="..."))
+    menu.add_page(discord.Embed(title="YouTube").set_image(url="..."))
+    menu.add_page(discord.Embed(title="Discord").set_image(url="..."))
+    # ...
+    
+    menu.add_go_to_select(ViewSelect.GoTo(title="Go to page...", page_numbers=...))
+
+    menu.add_button(ViewButton.back())
+    menu.add_button(ViewButton.next())
+
+    await menu.start()
+```
+
+### Updating ViewButton and Pages
+* Associated methods
+  * `await ViewMenu.refresh_menu_items()`
+  * `await ViewMenu.update(*, new_pages: Union[List[Union[Embed, str]], None], new_buttons: Union[List[ViewButton], None])`
+
+When the menu is running, you can update the pages or buttons on the menu. Using `ViewMenu.update()`, you can replace the pages and buttons. Using `ViewMenu.refresh_menu_items()` updates the buttons you have changed.
+
+#### Updating a Button
+```py
+@bot.command()
+async def menu(ctx):
+    menu = ViewMenu(..., name='test')
+    link_button = ViewButton(..., label='Link')
+    
+    menu.add_button(link_button)
+    menu.add_page(...)
+
+    await menu.start()
+
+
+@bot.command()
+async def disable(ctx):
+    menu = ViewMenu.get_session('test')
+    link_button = menu[0].get_button('Link', search_by='label')
+    
+    menu.disable_button(link_button)
+    await menu.refresh_menu_items()
+```
+If the buttons are not refreshed with `ViewMenu.refresh_menu_items()`, the menu will not be updated when changing a button.
+
+#### Updating Pages and Buttons
+Method `ViewMenu.update(...)` is used when you want to replace all or a few of the buttons on the menu. 
+```py
+menu = ViewMenu(...)
+
+# in a different .command()
+await menu.update(new_pages=[hello_embed, goodbye_embed], new_buttons=[link_button, next_button])
+```
+
+> **NOTE**: When using `ViewMenu.update(...)`, there is no need to use `ViewMenu.refresh_menu_items()` because they are updated during the update call. 
+
+---
+#### ViewButton Methods
+The `ViewButton` class comes with a set factory methods (class methods) that returns a `ViewButton` with parameters set according to their `custom_id` (excluding link buttons).
+
+* `ViewButton.link(label: str, url: str)`
+  * `style`: `discord.ButtonStyle.link`
+  * `label`: `<label>`
+  * `url`: `<url>`
+* `ViewButton.back()`
+  * `style`: `discord.ButtonStyle.gray`
+  * `label`: "Back"
+  * `custom_id`: `ViewButton.ID_PREVIOUS_PAGE`
+* `ViewButton.next()`
+	* `style`: `discord.ButtonStyle.gray`
+	* `label`: "Next"
+	* `custom_id`: `ViewButton.ID_NEXT_PAGE`
+* `ViewButton.go_to_first_page()`
+	* `style`: `discord.ButtonStyle.gray`
+	* `label`: "First Page"
+	* `custom_id`: `ViewButton.ID_GO_TO_FIRST_PAGE`
+* `ViewButton.go_to_last_page()`
+	* `style`: `discord.ButtonStyle.gray`
+	* `label`: "Last Page"
+	* `custom_id`: `ViewButton.ID_GO_TO_LAST_PAGE`
+* `ViewButton.go_to_page()`
+	* `style`: `discord.ButtonStyle.gray`
+	* `label`: "Page Selection"
+	* `custom_id`: `ViewButton.ID_GO_TO_PAGE`
+* `ViewButton.end_session()`
+	* style: `discord.ButtonStyle.gray`
+	* label: "Close"
+	* custom_id: `ViewButton.ID_END_SESSION`
+* `ViewButton.all()`
+  * Returns a `list` of `ViewButton` in the following order
+  * `.go_to_first_page()` `.back()` `.next()` `.go_to_last_page()` `.go_to_page()` `.end_session()`
+* `ViewButton.all_with_emojis()`
+  * Returns a `list` of `ViewButton` with their `emoji` parameters already set in the following order
+  * `.go_to_first_page()` `.back()` `.next()` `.go_to_last_page()` `.go_to_page()` `.end_session()`
+* `ViewButton.generate_skip(label: str, action: str, amount: int)`
+  * `style`: `discord.ButtonStyle.gray`
+  * `label`: `<label>`
+  * `custom_id`: `ViewButton.ID_SKIP`
+  * `skip`: `ViewButton.Skip(<action>, <amount>)`
+
+```py
+menu = ViewMenu(ctx, ...)
+menu.add_page(...)
+menu.add_page(...)
+
+menu.add_button(ViewButton.back())
+menu.add_button(ViewButton.next())
+
+await menu.start()
+```
+---
+### ViewButton Events
+You can set a `ViewButton` to be disabled or removed when it has been pressed a certain amount of times
+
+```
+class ViewButton.Event(event_type: str, value: int)
+```
+
+#### Parameters for ViewButton.Event
+* `event_type` (`str`) The action to take. Can either be "disable" or "remove"
+* `value` (`int`) The amount set for the specified event. Must be >= 1. If value is <= 0, it is implicitly set to 1
+
+Example:
+```py
+menu = ViewMenu(ctx, ...)
+
+# disable a button after 5 clicks
+button_1 = ViewButton(..., event=ViewButton.Event('disable', 5))
+menu.add_button(button_1)
+
+# remove a button after 10 clicks
+button_2 = ViewButton(..., event=ViewButton.Event('remove', 10))
+menu.add_button(button_2)
+```
+> **NOTE:** Not valid for link buttons. Also not ideal for buttons with a `custom_id` of `ViewButton.ID_END_SESSION`
+---
+### ViewMenu Relays
+Menu relays are functions that are called anytime a button that is apart of a menu is pressed. It is considered as an extension of a `ViewButton` with an ID of `ViewButton.ID_CALLER`. Unlike caller buttons which provides no details about the interactions on the menu, relays do.
+* Associated methods
+  * `ViewMenu.set_relay(func: Callable[[NamedTuple], None], *, only: Optional[List[ViewButton]]=None)`
+  * `ViewMenu.remove_relay()`
+
+When creating a function for your relay, that function must contain a single positional argument. When a button is pressed, a `RelayPayload` object (a named tuple) is passed to that function. The attributes of `RelayPayload` are:
+* `member` (`discord.Member`) The person who pressed the button
+* `button` (`ViewButton`) The button that was pressed
+
+Example:
+```py
+async def enter_giveaway(payload):
+    member = payload.member
+    channel = payload.button.menu.message.channel
+    await channel.send(f"{member.mention}, you've entered the giveaway!")
+
+menu = ViewMenu(ctx, ...)
+menu.set_relay(enter_giveaway)
+```
+The `set_relay` method comes with the `only` parameter. If that parameter is `None`, all buttons that are pressed will be relayed (except link buttons because they don't send interaction events). You can provide a `list` of buttons to that parameter so only button presses from those specified buttons will be relayed.
+```py
+def example(payload):
+    ...
+
+menu = ViewMenu(ctx, ...)
+
+back_button = ViewButton.back()
+next_button = ViewButton.next()
+
+menu.set_relay(example, only=[back_button])
+```
+
+---
+### Starting/Stopping the ViewMenu
+* Associated methods
+  * `await ViewMenu.start(*, send_to=None, reply=False)`
+  * `await ViewMenu.stop(*, delete_menu_message=False, remove_buttons=False, disable_buttons=False)`
+
+When starting the menu, you have the option to send the menu to a certain channel. Parameter `send_to` is the channel you'd like to send the menu to. You can set `send_to` as the channel name (`str`), channel ID (`int`), or channel object (`discord.TextChannel` / `discord.Thread`). Example:
+```py
+menu = ViewMenu(...)
+# channel name
+await menu.start(send_to='bot-commands')
+
+# channel ID
+await menu.start(send_to=1234567890123456)
+
+# channel object
+channel = guild.get_channel(1234567890123456)
+await menu.start(send_to=channel)
+
+# there's no need to specify send_to unless you want the menu to be sent to a different channel
+# from the one you're sending the initial message/using the command in. the menu can be started
+# in the current channel by omitting the send_to parameter
+await menu.start()
+```
+> **NOTE:** `send_to` is not valid if a menu was started in DM's
+
+Only one option is available when stopping the menu. If you have multiple parameters as `True`, only one will execute
+- `delete_menu_message` > `disable_buttons`
+- `disable_buttons` > `remove_buttons`
+---
+
+### Full Example
+Here is a basic implementation of `ViewMenu` that you can copy & paste for a quick demonstration.
+```py
+import asyncio
+import discord
+from discord.ext import commands
+from reactionmenu import ViewMenu, ViewButton
+
+bot = commands.Bot(command_prefix='!', intents=discord.Intents.all())
+
+async def start_bot():
+    async with bot:
+        await bot.start('...')
+
+@bot.command()
+async def example(ctx):
+    menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
+    
+    for member in ctx.guild.members:
+        if member.avatar:
+            embed = discord.Embed(description=f'Joined {member.joined_at.strftime("%b. %d, %Y")}')
+            embed.set_author(name=member.name, icon_url=member.avatar.url)
+            menu.add_page(embed)
+    
+    menu.add_button(ViewButton.back())
+    menu.add_button(ViewButton.next())
+    menu.add_button(ViewButton.end_session())
+    
+    await menu.start()
+
+asyncio.run(start_bot())
+```
+</details>
```

