# Comparing `tmp/clibrary-1.8.1.tar.gz` & `tmp/clibrary-1.9.0.tar.gz`

## Comparing `clibrary-1.8.1.tar` & `clibrary-1.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 clibrary-1.8.1/Makefile
--rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 clibrary-1.8.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 clibrary-1.8.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 clibrary-1.8.1/.github/SECURITY.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 clibrary-1.8.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 clibrary-1.8.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 clibrary-1.8.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 clibrary-1.8.1/docs/docs.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clibrary-1.8.1/src/CLIbrary/__init__.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 clibrary-1.8.1/src/CLIbrary/__main__.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 clibrary-1.8.1/src/CLIbrary/files.py
--rw-r--r--   0        0        0    10485 2020-02-02 00:00:00.000000 clibrary-1.8.1/src/CLIbrary/inputs.py
--rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 clibrary-1.8.1/src/CLIbrary/interface.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 clibrary-1.8.1/src/CLIbrary/outputs.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 clibrary-1.8.1/src/CLIbrary/settings.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 clibrary-1.8.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 clibrary-1.8.1/LICENSE
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 clibrary-1.8.1/README.md
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 clibrary-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 clibrary-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 clibrary-1.9.0/Makefile
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 clibrary-1.9.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 clibrary-1.9.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 clibrary-1.9.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 clibrary-1.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 clibrary-1.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 clibrary-1.9.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    11203 2020-02-02 00:00:00.000000 clibrary-1.9.0/docs/docs.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clibrary-1.9.0/src/CLIbrary/__init__.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 clibrary-1.9.0/src/CLIbrary/__main__.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 clibrary-1.9.0/src/CLIbrary/files.py
+-rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 clibrary-1.9.0/src/CLIbrary/inputs.py
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 clibrary-1.9.0/src/CLIbrary/interface.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 clibrary-1.9.0/src/CLIbrary/outputs.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 clibrary-1.9.0/src/CLIbrary/settings.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 clibrary-1.9.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 clibrary-1.9.0/LICENSE
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 clibrary-1.9.0/README.md
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 clibrary-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 clibrary-1.9.0/PKG-INFO
```

### Comparing `clibrary-1.8.1/.github/CODE_OF_CONDUCT.md` & `clibrary-1.9.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `clibrary-1.8.1/.github/CONTRIBUTING.md` & `clibrary-1.9.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `clibrary-1.8.1/.github/ISSUE_TEMPLATE/bug_report.md` & `clibrary-1.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `clibrary-1.8.1/.github/ISSUE_TEMPLATE/feature_request.md` & `clibrary-1.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `clibrary-1.8.1/.github/workflows/python-publish.yml` & `clibrary-1.9.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `clibrary-1.8.1/docs/docs.md` & `clibrary-1.9.0/docs/docs.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,16 +60,17 @@
 ### Settings
 
 As of version 1.2.1, CLIbrary has some "global options" to allow even more personalization.  
 Available options are:
 
 1. `CLIbrary.style.setting_darkMode`, bool: Enables global dark mode. Dafault: `False`.
 2. `CLIbrary.style.setting_plainMode`, bool: Disables styling. Default: `False`.
-3. `CLIbrary.input.setting_caseSensitive`, bool: Enables case-sensitiveness. Default: `False`.
+3. `CLIbrary.style.setting_caseSensitive`, bool: Enables case-sensitiveness. Default: `False`.
 4. `CLIbrary.data.setting_fileExtension`, str: Defines a file extension for *CLIbrary.aDump* and *CLIbrary.aLoad*. Default: `".pickle"`
+5. `CLIbrary.commands.setting_enableCompletion`, bool: Enables command completion. Default: `True`
 
 ### Import CLIbrary
 
 **CLIbrary** can be installed by:
 
 	python3 -m pip install --upgrade CLIbrary
 
@@ -92,18 +93,19 @@
 ## Interface
 
 [Go back to ToC](#table-of-contents)
 
 ### CLI
 
 ``` python
