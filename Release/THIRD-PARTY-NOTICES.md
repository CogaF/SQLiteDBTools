# Third-party notices

SQLite DB Tools is free of charge, its source code private (see [LICENSE.md](LICENSE.md)). It includes or links the
following third-party components, each under its own licence. These notices must be shipped with
every distributed copy of the application (the build copies this file next to the exe; the same
texts are shown in Help > About > Third-party notices). The full licence texts are in the folder
`licenses` next to the exe (`licenses/README.txt` says which file belongs to which component).

- wxWidgets
  - Licence: wxWindows Library Licence 3.1
  - Used for: the user interface
  - Source: https://www.wxwidgets.org/

- SQLite
  - Licence: Public domain
  - Used for: the database engine (SQLite is a registered trademark of Hipp, Wyrick & Company, Inc.)
  - Source: https://www.sqlite.org/

- SQLite3 Multiple Ciphers
  - Licence: MIT
  - Used for: encrypted databases
  - Source: https://github.com/utelle/SQLite3MultipleCiphers

- libsodium
  - Licence: ISC
  - Used for: key derivation and key wrapping of the protected databases
  - Source: https://libsodium.org/

- PoDoFo (and the components it bundles, listed below)
  - Licence: GNU LGPL 2.0 or later, or Mozilla Public License 2.0 (dual licence): used under the MPL 2.0
  - Used for: the PDF documents and reports
  - Source: https://github.com/podofo/podofo

- OpenSSL (linked into PoDoFo)
  - Licence: Apache License 2.0
  - Used for: needed by PoDoFo
  - Source: https://www.openssl.org/

- FreeType (linked into PoDoFo)
  - Licence: FreeType Licence (FTL)
  - Used for: fonts in the PDF
  - Source: https://freetype.org/

- libxml2, Fontconfig, Little CMS (linked into PoDoFo)
  - Licence: MIT
  - Used for: needed by PoDoFo
  - Source: https://gitlab.gnome.org/GNOME/libxml2, https://www.freedesktop.org/wiki/Software/fontconfig/, https://www.littlecms.com/

- zlib, libpng, libjpeg, libtiff (linked into PoDoFo)
  - Licence: zlib, libpng, IJG, libtiff licences (permissive)
  - Used for: images in the PDF
  - Source: https://zlib.net/, http://www.libpng.org/, https://ijg.org/, https://libtiff.gitlab.io/libtiff/

## wxWidgets - wxWindows Library Licence, Version 3.1

Copyright (c) 1998-2005 Julian Smart, Robert Roebling et al.

The wxWindows Library Licence is the GNU LGPL with an exception that explicitly allows distributing
applications that link wxWidgets (statically or dynamically) in binary form under the user's own
terms. Full text: `licenses/wxWindows-Library-Licence-3.1.txt` (and `licenses/LGPL-2.0.txt`), also at
<https://www.wxwidgets.org/about/licence/>.

## SQLite - public domain

The author disclaims copyright to the SQLite source code. In place of a legal notice, here is a
blessing: May you do good and not evil. May you find forgiveness for yourself and forgive others.
May you share freely, never taking more than you give. <https://www.sqlite.org/copyright.html>

## SQLite3 Multiple Ciphers - MIT

Copyright (c) 2019-2025 Ulrich Telle and contributors.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
associated documentation files (the "Software"), to deal in the Software without restriction,
including without limitation the rights to use, copy, modify, merge, publish, distribute,
sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions: The above copyright notice and this
permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN
NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## libsodium - ISC

Copyright (c) 2013-2025 Frank Denis <j at pureftpd dot org>

Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee
is hereby granted, provided that the above copyright notice and this permission notice appear in all
copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE
INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE
FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION,
ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.

## PoDoFo - LGPL 2.0+ / MPL 2.0, used under the MPL 2.0

