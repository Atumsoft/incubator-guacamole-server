#
# Licensed to the Apache Software Foundation (ASF) under one
# or more contributor license agreements.  See the NOTICE file
# distributed with this work for additional information
# regarding copyright ownership.  The ASF licenses this file
# to you under the Apache License, Version 2.0 (the
# "License"); you may not use this file except in compliance
# with the License.  You may obtain a copy of the License at
#
#   http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing,
# software distributed under the License is distributed on an
# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
# KIND, either express or implied.  See the License for the
# specific language governing permissions and limitations
# under the License.
#

AUTOMAKE_OPTIONS = foreign
ACLOCAL_AMFLAGS = -I m4

noinst_LTLIBRARIES = libguac_common_ssh.la

libguac_common_ssh_la_SOURCES = \
    guac_sftp.c                 \
    guac_ssh.c                  \
    guac_ssh_buffer.c           \
    guac_ssh_key.c              \
    guac_ssh_user.c

noinst_HEADERS =      \
    guac_sftp.h       \
    guac_ssh.h        \
    guac_ssh_buffer.h \
    guac_ssh_key.h    \
    guac_ssh_user.h

libguac_common_ssh_la_CFLAGS = \
    -Werror -Wall -pedantic    \
    @COMMON_INCLUDE@           \
    @LIBGUAC_INCLUDE@

libguac_common_ssh_la_LIBADD = \
    @LIBGUAC_LTLIB@

libguac_common_ssh_la_LDFLAGS = \
    @PTHREAD_LIBS@              \
    @SSH_LIBS@                  \
    @SSL_LIBS@