-CLIbrary.cmdIn(commandHandler={}) -> dict
+CLIbrary.cmdIn(commandHandler: dict = {}) -> dict
 ```
 
-*cmdIn* stands for *Command Input* as this function allows the user to input command as in a CLI interface.
+*cmdIn* stands for *Command Input* as this function allows the user to input command as in a CLI interface.  
+As of version 1.9.0, CLIbrary supports tab completion and hinting thanks to [cmdInput](#cmdinput).
 
 The handler for this function makes use of the following parameters:
 * request, str: The prompt to the user.
 * added, str: A set of characters to be automatically added to the prompt. Default is ": ".
 * style, str[^1]: A particular colour style to be applied to the prompt.
 * verbose, bool.
 * allowedCommands, list: A list of all the allowed commands for the CLI interface.
@@ -120,26 +122,36 @@
 
 with no more than a single word for the command itself.
 
 [^1]: Colorama styling works best for styling inside **CLIbrary**.
 
 [^2]: The options get returned without the dashes.
 
+### cmdInput
+
+``` python
+CLIbrary.interface.cmdInput(handler: dict) -> None
+```
+
+*cmdInput* is cmdIn's alternative to Python's input which allows for tab completion and hinting.
+There's no need to call this function manually as its calls are embedded inside *cmdIn*.
+
 ### Option parser
 
 ``` python
-CLIbrary.optionParser(instructions: list) -> None
+CLIbrary.interface.optionParser(instructions: list) -> None
 ```
 
 *optionParser* is a function that receives a list of strings and returns the single dash options sdOpts, a dictionary, and the double dash options, a list.
+There's no need to call this function manually as its calls are embedded inside *cmdIn*.
 
 ### Help
 
 ``` python
-CLIbrary.helpPrint(handler={}) -> None
+CLIbrary.interface.helpPrint(handler: dict) -> None
 ```
 
 *helpPrint* is a function that reads and print the help JSON whose path gets passed to *cmdIn*.
 There's no need to call this function manually as its calls are embedded inside *cmdIn*.
 
 ### Help entries
 
@@ -221,15 +233,15 @@
 ## Inputs
 
 [Go back to ToC](#table-of-contents)
 
 ### Strings
 
 ``` python
-CLIbrary.strIn(stringHandler={}) -> str
+CLIbrary.strIn(stringHandler: dict = {}) -> str
 ```
 
 *strIn* stands for *String Input* as this function's purpose is receiving string inputs.
 
 The handler for this function makes use of the following parameters:
 * Strings.
 	* request: The prompt to the user.
@@ -247,15 +259,15 @@
 	* fixedLength: The length of the accepted answer, if different from zero.
 
 The returned value isn't case sensitive.
 
 ### Numbers
 
 ``` python
-CLIbrary.numIn(numberHandler={}) -> "int, float"
+CLIbrary.numIn(numberHandler: dict = {}) -> "int, float"
 ```
 
 *numIn* stands for *Number Input* as this function's purpose is receiving numeric inputs.
 
 The handler for this function makes use of the following parameters:
 * Strings.
 	* request: The prompt to the user.
@@ -267,30 +279,30 @@
 	* verbose.
 * Integers.
 	* round: The number of decimal to round to, if different from -1.
 
 ### Booleans
 
 ``` python
-CLIbrary.boolIn(boolHandler={}) -> bool
+CLIbrary.boolIn(boolHandler: dict = {}) -> bool
 ```
 
 *boolIn* stands for *Boolean Input* as this function's purpose is receiving boolean inputs.
 
 The handler for this function makes use of the following parameters:
 * Strings.
 	* request: The prompt to the user.
 	* added: A set of characters to be automatically added to the prompt.
 * Bools.
 	* verbose.
 
 ### Dates
 
 ``` python
-CLIbrary.dateIn(dateHandler={}) -> str
+CLIbrary.dateIn(dateHandler: dict = {}) -> str
 ```
 
 *dateIn* stands for *Date Input* as this function's purpose is receiving date[^4] inputs.
 
 The handler for this function makes use of the following parameters:
 * Strings.
 	* request: The prompt to the user.
@@ -300,15 +312,15 @@
 	* verbose.
 
 [^4]: Dates have to be passed in respect to the [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) standard. 
 
 ### List handling
 
 ``` python
-CLIbrary.listCh(listHandler={})
+CLIbrary.listCh(listHandler: dict = {})
 ```
 
 *listCh* stands for *List Choice* as this function returns the choosen element from a list.
 
 The handler for this function makes use of the following parameters:
 * Strings.
 	* request: The prompt to the user.
```

#### html2text {}

