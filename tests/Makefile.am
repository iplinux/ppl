# Automake source file for the Parma Polyhedra Library.
# Copyright (C) 2001-2009 Roberto Bagnara <bagnara@cs.unipr.it>
#
# This file is part of the Parma Polyhedra Library (PPL).
#
# The PPL is free software; you can redistribute it and/or modify it
# under the terms of the GNU General Public License as published by the
# Free Software Foundation; either version 3 of the License, or (at your
# option) any later version.
#
# The PPL is distributed in the hope that it will be useful, but WITHOUT
# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
# FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License
# for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program; if not, write to the Free Software Foundation,
# Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02111-1307, USA.
#
# For the most up-to-date information see the Parma Polyhedra Library
# site: http://www.cs.unipr.it/ppl/ .

SUBDIRS = \
. \
Powerset \
Partially_Reduced_Product \
Box \
MIP_Problem \
Octagonal_Shape \
BD_Shape \
Polyhedron \
Grid
#Ask_Tell

AM_CPPFLAGS = -I$(top_builddir)/src -I$(top_srcdir)/src @extra_includes@

check_LIBRARIES = libppl_tests.a

libppl_tests_a_SOURCES = \
files.hh \
files.cc \
ppl_test.cc \
Partial_Function.cc

LDADD = \
$(top_builddir)/src/libppl.la \
libppl_tests.a \
@extra_libraries@

noinst_HEADERS = \
ppl_test.hh \
Partial_Function.defs.hh \
Partial_Function.inlines.hh \
Partial_Function.types.hh \
Random_Number_Generator.defs.hh \
Random_Number_Generator.inlines.hh \
Random_Number_Generator.types.hh

EXTRA_DIST = valgrind_suppressions
