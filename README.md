**Deprectated and no longer supported**

1) About.

2) Licence. All Yandex code in this distribution is under following licence:

----------------------------------------------------------
Copyright (c) 2012 Yandex

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

----------------------------------------------------------

Some libraries in this distribution is under GPLv2/v3, so you can use Yandex code also with GPLv2/GPLv3.
See http://www.gnu.org/copyleft/gpl.html

3) Install instructions.
 * checkout balancer
 * mkdir build
   cd build
   cmake -DMAKE_ONLY=web/httpd/server -DCMAKE_BUILD_TYPE=release ../balancer
   make -j 2
 * optionally you can create local.cmake in build/, with some interesting options:
   SET(MY_GCC gcc46)
   SET(MY_GPP g++46)
   SET(USE_STATIC_CPP_RUNTIME no), for disabling static linkage of c++ runtime(libsupc++)