```diff
@@ -28,40 +28,48 @@
 is_a_dictionary_structured_as_{"option":_value}._Note_that,_although_every
 function_has_a_default_handler,_it_is_recommended_to_provide_at_least_some
 options_to_achieve_a_better_user_experience._###_Settings_As_of_version_1.2.1,
 CLIbrary_has_some_"global_options"_to_allow_even_more_personalization.
 Available_options_are:_1._`CLIbrary.style.setting_darkMode`,_bool:_Enables
 global_dark_mode._Dafault:_`False`._2._`CLIbrary.style.setting_plainMode`,
 bool:_Disables_styling._Default:_`False`._3.
-`CLIbrary.input.setting_caseSensitive`,_bool:_Enables_case-sensitiveness.
+`CLIbrary.style.setting_caseSensitive`,_bool:_Enables_case-sensitiveness.
 Default:_`False`._4._`CLIbrary.data.setting_fileExtension`,_str:_Defines_a_file
-extension_for_*CLIbrary.aDump*_and_*CLIbrary.aLoad*._Default:_`".pickle"`_###
-Import_CLIbrary_**CLIbrary**_can_be_installed_by:_python3_-m_pip_install_--
-upgrade_CLIbrary_verified_by:_python3_-m_CLIbrary_imported_by:_```_python
-import_CLIbrary_```_and_all_the_functions_can_be_accessed_by:_```_python
-CLIbrary.FUNCTION_NAME()_```_##_Interface_[Go_back_to_ToC](#table-of-contents)
-###_CLI_```_python_CLIbrary.cmdIn(commandHandler={})_->_dict_```_*cmdIn*_stands
-for_*Command_Input*_as_this_function_allows_the_user_to_input_command_as_in_a
-CLI_interface._The_handler_for_this_function_makes_use_of_the_following
-parameters:_*_request,_str:_The_prompt_to_the_user._*_added,_str:_A_set_of
-characters_to_be_automatically_added_to_the_prompt._Default_is_":_"._*_style,
-str[^1]:_A_particular_colour_style_to_be_applied_to_the_prompt._*_verbose,
-bool._*_allowedCommands,_list:_A_list_of_all_the_allowed_commands_for_the_CLI
-interface._*_helpPath,_str:_The_path_to_the_help_JSON._This_enables_the_*help*
-command._This_function_returns_a_dictionary_with_the_following_keys:_*_command,
-str:_The_command._*_sdOpts,_dict:_A_dictionary_containing_single-dash_options
-as_{"opts1":_"value1",_"opts2":_"value2",_...}[^2]._*_ddOpts,_list:_A_list
-containing_double-dash_options_as_[opts1,_opts2,_...][^2]._Commands_are_always
-structured_as:_command_-sdOpt_value_--ddOpt_with_no_more_than_a_single_word_for
-the_command_itself._[^1]:_Colorama_styling_works_best_for_styling_inside
-**CLIbrary**._[^2]:_The_options_get_returned_without_the_dashes._###_Option
-parser_```_python_CLIbrary.optionParser(instructions:_list)_->_None_```
-*optionParser*_is_a_function_that_receives_a_list_of_strings_and_returns_the
-single_dash_options_sdOpts,_a_dictionary,_and_the_double_dash_options,_a_list.
-###_Help_```_python_CLIbrary.helpPrint(handler={})_->_None_```_*helpPrint*_is_a
+extension_for_*CLIbrary.aDump*_and_*CLIbrary.aLoad*._Default:_`".pickle"`_5.
+`CLIbrary.commands.setting_enableCompletion`,_bool:_Enables_command_completion.
+Default:_`True`_###_Import_CLIbrary_**CLIbrary**_can_be_installed_by:_python3_-
+m_pip_install_--upgrade_CLIbrary_verified_by:_python3_-m_CLIbrary_imported_by:
+```_python_import_CLIbrary_```_and_all_the_functions_can_be_accessed_by:_```
+python_CLIbrary.FUNCTION_NAME()_```_##_Interface_[Go_back_to_ToC](#table-of-
+contents)_###_CLI_```_python_CLIbrary.cmdIn(commandHandler:_dict_=_{})_->_dict
+```_*cmdIn*_stands_for_*Command_Input*_as_this_function_allows_the_user_to
+input_command_as_in_a_CLI_interface._As_of_version_1.9.0,_CLIbrary_supports_tab
+completion_and_hinting_thanks_to_[cmdInput](#cmdinput)._The_handler_for_this
+function_makes_use_of_the_following_parameters:_*_request,_str:_The_prompt_to
+the_user._*_added,_str:_A_set_of_characters_to_be_automatically_added_to_the
+prompt._Default_is_":_"._*_style,_str[^1]:_A_particular_colour_style_to_be
+applied_to_the_prompt._*_verbose,_bool._*_allowedCommands,_list:_A_list_of_all
+the_allowed_commands_for_the_CLI_interface._*_helpPath,_str:_The_path_to_the
+help_JSON._This_enables_the_*help*_command._This_function_returns_a_dictionary
+with_the_following_keys:_*_command,_str:_The_command._*_sdOpts,_dict:_A
+dictionary_containing_single-dash_options_as_{"opts1":_"value1",_"opts2":
+"value2",_...}[^2]._*_ddOpts,_list:_A_list_containing_double-dash_options_as_
+[opts1,_opts2,_...][^2]._Commands_are_always_structured_as:_command_-sdOpt
+value_--ddOpt_with_no_more_than_a_single_word_for_the_command_itself._[^1]:
+Colorama_styling_works_best_for_styling_inside_**CLIbrary**._[^2]:_The_options
+get_returned_without_the_dashes._###_cmdInput_```_python
+CLIbrary.interface.cmdInput(handler:_dict)_->_None_```_*cmdInput*_is_cmdIn's
+alternative_to_Python's_input_which_allows_for_tab_completion_and_hinting.
+There's_no_need_to_call_this_function_manually_as_its_calls_are_embedded_inside
+*cmdIn*._###_Option_parser_```_python_CLIbrary.interface.optionParser
+(instructions:_list)_->_None_```_*optionParser*_is_a_function_that_receives_a
+list_of_strings_and_returns_the_single_dash_options_sdOpts,_a_dictionary,_and
+the_double_dash_options,_a_list._There's_no_need_to_call_this_function_manually
+as_its_calls_are_embedded_inside_*cmdIn*._###_Help_```_python
+CLIbrary.interface.helpPrint(handler:_dict)_->_None_```_*helpPrint*_is_a
 function_that_reads_and_print_the_help_JSON_whose_path_gets_passed_to_*cmdIn*.
 There's_no_need_to_call_this_function_manually_as_its_calls_are_embedded_inside
 *cmdIn*._###_Help_entries_A_help_entry_must_be_formatted_this_way:_```_json
 "command":_{_"description":_"Command_description.",_"options":_{"-sdOpt#":
 "VALUE_DESCRIPTION",_"-sdOpt":_"VALUE_DESCRIPTION",_"--ddOpt":_""}_}_```_where
 mandatory_options_get_identified_by_a_"#"_and_double-dash_options_don't_require
 a_value_description._This_is_an_example_from_**openBriefcase**'s_accounts_help
@@ -86,51 +94,52 @@
 following_parameters:_*_path,_str:_The_path_to_the_file._*_ignoreMissing,_bool:
 Whether_to_display_an_error_on_missing_files._###_Dumping_```_python
 CLIbrary.aDump(fileHandler:_dict)_->_None_```_*aDump*_stands_for_*Automatic
 Dumping*_as_this_function_dumps_informations_to_files_without_user
 confirmation._The_handler_for_this_function_makes_use_of_the_following
 parameters:_*_path,_str:_The_path_to_the_file._*_data:_The_data_to_be_dumped.
 ##_Inputs_[Go_back_to_ToC](#table-of-contents)_###_Strings_```_python
