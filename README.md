# sift

A fast and powerful open source alternative to grep.

Please go to [sift-tool.org](https://sift-tool.org) for more information.

## libliflin fork: siftweb. 

super rudimentary, single threaded, kinda broken, sift as a web form. 

1. global lock. 
2. output doesn't do line printing quite right.
3. doesn't use cgo because mingw 64 installer just gives me a windows error on windows server 2012
4. But it is a website?


`go get github.com/libliflin/sift/siftweb`

    Usage of siftweb:
      -dir string
            Directory. The directory in which to search.
      -f string
            From. The server listen address. E.g. http://localhost:8000.

or as I do:

`go build && siftweb -f http://localhost:9090 -dir .`

I just copied sift code into /siftweb and changed it's main to be a http server.

## License

Copyright (C) 2014-2016 Sven Taute

libliflin modifications: Copyright 2016 William Laffin

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, version 3 of the License.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.

