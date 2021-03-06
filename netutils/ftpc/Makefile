############################################################################
# apps/netutils/ftpc/Makefile
#
#   Copyright (C) 2011-2012 Gregory Nutt. All rights reserved.
#   Author: Gregory Nutt <gnutt@nuttx.org>
#
# Redistribution and use in source and binary forms, with or without
# modification, are permitted provided that the following conditions
# are met:
#
# 1. Redistributions of source code must retain the above copyright
#    notice, this list of conditions and the following disclaimer.
# 2. Redistributions in binary form must reproduce the above copyright
#    notice, this list of conditions and the following disclaimer in
#    the documentation and/or other materials provided with the
#    distribution.
# 3. Neither the name NuttX nor the names of its contributors may be
#    used to endorse or promote products derived from this software
#    without specific prior written permission.
#
# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
# FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
# COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
# INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS
# OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED
# AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
# ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
# POSSIBILITY OF SUCH DAMAGE.
#
############################################################################

include $(APPDIR)/Make.defs

ifeq ($(CONFIG_NET_TCP),y)
# FTP connection management
CSRCS += ftpc_connect.c ftpc_disconnect.c

# FTP commands
CSRCS += ftpc_cdup.c ftpc_chdir.c ftpc_chmod.c ftpc_filesize.c ftpc_filetime.c
CSRCS += ftpc_help.c ftpc_idle.c ftpc_listdir.c ftpc_login.c ftpc_mkdir.c
CSRCS += ftpc_noop.c ftpc_rpwd.c ftpc_quit.c ftpc_rename.c ftpc_rmdir.c ftpc_unlink.c
CSRCS += ftpc_cmd.c

# FTP transfers
CSRCS += ftpc_getfile.c ftpc_putfile.c ftpc_transfer.c

# FTP responses
CSRCS += ftpc_response.c ftpc_getreply.c

# FTP helpers
CSRCS += ftpc_utils.c ftpc_socket.c
endif

include $(APPDIR)/Application.mk