-CLIbrary.strIn(stringHandler={})_->_str_```_*strIn*_stands_for_*String_Input*
-as_this_function's_purpose_is_receiving_string_inputs._The_handler_for_this
-function_makes_use_of_the_following_parameters:_*_Strings._*_request:_The
+CLIbrary.strIn(stringHandler:_dict_=_{})_->_str_```_*strIn*_stands_for_*String
+Input*_as_this_function's_purpose_is_receiving_string_inputs._The_handler_for
+this_function_makes_use_of_the_following_parameters:_*_Strings._*_request:_The
 prompt_to_the_user._*_added:_A_set_of_characters_to_be_automatically_added_to
 the_prompt._*_Lists._*_allowedChars:_The_set_of_allowed_characters_which_aren't
 letters._*_allowedAnswers:_The_list_of_the_only_allowed_answers,_if_not_empty.
 *_blockedAnswers:_The_list_of_the_blocked_answers._*_Bools._*_empty:_Whether_to
 allow_or_not_empty_strings._*_space:_Whether_to_allow_or_not_the_use_of_spaces.
 *_verification:_Whether_to_ask_for_an_answer_verification._Useful_for
 passwords._*_verbose._*_Integers._*_fixedLength:_The_length_of_the_accepted
 answer,_if_different_from_zero._The_returned_value_isn't_case_sensitive._###
