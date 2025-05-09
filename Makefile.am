include $(top_srcdir)/doxygen-include.am

ACLOCAL_AMFLAGS = -I m4

MOSTLYCLEANFILES = $(DX_CLEANFILES)

POSIX_C_SOURCE=200809L

EXTRA_DIST = \
	bootstrap \
	ChangeLog \
	COPYING \
	doc \
	README.md \
	src/libbluray/bdj/build.xml \
	src/libbluray/bdj/java \
	src/libbluray/bdj/java-build-support \
	src/libbluray/bdj/java-j2me \
	src/libbluray/bdj/java-j2se \
	contrib/asm

AM_CFLAGS = \
	-std=c99

AM_CPPFLAGS = \
	-D_ISOC99_SOURCE \
	-D_POSIX_C_SOURCE=$(POSIX_C_SOURCE) \
	-D_REENTRANT \
	\
	-I$(top_srcdir)/src \
	-I$(top_srcdir)/src/libbluray

lib_LTLIBRARIES=libbluray.la
libbluray_la_CPPFLAGS = \
	$(AM_CPPFLAGS) \
	-I$(top_builddir)/src/libbluray \
	$(BDJAVA_CFLAGS) \
	-I${top_srcdir}/contrib/libudfread/src/ \
	$(LIBXML2_CFLAGS) \
	$(FT2_CFLAGS) \
	$(LIBUDFREAD_CFLAGS) \
	$(FONTCONFIG_CFLAGS)
libbluray_la_SOURCES = \
	src/file/dirs.h \
	src/file/dl.h \
	src/file/file.h \
	src/file/file.c \
	src/file/filesystem.h \
	src/file/filesystem.c \
	src/file/mount.h \
	src/libbluray/bluray.h \
	src/libbluray/bluray.c \
	src/libbluray/bluray_internal.h \
	src/libbluray/bluray-version.h \
	src/libbluray/keys.h \
	src/libbluray/player_settings.h \
	src/libbluray/register.h \
	src/libbluray/register.c \
	src/libbluray/bdnav/bdid_parse.h \
	src/libbluray/bdnav/bdid_parse.c \
	src/libbluray/bdnav/bdmv_parse.h \
	src/libbluray/bdnav/bdmv_parse.c \
	src/libbluray/bdnav/bdparse.h \
	src/libbluray/bdnav/clpi_parse.c \
	src/libbluray/bdnav/clpi_parse.h \
	src/libbluray/bdnav/extdata_parse.h \
	src/libbluray/bdnav/extdata_parse.c \
	src/libbluray/bdnav/index_parse.h \
	src/libbluray/bdnav/index_parse.c \
	src/libbluray/bdnav/meta_data.h \
	src/libbluray/bdnav/meta_parse.h \
	src/libbluray/bdnav/meta_parse.c \
	src/libbluray/bdnav/mpls_parse.h \
	src/libbluray/bdnav/mpls_data.h \
	src/libbluray/bdnav/mpls_parse.c \
	src/libbluray/bdnav/navigation.h \
	src/libbluray/bdnav/navigation.c \
	src/libbluray/bdnav/sound_parse.h \
	src/libbluray/bdnav/sound_parse.c \
	src/libbluray/bdnav/uo_mask.h \
	src/libbluray/bdnav/uo_mask.c \
	src/libbluray/bdnav/uo_mask_table.h \
	src/libbluray/decoders/graphics_controller.h \
	src/libbluray/decoders/graphics_controller.c \
	src/libbluray/decoders/graphics_processor.h \
	src/libbluray/decoders/graphics_processor.c \
	src/libbluray/decoders/hdmv_pids.h \
	src/libbluray/decoders/ig.h \
	src/libbluray/decoders/ig_decode.h \
	src/libbluray/decoders/ig_decode.c \
	src/libbluray/decoders/m2ts_demux.h \
	src/libbluray/decoders/m2ts_demux.c \
	src/libbluray/decoders/m2ts_filter.h \
	src/libbluray/decoders/m2ts_filter.c \
	src/libbluray/decoders/overlay.h \
	src/libbluray/decoders/pg.h \
	src/libbluray/decoders/pg_decode.h \
	src/libbluray/decoders/pg_decode.c \
	src/libbluray/decoders/pes_buffer.h \
	src/libbluray/decoders/pes_buffer.c \
	src/libbluray/decoders/rle.h \
	src/libbluray/decoders/rle.c \
	src/libbluray/decoders/textst.h \
	src/libbluray/decoders/textst_decode.h \
	src/libbluray/decoders/textst_decode.c \
	src/libbluray/decoders/textst_render.h \
	src/libbluray/decoders/textst_render.c \
	src/libbluray/disc/aacs.h \
	src/libbluray/disc/aacs.c \
	src/libbluray/disc/bdplus.h \
	src/libbluray/disc/bdplus.c \
	src/libbluray/disc/dec.h \
	src/libbluray/disc/dec.c \
	src/libbluray/disc/disc.h \
	src/libbluray/disc/disc.c \
	src/libbluray/disc/enc_info.h \
	src/libbluray/disc/properties.h \
	src/libbluray/disc/properties.c \
	src/libbluray/hdmv/hdmv_insn.h \
	src/libbluray/hdmv/hdmv_vm.h \
	src/libbluray/hdmv/hdmv_vm.c \
	src/libbluray/hdmv/mobj_data.h \
	src/libbluray/hdmv/mobj_parse.h \
	src/libbluray/hdmv/mobj_parse.c \
	src/libbluray/hdmv/mobj_print.h \
	src/libbluray/hdmv/mobj_print.c \
	src/util/array.h \
	src/util/array.c \
	src/util/attributes.h \
	src/util/bits.h \
	src/util/bits.c \
	src/util/event_queue.h \
	src/util/event_queue.c \
	src/util/logging.h \
	src/util/logging.c \
	src/util/log_control.h \
	src/util/macro.h \
	src/util/mutex.h \
	src/util/mutex.c \
	src/util/refcnt.h \
	src/util/refcnt.c \
	src/util/strutl.h \
	src/util/strutl.c \
	src/util/time.h \
	src/util/time.c

