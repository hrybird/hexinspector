# Process this file with automake to produce Makefile.in
## Copyright (c) 2010 Jen Freeman

## $Id$

## This program is free software; you can redistribute it and/or modify
## it under the terms of the GNU General Public License as published by
## the Free Software Foundation; either version 2 of the License, or
## (at your option) any later version.
##
## This program is distributed in the hope that it will be useful,
## but WITHOUT ANY WARRANTY; without even the implied warranty of
## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
## GNU General Public License for more details.
##
## You should have received a copy of the GNU General Public License along
## with this program; if not, write to the Free Software Foundation, Inc.,
## 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
##
## Author contact information:
##
## Web: http://github.com/jenf/hexinspector

AUTOMAKE_OPTIONS = foreign
noinst_LIBRARIES = libhi.a

libhi_a_SOURCES =  hi_file.c hi_buzhash.c hi_diff.c hi_search.c
libhi_a_CFLAGS = $(GLIB_CFLAGS) $(PCRE_CFLAGS)
bin_PROGRAMS = hi

hi_SOURCES = hi.c hi_ncurses_main.c hi_ncurses_file_pager.c hi_ncurses_highlight.c hi_ncurses_display.c \
	      hi_ncurses_location.c hi_ncurses_common.c hi_ncurses_help.c

hi_CFLAGS = $(GLIB_CFLAGS) $(PCRE_CFLAGS)
hi_LDADD = libhi.a $(GLIB_LIBS) $(NCURSES_LIBS) $(PCRE_LIBS)