-Numbers_```_python_CLIbrary.numIn(numberHandler={})_->_"int,_float"_```_*numIn*
-stands_for_*Number_Input*_as_this_function's_purpose_is_receiving_numeric
-inputs._The_handler_for_this_function_makes_use_of_the_following_parameters:_*
-Strings._*_request:_The_prompt_to_the_user._*_added:_A_set_of_characters_to_be
-automatically_added_to_the_prompt._*_Strings._*_allowedRange:_The_range_in
-which_the_function_accepts_an_answer,_if_not_empty._*_allowedTypes:_Whether_to
-accept_just_integer_or_integer_and_floats._*_Bools._*_verbose._*_Integers._*
-round:_The_number_of_decimal_to_round_to,_if_different_from_-1._###_Booleans
-```_python_CLIbrary.boolIn(boolHandler={})_->_bool_```_*boolIn*_stands_for
-*Boolean_Input*_as_this_function's_purpose_is_receiving_boolean_inputs._The
-handler_for_this_function_makes_use_of_the_following_parameters:_*_Strings._*
-request:_The_prompt_to_the_user._*_added:_A_set_of_characters_to_be
-automatically_added_to_the_prompt._*_Bools._*_verbose._###_Dates_```_python
-CLIbrary.dateIn(dateHandler={})_->_str_```_*dateIn*_stands_for_*Date_Input*_as
-this_function's_purpose_is_receiving_date[^4]_inputs._The_handler_for_this
+Numbers_```_python_CLIbrary.numIn(numberHandler:_dict_=_{})_->_"int,_float"_```
+*numIn*_stands_for_*Number_Input*_as_this_function's_purpose_is_receiving
+numeric_inputs._The_handler_for_this_function_makes_use_of_the_following
+parameters:_*_Strings._*_request:_The_prompt_to_the_user._*_added:_A_set_of
+characters_to_be_automatically_added_to_the_prompt._*_Strings._*_allowedRange:
+The_range_in_which_the_function_accepts_an_answer,_if_not_empty._*
+allowedTypes:_Whether_to_accept_just_integer_or_integer_and_floats._*_Bools._*
+verbose._*_Integers._*_round:_The_number_of_decimal_to_round_to,_if_different
+from_-1._###_Booleans_```_python_CLIbrary.boolIn(boolHandler:_dict_=_{})_-
+>_bool_```_*boolIn*_stands_for_*Boolean_Input*_as_this_function's_purpose_is
+receiving_boolean_inputs._The_handler_for_this_function_makes_use_of_the
+following_parameters:_*_Strings._*_request:_The_prompt_to_the_user._*_added:_A
+set_of_characters_to_be_automatically_added_to_the_prompt._*_Bools._*_verbose.
+###_Dates_```_python_CLIbrary.dateIn(dateHandler:_dict_=_{})_->_str_```
+*dateIn*_stands_for_*Date_Input*_as_this_function's_purpose_is_receiving_date
+[^4]_inputs._The_handler_for_this_function_makes_use_of_the_following
+parameters:_*_Strings._*_request:_The_prompt_to_the_user._*_added:_A_set_of
+characters_to_be_automatically_added_to_the_prompt._*_Bools._*_placeholders:
+Enables_the_use_of_"x"s_as_placeholders_for_not_fully_known_dates._*_verbose._
+[^4]:_Dates_have_to_be_passed_in_respect_to_the_[ISO_8601](https://
+en.wikipedia.org/wiki/ISO_8601)_standard._###_List_handling_```_python
+CLIbrary.listCh(listHandler:_dict_=_{})_```_*listCh*_stands_for_*List_Choice*
+as_this_function_returns_the_choosen_element_from_a_list._The_handler_for_this
 function_makes_use_of_the_following_parameters:_*_Strings._*_request:_The
 prompt_to_the_user._*_added:_A_set_of_characters_to_be_automatically_added_to
-the_prompt._*_Bools._*_placeholders:_Enables_the_use_of_"x"s_as_placeholders
-for_not_fully_known_dates._*_verbose._[^4]:_Dates_have_to_be_passed_in_respect
-to_the_[ISO_8601](https://en.wikipedia.org/wiki/ISO_8601)_standard._###_List
-handling_```_python_CLIbrary.listCh(listHandler={})_```_*listCh*_stands_for
-*List_Choice*_as_this_function_returns_the_choosen_element_from_a_list._The
-handler_for_this_function_makes_use_of_the_following_parameters:_*_Strings._*
-request:_The_prompt_to_the_user._*_added:_A_set_of_characters_to_be
-automatically_added_to_the_prompt._*_Lists._*_list:_The_list_from_which_the
-element_gets_choosen._##_Outputs_[Go_back_to_ToC](#table-of-contents)_###
-Output_function_```_python_CLIbrary.output(outputHandler:_dict)_->_None_```_The
-handler_for_this_function_makes_use_of_the_following_parameters:_*_Strings._*
-string:_The_output_string._*_type:_The_output_type,_to_be_choosen_from:_*
-`"error"`,_*_`"warning"`,_*_`"verbose"`,_*_`""`:_A_plain_style,_similar_to_that
-of_`CLIbrary.style.setting_plainMode`._*_before:_A_string_that_gets_printed
-before_the_output_and_is_unaffected_by_the_output_styling._*_after:_A_string
-that_gets_printed_after_the_output_and_is_unaffected_by_the_output_styling._
+the_prompt._*_Lists._*_list:_The_list_from_which_the_element_gets_choosen._##
+Outputs_[Go_back_to_ToC](#table-of-contents)_###_Output_function_```_python
+CLIbrary.output(outputHandler:_dict)_->_None_```_The_handler_for_this_function
+makes_use_of_the_following_parameters:_*_Strings._*_string:_The_output_string.
+*_type:_The_output_type,_to_be_choosen_from:_*_`"error"`,_*_`"warning"`,_*
+`"verbose"`,_*_`""`:_A_plain_style,_similar_to_that_of
+`CLIbrary.style.setting_plainMode`._*_before:_A_string_that_gets_printed_before
+the_output_and_is_unaffected_by_the_output_styling._*_after:_A_string_that_gets
+printed_after_the_output_and_is_unaffected_by_the_output_styling._
```

