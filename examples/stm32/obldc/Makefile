##
## This file is part of the libopencm3 project.
##
## Copyright (C) 2010 Piotr Esden-Tempski <piotr@esden.net>
##
## This program is free software: you can redistribute it and/or modify
## it under the terms of the GNU General Public License as published by
## the Free Software Foundation, either version 3 of the License, or
## (at your option) any later version.
##
## This program is distributed in the hope that it will be useful,
## but WITHOUT ANY WARRANTY; without even the implied warranty of
## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
## GNU General Public License for more details.
##
## You should have received a copy of the GNU General Public License
## along with this program.  If not, see <http://www.gnu.org/licenses/>.
##

# Be silent per default, but 'make V=1' will show all compiler calls.
ifneq ($(V),1)
Q := @
# Do not print "Entering directory ...".
MAKEFLAGS += --no-print-directory
endif

all: led systick usart can

led:
	@printf "  BUILD   examples/stm32/obldc/led\n"
	$(Q)$(MAKE) -C led

systick:
	@printf "  BUILD   examples/stm32/obldc/systick\n"
	$(Q)$(MAKE) -C systick

usart:
	@printf "  BUILD   examples/stm32/obldc/usart\n"
	$(Q)$(MAKE) -C usart

can:
	@printf "  BUILD   examples/stm32/obldc/can\n"
	$(Q)$(MAKE) -C can

clean:
	@printf "  CLEAN   examples/stm32/obldc/led\n"
	$(Q)$(MAKE) -C led clean
	@printf "  CLEAN   examples/stm32/obldc/systick\n"
	$(Q)$(MAKE) -C systick clean
	@printf "  CLEAN   examples/stm32/obldc/usart\n"
	$(Q)$(MAKE) -C usart clean
	@printf "  CLEAN   examples/stm32/obldc/can\n"
	$(Q)$(MAKE) -C can clean

.PHONY: led systick usart can

