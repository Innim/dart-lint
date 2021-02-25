## [0.1.8] - 2021-02-25

* Exclude generated code from analysis by default.

## [0.1.7+2] - 2021-02-04

* Readme: add information about disabling rules.

## [0.1.7+1] - 2021-01-29

* Disabled `use_setters_to_change_properties`: it's bad when we have only setter (without getter) and it has many false positive (for example in callbacks).

## [0.1.7] - 2021-01-28

* Enabled style rules: `use_full_hex_values_for_flutter_colors`, `use_is_even_rather_than_modulo`, `use_raw_strings`, `use_setters_to_change_properties`, `use_string_buffers`, `use_to_and_as_if_applicable`, `void_checks`, `package_names`, `sort_pub_dependencies`.

## [0.1.6+1] - 2021-01-02

* Temporary disabled rule `avoid_type_to_string`.

## [0.1.6] - 2021-01-02

* Enabled error rules: `avoid_print`, `avoid_returning_null_for_future`, `avoid_type_to_string`, `cancel_subscriptions`, 
`control_flow_in_finally`, `empty_statements`, `hash_and_equals`, `invariant_booleans`,
`iterable_contains_unrelated_type`, `list_remove_unrelated_type`, `literal_only_boolean_expressions`,
`no_adjacent_strings_in_list`, `no_logic_in_create_state`, `prefer_void_to_null`,
`test_types_in_equals`, `throw_in_finally`, `unnecessary_statements`, `unsafe_html`, `use_key_in_widget_constructors`.
* Enabled style rules: `unnecessary_overrides`, `unnecessary_parenthesis`, `unnecessary_raw_strings`, `unnecessary_string_escapes`,
`unnecessary_string_interpolations`.

## [0.1.5] - 2021-01-01

* Enabled rules: `sort_unnamed_constructors_first`, `type_annotate_public_apis`, `unnecessary_await_in_return`, 
`unnecessary_brace_in_string_interps`, `unnecessary_getters_setters`, `unnecessary_lambdas`, `unnecessary_null_aware_assignments`, 
`unnecessary_nullable_for_final_variable_declarations`.

## [0.1.4] - 2020-12-26

* Enabled rules: `prefer_inlined_adds`, `prefer_interpolation_to_compose_strings`, `prefer_is_not_operator`, `prefer_mixin`, 
`prefer_null_aware_operators`, `prefer_typing_uninitialized_variables`, `provide_deprecation_message`, `sized_box_for_whitespace`.

## [0.1.3+1] - 2020-12-23

* Disabled rule `prefer_if_elements_to_conditional_expressions`: it's not working well.
* Fix changelog.

## [0.1.3] - 2020-12-23

* Enabled rules: `only_throw_errors`, `overridden_fields`, `package_prefixed_library_names`, `parameter_assignments`, 
`prefer_asserts_in_initializer_lists`, `prefer_const_constructors`, `prefer_const_constructors_in_immutables`, 
`prefer_const_declarations`, `prefer_const_literals_to_create_immutables`, `prefer_final_in_for_each`,
`prefer_final_locals`, `prefer_function_declarations_over_variables`, `prefer_if_elements_to_conditional_expressions`,
`prefer_initializing_formals`.

## [0.1.2+1] - 2020-12-22

* Readme: Fix version shield.

## [0.1.2] - 2020-12-22

* Enabled rules: `exhaustive_cases`, `file_names`, `implementation_imports`, `join_return_with_assignment`,
`leading_newlines_in_multiline_strings`, `missing_whitespace_between_adjacent_strings`, `no_default_cases`,
`no_runtimeType_toString`, `non_constant_identifier_names`.

## [0.1.1+1] - 2020-12-11

* Update package desciption.

## [0.1.1] - 2020-12-11

* Add link for every rule.
* Enables rules: `avoid_web_libraries_in_flutter`, `avoid_bool_literals_in_conditional_expressions`, `avoid_catching_errors`, 
`avoid_escaping_inner_quotes`, `avoid_implementing_value_types`, `avoid_positional_boolean_parameters`, `avoid_renaming_method_parameters`, 
`avoid_returning_null_for_void`, `avoid_setters_without_getters`, `avoid_types_on_closure_parameters`, `avoid_unnecessary_containers`,
`avoid_unused_constructor_parameters`, `avoid_void_async`, `await_only_futures`, `camel_case_types`, `constant_identifier_names`,.

## [0.1.0] - 2020-12-09

* Main set of rules for analysis: based on pedantic.
* Strong mode.
* Changed some errors severity.
