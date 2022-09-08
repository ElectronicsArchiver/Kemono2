
# Development Mode

This mode provides a way to create a dev environment <br>
from scratch for ease of development and testing.

<br>
<br>

## Location

Development-only files live in their `development` folder, <br>
located in the root of a project, which exposes its own <br>
exported modules in its index file.

Only exports declared within are allowed to be imported <br>
outside and only do it conditionally by checking for the <br>
presence of development environment variable beforehand.

The folder structure follows the same logic as the `src` <br>
folder, in that it can have its own `lib`, `endpoints`, <br>
`types` and even `internals` folders.

The server also provides the `/development` <br>
endpoint, giving access to various features.

<br>
<br>

## Features

<br>

### Test Entries

Test entries can be generated with <br>
the following two mechanisms.

<br>

#### Seeded

Uses a seed to generate the same result with <br>
each use, it thus should error on the second use.

*It is used to populate the initial test database.*

<br>

#### Random

Creates random new entries regardless of circumstances.

*Used to add random entries in any table during development.*

<br>
<br>

## Issues

<br>

-   Due to some underlying changes of the <br>
    importing process the test import does <br>
    not work.

<br>
