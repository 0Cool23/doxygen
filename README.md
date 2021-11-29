## Doxygen submodule documentation {#PAGE_SolutionDoxygen}

## Using Doxygen

### LicenseInfo {#SEC_SolutionDoxygen_LicenseInfo}

#### Preparing solution for licenses

Copy the file `dox\doxygen\licenses.dox` to the directory `dox` and include it
as existing solution item to the `dox`directory. Then edit the file and remove
the <i>\@cond</i> and <i>\@endcond</i> doxygen tags.

#### Adding and adjusting a license for a project

Choose a sutible license file from the `dox/doxygen/licenses` directory and
copy the file into the root directory of your project (e.g. `license-lgpl2.1.md`).

Next adjust the license original file header

```
### Library (LGPL v2.1) {#LIBRARY_PROJECT_LGPL_2_1}

Library - short description.

    Copyright (C) 2021
....
```

with information to match your project by adjusting title, doxygen reference and
description.


```
### libId3Buffer Library (LGPL v2.1) {#LIBRARY_LIBID3BUFFER_LGPL_2_1}

liId3Buffer - Library to analyse and modify music files header information.

    Copyright (C) 2021
....
```

Now add the license reference `LIBRARY_LIBID3BUFFER_LGPL_2_1`  to a section
in the `dox\license.dox` file.

```
....
@section SEC_LIBRARIES Libraries
<!-- @subpage LIBRARY_PROJECT_LGPL_2_1 -->
@subpage LIBRARY_LIBID3BUFFER_LGPL_2_1
....
```
