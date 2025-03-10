[0.1.0a]

- core functionalities, including build and batch methods

[0.2.0a]

- handling of all pydantic constraint

[0.3.0b]

- full features MvP

[0.3.1b]

- fix issues with decimal parsing

[0.3.2b]

- removed support for python 3.6
- added beanie extension

[0.3.3b]

- resolve TypeError being raised from issubclass() for python 3.9+

[0.3.4b]

- add support for forward refs
- add support for ODMantic
- add Ignore and Require fields

[0.3.5b]

- update readme
- update fields

[0.4.0]

- added support for dataclasses

[0.4.1]

- randomly return None values for Optional[] marked fields

[0.4.2]

- updated handling of dataclasses to support randomized optionals

[0.4.3]

- fixed `py.typed` not placed inside the package

[0.4.4]

- make exports explicit

[0.4.5]

- fix generation of enum in complex types

[0.4.6]

- fix generation of nested constrained fields

[0.5.0]

- add ormar extension


[0.6.0]

- added `__allow_none_optionals__` factory class variable
- updated the `ModelFactory.create_factory` method to accept an optional `base` kwarg user defined **kwargs
- added a new method on `ModelFactory` called `should_set_none_value`, which dictates whether a None value should be set for a given `ModelField`
- updated dependencies


[0.6.1]

- fix bug were nested optionals did not factor in `__allow_none_optionals__` settings


[0.6.2]

- fix bug with Literal[] values not being recognized


[0.6.3]

- fix backwards compatible import


[0.7.0]

- added support for `factory_use_construct` kwargs, thanks - @danielkatzan


[0.8.0]

- added random configuration. Thanks to @eviltnan


[1.0.0]

- updated to support pydantic 1.9.0, including all new types


[1.1.0]

- resolve compatibilities issues with pydantic 1.8.2
- add support for constrained frozenset


[1.2.0]

- fix factory typing and resolve issue with TypeVars not being bounded, @lindycoder
- add support for naive classes (including all builtin exceptions)
- fix the `create_model_factory` method to use the current `cls` as the created factory's base by default


[1.2.1]

- suppress NameError that can occur when calling `update_forward_refs` without access to a localNS


[1.2.2]

- added `Any` to Providers


[1.2.3]

- fixed regression due to lambda function argument

[1.2.4]

- updated dependencies


[1.2.5]

- fix handling of choice for ormar extension @mciszczon
- fix handling of FKs for ormar extension


[1.2.6]

- fix handling of decimal mac length @DaanRademaker