### Comparing `clibrary-1.8.1/src/CLIbrary/__main__.py` & `clibrary-1.9.0/src/CLIbrary/__main__.py`

 * *Files identical despite different names*

### Comparing `clibrary-1.8.1/src/CLIbrary/files.py` & `clibrary-1.9.0/src/CLIbrary/files.py`

 * *Files identical despite different names*

### Comparing `clibrary-1.8.1/src/CLIbrary/inputs.py` & `clibrary-1.9.0/src/CLIbrary/inputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime
 
 from .outputs import *
 from .settings import style
 
 # INPUT HANDLING
 
-def strIn(stringHandler={}) -> str: # String input.	
+def strIn(stringHandler: dict = {}) -> str: # String input.	
 	handler = {}
 
 	# Strings.
 	handler["request"] = "String: " # The input request.
 	handler["added"] = ": " # The set of added characters to the input request.
 
 	# Lists.
@@ -136,15 +136,15 @@
 
 		except(EOFError, KeyboardInterrupt):
 			output({"type": "error", "string": "KEYBOARD ERROR"})
 		
 		except:
 			output({"type": "error", "string": "ERROR"})
 
-def dateIn(dateHandler={}) -> str: # Date input.
+def dateIn(dateHandler: dict = {}) -> str: # Date input.
 	handler = {}
 
 	# Strings.
 	handler["request"] = "Date"
 	handler["added"] = " [YYYY-MM-DD]: "
 
 	# Bools.
@@ -186,15 +186,15 @@
 			return answer
 		
 		except(ValueError):
 			pass
 		
 		output({"type": "error", "string": "DATE FORMAT ERROR"})
 
-def boolIn(boolHandler={}) -> bool: # Bool input.
+def boolIn(boolHandler: dict = {}) -> bool: # Bool input.
 	handler = {}
 
 	# Strings.
 	handler["request"] = "Bool"
 	handler["added"] = " [y/n]: "
 
 	# Bools.
@@ -225,15 +225,15 @@
 	
 	if answer == "y":
 		return True
 		
 	else:
 		return False
 
-def numIn(numberHandler={}) -> "int, float": # Number input.
+def numIn(numberHandler: dict = {}) -> "int, float": # Number input.
 	# Automatically recognizes wether the input is a float or an integer.
 
 	handler = {}
 
 	# Strings.
 	handler["request"] = "Number"
 	handler["added"] = ": "
@@ -314,15 +314,15 @@
 			output({"type": "error", "string": "KEYBOARD ERROR"})
 
 		except:
 			output({"type": "error", "string": "ERROR"})
 
 # LISTS HANDLING
 
-def listCh(listHandler={}): # List choice.
+def listCh(listHandler: dict = {}): # List choice.
 	handler = {}
 
 	# Strings.
 	handler["request"] = "List item"
 	handler["added"] = ": "
 
 	# Lists.
```

### Comparing `clibrary-1.8.1/src/CLIbrary/interface.py` & `clibrary-1.9.0/src/CLIbrary/interface.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from colorama import Fore, Back, Style
+from getkey import getkey, keys # cmdInput.
+import string
+import sys
 import json
 
 from .outputs import *
 
 # COMMANDS HANDLING
 
