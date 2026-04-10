cmake_minimum_required(VERSION 4.3)
project(Threads)
string(JOIN "\n" EXT2
  "set(THREAD_PREFER_PTHREAD_FLAG ON)"
  "find_package(Threads REQUIRED BYPASS_PROVIDER)"
  ""
  )
xpExternPackage(BASE v0 XPDIFF "bin"
  WEB "https://cmake.org/cmake/help/latest/module/FindThreads.html"
  DESC "Finds and determines the thread library of the system for multithreading support"
  LICENSE "[LGPL-2.1-or-later](https://spdx.org/licenses/LGPL-2.1-or-later.html 'GNU Lesser General Public License v2.1 or later')"
  )