# bd-j
libbluray_la_SOURCES += \
	src/libbluray/bdj/bdj.h \
	src/libbluray/bdj/bdj.c \
	src/libbluray/bdj/bdjo_data.h \
	src/libbluray/bdj/bdjo_parse.h \
	src/libbluray/bdj/bdjo_parse.c \
	src/libbluray/bdj/native/bdjo.h \
	src/libbluray/bdj/native/bdjo.c \
	src/libbluray/bdj/native/java_awt_BDFontMetrics.h \
	src/libbluray/bdj/native/java_awt_BDFontMetrics.c \
	src/libbluray/bdj/native/java_awt_BDGraphics.h \
	src/libbluray/bdj/native/java_awt_BDGraphics.c \
	src/libbluray/bdj/native/org_videolan_Libbluray.h \
	src/libbluray/bdj/native/org_videolan_Libbluray.c \
	src/libbluray/bdj/native/org_videolan_Logger.h \
	src/libbluray/bdj/native/org_videolan_Logger.c \
	src/libbluray/bdj/native/register_native.h \
	src/libbluray/bdj/native/register_native.c \
	src/libbluray/bdj/native/util.h \
	src/libbluray/bdj/native/util.c

# libudfread
libbluray_la_SOURCES += \
	src/libbluray/disc/udf_fs.h \
	src/libbluray/disc/udf_fs.c
if !HAVE_LIBUDFREAD
libbluray_la_SOURCES += \
	contrib/libudfread/src/blockinput.h \
	contrib/libudfread/src/default_blockinput.h \
	contrib/libudfread/src/default_blockinput.c \
	contrib/libudfread/src/ecma167.h \
	contrib/libudfread/src/ecma167.c \
	contrib/libudfread/src/udfread.h \
	contrib/libudfread/src/udfread.c
endif

if HAVE_DARWIN
libbluray_la_SOURCES+= \
	src/file/dir_posix.c \
	src/file/dirs_darwin.c \
	src/file/dl_posix.c \
	src/file/file_posix.c \
	src/file/mount_darwin.c
else
if HAVE_WIN32
libbluray_la_SOURCES+= \
	src/file/dir_win32.c \
	src/file/dirs_win32.c \
	src/file/dl_win32.c \
	src/file/file_win32.c \
	src/file/mount.c
else
if HAVE_GETFSSTAT
libbluray_la_SOURCES+= \
	src/file/dir_posix.c \
	src/file/dirs_xdg.c \
	src/file/dl_posix.c \
	src/file/file_posix.c \
	src/file/mount_getfsstat.c
else
libbluray_la_SOURCES+= \
	src/file/dir_posix.c \
	src/file/dirs_xdg.c \
	src/file/dl_posix.c \
	src/file/file_posix.c \
	src/file/mount.c
endif
endif
endif

libbluray_la_LDFLAGS= -no-undefined -version-info $(LT_VERSION_INFO)
libbluray_la_LIBADD= $(LIBXML2_LIBS) $(FT2_LIBS) $(FONTCONFIG_LIBS) $(LIBUDFREAD_LIBS) $(EXTRA_LIBS)

