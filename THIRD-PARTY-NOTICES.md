# Third-party notices

SQLite DB Tools is free of charge, its source code private (see [LICENSE.md](LICENSE.md)). It includes or links the
following third-party components, each under its own licence. These notices must be shipped with
every distributed copy of the application (the build copies this file next to the exe; the same
texts are shown in Help > About > Third-party notices).

| Component | Licence | Used for | Source |
|---|---|---|---|
| wxWidgets | wxWindows Library Licence 3.1 | the user interface | <https://www.wxwidgets.org/> |
| SQLite | Public domain | the database engine (SQLite is a registered trademark of Hipp, Wyrick & Company, Inc.) | <https://www.sqlite.org/> |
| SQLite3 Multiple Ciphers | MIT | encrypted databases | <https://github.com/utelle/SQLite3MultipleCiphers> |
| libsodium | ISC | key derivation and key wrapping of the protected databases | <https://libsodium.org/> |
| PoDoFo | GNU LGPL 2.0 or later, or Mozilla Public License 2.0 (dual licence) | the PDF documents and reports | <https://github.com/podofo/podofo> |
| OpenSSL (linked into PoDoFo) | Apache License 2.0 | - (needed by PoDoFo) | <https://www.openssl.org/> |
| FreeType (linked into PoDoFo) | FreeType Licence (FTL) | fonts in the PDF | <https://freetype.org/> |
| libxml2, Fontconfig, Little CMS (linked into PoDoFo) | MIT | - (needed by PoDoFo) | <https://gitlab.gnome.org/GNOME/libxml2>, <https://www.freedesktop.org/wiki/Software/fontconfig/>, <https://www.littlecms.com/> |
| zlib, libpng, libjpeg, libtiff (linked into PoDoFo) | zlib, libpng, IJG, libtiff licences (permissive) | images in the PDF | <https://zlib.net/>, <http://www.libpng.org/>, <https://ijg.org/>, <https://libtiff.gitlab.io/libtiff/> |

## wxWidgets - wxWindows Library Licence, Version 3.1

Copyright (c) 1998-2005 Julian Smart, Robert Roebling et al.

The wxWindows Library Licence is the GNU LGPL with an exception that explicitly allows distributing
applications that link wxWidgets (statically or dynamically) in binary form under the user's own
terms. Full text: <https://www.wxwidgets.org/about/licence/>.

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

## PoDoFo - LGPL 2.0+ / MPL 2.0

PoDoFo, Copyright (C) the PoDoFo authors, is used under the **Mozilla Public License 2.0**
(<https://www.mozilla.org/MPL/2.0/>). Under the MPL the application may link PoDoFo statically or
dynamically; the PoDoFo source code - unmodified - is available at <https://github.com/podofo/podofo>.
If PoDoFo is modified, those modified files must be made available under the MPL 2.0.

(If the LGPL is chosen instead, a statically linked exe must be distributed so that the user can
relink it with another PoDoFo - the `_DLL` configurations, with `podofo.dll` next to the exe,
satisfy that directly.)

## OpenSSL - Apache License 2.0

This product includes software developed by the OpenSSL Project for use in the OpenSSL Toolkit
(<https://www.openssl.org/>). Licensed under the Apache License 2.0:
<https://www.apache.org/licenses/LICENSE-2.0>.

## FreeType

Portions of this software are copyright (C) The FreeType Project (<https://freetype.org>). All rights
reserved. Used under the FreeType Licence (FTL).

## libxml2, Fontconfig, Little CMS, zlib, libpng, libjpeg, libtiff

Used under their permissive licences (MIT, zlib, libpng, IJG and libtiff licences), which allow use
in proprietary software provided their copyright notices are retained. This software is based in
part on the work of the Independent JPEG Group.

## Microsoft Visual C++ runtime

Linked into the program and redistributed under the Visual Studio license terms (Visual C++ Redistributable).
Microsoft, Windows and Visual Studio are trademarks of the Microsoft group of companies.