-def cmdIn(commandHandler={}) -> dict: # Command input.
+def cmdIn(commandHandler: dict = {}) -> dict: # Command input.
 	from .settings import style
-	
+
 	handler = {}
 	answer = {}
 
 	# Strings.
 	handler["request"] = "Command" # The input request.
 	handler["added"] = ": " # The set of added characters to the input request.
 	handler["style"] = "" # Prompt style.
@@ -51,15 +54,15 @@
 
 	# Plain style.
 	if style.setting_plainMode:
 		handler["style"] = ""
 
 	while True:
 		try:
-			rawAnswer = str(input(handler["style"] + handler["request"] + Style.RESET_ALL + handler["added"] + Style.RESET_ALL))
+			rawAnswer = cmdInput(handler)
 
 			if not style.setting_caseSensitive: # Case-sensitiveness.
 				rawAnswer = rawAnswer.lower()
 			
 			if handler["verbose"]:
 				output({"type": "verbose", "string": "VERBOSE, INPUT: " + rawAnswer})
 
@@ -75,29 +78,80 @@
 			if answer["command"] not in handler["allowedCommands"] and rawAnswer != "": # Checks the commands list.
 				output({"type": "error", "string": "UNKNOWN OR UNAVAILABLE COMMAND"})
 				continue
 
 			if answer["command"] == "help": # Prints the help.
 				helpPrint(handler)
 				continue
+
+			answer["sdOpts"], answer["ddOpts"] = optionsParser(instructions)
 		
 		except(IndexError):
 			output({"type": "error", "string": "SYNTAX ERROR"})
 			continue
 
 		except(EOFError, KeyboardInterrupt): # Handles keyboard interruptions.
 			output({"type": "error", "string": "KEYBOARD ERROR"})
 			continue
-			
-		answer["sdOpts"], answer["ddOpts"] = optionsParser(instructions)
+
 		return answer
 
 # UTILITIES
 
-def helpPrint(handler={}) -> None: # Prints the help.
+def cmdInput(handler: dict = {}) -> str:
+	from .settings import commands
+
+	buffer = ""
+
+	# Completion.
+	completion = ""
+
+	request = handler["style"] + handler["request"] + Style.RESET_ALL + handler["added"]
+	style = lambda string: Style.DIM + string.replace(" ".join(buffer.split()), "") + Style.RESET_ALL
+
+	sys.stdout.write(request)
+	sys.stdout.flush()
+
+	while True:
+		key = getkey()
+
+		# KEYS HANDLING.
+
+		if key == keys.ENTER:
+			print() # New line.
+			return " ".join(buffer.split())
+		
+		elif key in [keys.UP, keys.DOWN, keys.LEFT, keys.RIGHT]: # Ignores arrows.
+			continue
+		
+		elif key == keys.BACKSPACE: # handles deletion.
+			buffer = buffer[:-1]
+
+		elif key == keys.TAB and completion and commands.setting_enableCompletion: # Tab completion.
+			buffer = completion + " "
+
+		elif key in string.printable: # Adds the newly inserted character.
+			buffer += key
+
+		# COMPLETION HANDLING.
+
+		completion = ""
+		# Search for a possibile completion.
+		if " ".join(buffer.split()) != "" and len(" ".join(buffer.split()).split(" ")) == 1 and buffer[-1] != " " and commands.setting_enableCompletion:
+			# This works if the buffer is made of a single word and does not end with a space.
+			# This also checks for commands.setting_enableCompletion.
+			for command in handler["allowedCommands"]:
+				if command[0:len(" ".join(buffer.split()))] == " ".join(buffer.split()):
+					completion = command
+					break
+
+		sys.stdout.write("\x1b[2K\r" + request + buffer + style(completion))
+		sys.stdout.flush()
+
+def helpPrint(handler: dict) -> None: # Prints the help.
 	from .settings import style
 
 	try:
 		helpFile = open(handler["helpPath"], "r")
 		helpJson = json.load(helpFile)
 		helpFile.close()
```

### Comparing `clibrary-1.8.1/src/CLIbrary/outputs.py` & `clibrary-1.9.0/src/CLIbrary/outputs.py`

 * *Files identical despite different names*

### Comparing `clibrary-1.8.1/LICENSE` & `clibrary-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clibrary-1.8.1/README.md` & `clibrary-1.9.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # CLIbrary
 
 A comprehensive Python library of standard CLI utilities for convenient command, I/O, and file handling.  