noinst_HEADERS = \
	jni/jni.h \
	jni/linux/jni_md.h \
	jni/win32/jni_md.h \
	jni/darwin/jni_md.h \
	jni/freebsd/jni_md.h \
	jni/netbsd/jni_md.h \
	jni/openbsd/jni_md.h

pkginclude_HEADERS = \
	src/file/filesystem.h \
	src/libbluray/bluray.h \
	src/libbluray/bluray-version.h \
	src/libbluray/keys.h \
	src/libbluray/player_settings.h \
	src/libbluray/bdnav/clpi_data.h \
	src/libbluray/bdnav/meta_data.h \
	src/libbluray/decoders/overlay.h \
	src/util/log_control.h


if USING_BDJAVA_BUILD_JAR

if USING_JAVAC_12
java_versions = -Djava_version_asm=1.7 -Djava_version_bdj=1.7
else
if USING_JAVAC_9
java_versions = -Djava_version_asm=1.6 -Djava_version_bdj=1.6
else
java_versions = -Djava_version_asm=1.5 -Djava_version_bdj=1.4
endif
endif

if BDJ_J2SE
awt_src = java-$(BDJ_TYPE):java-build-support
else
awt_src = java-$(BDJ_TYPE)
endif

jardir=$(datadir)/java/
jar_DATA = \
	$(top_builddir)/.libs/libbluray-$(BDJ_TYPE)-$(VERSION).jar \
	$(top_builddir)/.libs/libbluray-awt-$(BDJ_TYPE)-$(VERSION).jar

$(jar_DATA): all-local

all-local:
	ant -f $(top_srcdir)/src/libbluray/bdj/build.xml \
	    -Dbuild='$(abs_builddir)/src/libbluray/bdj/build' \
	    -Ddist='$(abs_builddir)/.libs' \
	    -Dsrc_awt=:$(awt_src) \
	    $(java_versions) \
	    -Dbootclasspath="$(BDJ_BOOTCLASSPATH)" \
	    -Dversion='$(BDJ_TYPE)-$(VERSION)'

clean-local:
	ant -f $(top_srcdir)/src/libbluray/bdj/build.xml \
	    -Dbuild='$(abs_builddir)/src/libbluray/bdj/build' \
	    -Ddist='$(abs_builddir)/.libs' \
	    -Dversion='$(BDJ_TYPE)-$(VERSION)' \
	    clean
endif

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = src/libbluray.pc


#
# examples
#

if USING_EXAMPLES

noinst_PROGRAMS = \
	bdj_test \
	bdjo_dump \
	clpi_dump \
	hdmv_test \
	index_dump \
	libbluray_test \
	mobj_dump \
	mpls_dump \
	sound_dump

bin_PROGRAMS = \
	bd_list_titles \
	bd_splice \
	bd_info

bd_info_SOURCES = src/examples/bd_info.c
bd_info_LDADD = libbluray.la

bd_splice_SOURCES = src/examples/bdsplice.c
bd_splice_LDADD = libbluray.la

bdj_test_SOURCES = src/devtools/bdj_test.c
bdj_test_LDADD = libbluray.la

bdjo_dump_SOURCES = src/devtools/bdjo_dump.c
bdjo_dump_LDADD = libbluray.la

clpi_dump_CFLAGS = $(AM_CFLAGS)
clpi_dump_SOURCES = \
	src/devtools/clpi_dump.c \
	src/devtools/strings.h \
	src/devtools/util.c \
	src/devtools/util.h
clpi_dump_LDADD = libbluray.la

hdmv_test_SOURCES = src/devtools/hdmv_test.c
hdmv_test_LDADD = libbluray.la

index_dump_SOURCES = src/examples/index_dump.c
index_dump_LDADD = libbluray.la

libbluray_test_SOURCES = src/examples/libbluray_test.c
libbluray_test_LDADD = libbluray.la

bd_list_titles_SOURCES = src/examples/list_titles.c
bd_list_titles_LDADD = libbluray.la

mobj_dump_CFLAGS = $(AM_CFLAGS)
mobj_dump_SOURCES = \
	src/devtools/mobj_dump.c \
	src/libbluray/hdmv/mobj_print.c
mobj_dump_LDADD = libbluray.la

mpls_dump_CFLAGS = $(AM_CFLAGS)
mpls_dump_SOURCES = \
	src/devtools/mpls_dump.c \
	src/devtools/strings.h \
	src/devtools/util.c \
	src/devtools/util.h
mpls_dump_LDADD = libbluray.la

sound_dump_SOURCES = src/examples/sound_dump.c
sound_dump_LDADD = libbluray.la

endif