PoDoFo, Copyright (C) the PoDoFo authors (<https://github.com/podofo/podofo>), is used **unmodified** under the
**Mozilla Public License 2.0** (full text: `licenses/MPL-2.0.txt`; PoDoFo's own notice: `licenses/PoDoFo-NOTICE.txt`).

- **Which version:** the one shown in Help > About > Dependencies.
- **Its source code (MPL 2.0, section 3.2):** the release of that version at <https://github.com/podofo/podofo/releases>,
  unmodified. A copy is also available on request from the author of this program, for at least as long as this version is
  distributed.
- **This program is a "Larger Work" (MPL 2.0, section 3.3):** its own code is not PoDoFo's and stays under its own licence
  (LICENSE.md). Nothing in LICENSE.md limits the rights the MPL 2.0 gives over PoDoFo itself.
- If PoDoFo is ever modified, the modified files are published under the MPL 2.0 together with the program that uses them.

(If the LGPL is chosen instead, a statically linked exe must be distributed so that the user can relink it with another
PoDoFo - the `_DLL` configurations, with `podofo.dll` next to the exe, satisfy that directly. This program does not choose it.)

### Components bundled in PoDoFo

PoDoFo compiles these into itself (its NOTICE file); their notices travel with it:

- **SASLprep**
  - Copyright: (c) 2025 Francesco Pretto
  - Licence: MIT
  - Full text: `licenses/MIT-PoDoFo-components.txt`

- **Adobe Font Development Kit for OpenType (AFDKO; when PoDoFo is built with `PODOFO_WITH_AFDKO`, the default)**
  - Copyright: (c) 2014-2021 Adobe
  - Licence: Apache License 2.0
  - Full text: `licenses/AFDKO-Apache-2.0.txt`, `licenses/Apache-2.0.txt`

- **Google PDFium (parts)**
  - Copyright: (c) 2014-2017 The PDFium Authors
  - Licence: Apache License 2.0 and BSD 3-clause
  - Full text: `licenses/PDFium-BSD-3-Clause.txt`, `licenses/Apache-2.0.txt`

- **Chromium Numerics**
  - Copyright: (c) 2017-2021 The Chromium Authors
  - Licence: BSD 3-clause
  - Full text: `licenses/Chromium-Numerics-BSD-3-Clause.txt`

- **Liberation Fonts**
  - Copyright: (c) 2010 Google Corporation (Arimo, Tinos, Cousine); (c) 2012 Red Hat, Inc. (Liberation)
  - Licence: SIL Open Font License 1.1
  - Full text: `licenses/OFL-1.1-Liberation-Fonts.txt`

- **tcb-span**
  - Copyright: (c) Tristan Brindle 2018
  - Licence: Boost Software License 1.0
  - Full text: `licenses/BSL-1.0.txt`

- **fast_float**
  - Copyright: (c) 2021 The fast_float authors
  - Licence: Apache 2.0 / MIT / Boost 1.0 (used under MIT)
  - Full text: `licenses/MIT-PoDoFo-components.txt`

- **fmt**
  - Copyright: (c) 2012 - present, Victor Zverovich
  - Licence: MIT
  - Full text: `licenses/MIT-PoDoFo-components.txt`

- **Howard Hinnant's date**
  - Copyright: (c) 2015-2019 Howard Hinnant et al.
  - Licence: MIT
  - Full text: `licenses/MIT-PoDoFo-components.txt`

- **utf8proc**
  - Copyright: (c) 2014-2021 Steven G. Johnson, Jiahao Chen and contributors; (c) 2009 Public Software Group e. V.
  - Licence: MIT
  - Full text: `licenses/MIT-PoDoFo-components.txt`

- **utf8cpp**
  - Copyright: (c) 2006 Nemanja Trifunovic
  - Licence: Boost Software License 1.0
  - Full text: `licenses/BSL-1.0.txt`

## OpenSSL - Apache License 2.0

This product includes software developed by the OpenSSL Project for use in the OpenSSL Toolkit
(<https://www.openssl.org/>). Licensed under the Apache License 2.0 (`licenses/Apache-2.0.txt`,
`licenses/OpenSSL-Apache-2.0.txt`).

## FreeType

Portions of this software are copyright (C) The FreeType Project (<https://freetype.org>). All rights
reserved. Used under the FreeType Licence (FTL, `licenses/FreeType-FTL.txt`).

## libxml2, Fontconfig, Little CMS, zlib, libpng, libjpeg, libtiff

Used under their permissive licences (MIT, zlib, libpng, IJG and libtiff licences), which allow use
in proprietary software provided their copyright notices are retained: each one's copyright and full
licence in `licenses/` (`libxml2-MIT.txt`, `Fontconfig.txt`, `LittleCMS-MIT.txt`, `zlib.txt`, `libpng.txt`,
`libjpeg-IJG.txt`, `libtiff.txt`). This software is based in part on the work of the Independent JPEG Group.

The Android app builds PoDoFo with libjpeg-turbo in place of libjpeg: (c) 2009-2024 D. R. Commander and others, under the
IJG licence and the Modified (3-clause) BSD licence (`licenses/libjpeg-turbo-BSD-3-Clause.txt`, `licenses/libjpeg-IJG.txt`).

## Microsoft Visual C++ runtime

Linked into the program and redistributed under the Visual Studio license terms (Visual C++ Redistributable).
Microsoft, Windows and Visual Studio are trademarks of the Microsoft group of companies.