-Make sure to take a look at the [documentation](https://github.com/diantonioandrea/CLIbrary/blob/main/docs/docs.md) and at the [contributing guidelines](https://github.com/diantonioandrea/CLIbrary/blob/main/.github/CONTRIBUTING.md).
+
+**CLIbrary** is a comprehensive Python library that makes command line usage, input/output, and file handling easier and more efficient. *It provides a wide range of tools for interacting with a shell*, including essential utilities for *command line parsing and I/O, file manipulations, tab completion, and command hinting*. With these tools, **CLIbrary** makes it easy to integrate powerful command-line functionality into any Python project.  
+
+Make sure to take a look at the [documentation](https://github.com/diantonioandrea/CLIbrary/blob/main/docs/docs.md), at the [contributing guidelines](https://github.com/diantonioandrea/CLIbrary/blob/main/.github/CONTRIBUTING.md) and at the [examples](#examples).
 
 ## Installation
 
 ### Installing CLIbrary
 
 **CLIbrary** can be installed from [PyPI](https://pypi.org) by:
 
@@ -15,15 +18,15 @@
 
 The installation of **CLIbrary** can be verified by:
 
 	python3 -m CLIbrary
 
 which would return something similar to[^1]:
 
-	●  CLIbrary v1.7.2 
+	 ●  CLIbrary v1.7.2 
 	A comprehensive Python library of standard CLI utilities for convenient command, I/O, and file handling.
 	Developed by Andrea Di Antonio, more on https://github.com/diantonioandrea/CLIbrary
 	Documentation on https://github.com/diantonioandrea/CLIbrary/blob/main/docs.md
 	Bug tracker on https://github.com/diantonioandrea/CLIbrary/issues
 
 [^1]: Example referring to version 1.7.2
```

### Comparing `clibrary-1.8.1/pyproject.toml` & `clibrary-1.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling", "colorama", "datetime", "setuptools"]
+requires = ["hatchling", "colorama", "datetime", "setuptools", "getkey"]
 build-backend = "hatchling.build"
 
 [project]
 name = "CLIbrary"
-version = "1.8.1"
+version = "1.9.0"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "A comprehensive Python library of standard CLI utilities for convenient command, I/O, and file handling."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `clibrary-1.8.1/PKG-INFO` & `clibrary-1.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CLIbrary
-Version: 1.8.1
+Version: 1.9.0
 Summary: A comprehensive Python library of standard CLI utilities for convenient command, I/O, and file handling.
 Project-URL: Homepage, https://github.com/diantonioandrea/CLIbrary
 Project-URL: Documentation, https://github.com/diantonioandrea/CLIbrary/blob/main/docs/docs.md
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/CLIbrary/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,15 +12,18 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # CLIbrary
 
 A comprehensive Python library of standard CLI utilities for convenient command, I/O, and file handling.  
-Make sure to take a look at the [documentation](https://github.com/diantonioandrea/CLIbrary/blob/main/docs/docs.md) and at the [contributing guidelines](https://github.com/diantonioandrea/CLIbrary/blob/main/.github/CONTRIBUTING.md).
+
+**CLIbrary** is a comprehensive Python library that makes command line usage, input/output, and file handling easier and more efficient. *It provides a wide range of tools for interacting with a shell*, including essential utilities for *command line parsing and I/O, file manipulations, tab completion, and command hinting*. With these tools, **CLIbrary** makes it easy to integrate powerful command-line functionality into any Python project.  
+
+Make sure to take a look at the [documentation](https://github.com/diantonioandrea/CLIbrary/blob/main/docs/docs.md), at the [contributing guidelines](https://github.com/diantonioandrea/CLIbrary/blob/main/.github/CONTRIBUTING.md) and at the [examples](#examples).
 
 ## Installation
 
 ### Installing CLIbrary
 
 **CLIbrary** can be installed from [PyPI](https://pypi.org) by:
 
@@ -30,15 +33,15 @@
 
 The installation of **CLIbrary** can be verified by:
 
 	python3 -m CLIbrary
 
 which would return something similar to[^1]:
 
-	●  CLIbrary v1.7.2 
+	 ●  CLIbrary v1.7.2 
 	A comprehensive Python library of standard CLI utilities for convenient command, I/O, and file handling.
 	Developed by Andrea Di Antonio, more on https://github.com/diantonioandrea/CLIbrary
 	Documentation on https://github.com/diantonioandrea/CLIbrary/blob/main/docs.md
 	Bug tracker on https://github.com/diantonioandrea/CLIbrary/issues
 
 [^1]: Example referring to version 1.7.2
```

