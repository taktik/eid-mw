lib_LTLIBRARIES = libbeidpkcs11.la
AM_CFLAGS = -DLTC_NO_ASM
libbeidpkcs11_la_CXXFLAGS = -DUSING_DL_OPEN -DEIDMW_CAL_EXPORT -DCAL_BEID -DCARDPLUGIN_IN_CAL -DBEID_35 -DNDEBUG -DBEID_OLD_PINPAD -DLTC_NO_ASM -fvisibility=hidden -I$(srcdir)/common -I$(srcdir)/cardlayer -I$(top_srcdir)/doc/sdk/include/rsaref220 @PCSC_CFLAGS@
libbeidpkcs11_la_CPPFLAGS = -I$(srcdir)/common -I$(srcdir)/cardlayer -I$(top_srcdir)/doc/sdk/include/rsaref220 @PCSC_CFLAGS@ -DLIBEXECDIR='"$(libexecdir)"'
libbeidpkcs11_la_LIBADD = @PCSC_LIBS@ -ldl
libbeidpkcs11_la_SOURCES = \
	asn1.c \
	cal.cpp \
	cert.c \
	encrypt.c \
	general.c \
	pkcs11log.c \
	object.c \
	p11.c \
	phash.cpp \
	session.c \
	sign.c \
	pkcs11util.cpp \
	display.cpp \
	common/mw_util.cpp \
	common/libtomcrypt/md5.c \
	common/libtomcrypt/rmd160.c \
	common/libtomcrypt/sha1.c \
	common/libtomcrypt/sha256.c \
	common/libtomcrypt/sha384.c \
	common/libtomcrypt/sha512.c \
	common/bytearray.cpp \
	common/configcommon.cpp \
	common/configuration.cpp \
	common/datafile.cpp \
	common/dynamiclib.cpp \
	common/hash.cpp \
	common/logbase.cpp \
	common/log.cpp \
	common/mutex.cpp \
	common/mwexception.cpp \
	common/thread.cpp \
	common/tlvbuffer.cpp \
	common/tlv.cpp \
	common/util.cpp \
	cardlayer/card.cpp \
	cardlayer/cardfactory.cpp \
	cardlayer/cardlayer.cpp \
	cardlayer/cardreaderinfo.cpp \
	cardlayer/context.cpp \
	cardlayer/p15correction.cpp \
	cardlayer/pcsc.cpp \
	cardlayer/pinpad.cpp \
	cardlayer/pinpadlib.cpp \
	cardlayer/pkcs15.cpp \
	cardlayer/pkcs15parser.cpp \
	cardlayer/pkicard.cpp \
	cardlayer/reader.cpp \
	cardlayer/readersinfo.cpp \
	cardlayer/threadpool.cpp \
	cardlayer/unknowncard.cpp \
	cardlayer/cardpluginbeid/beidcard.cpp \
	cardlayer/cardpluginbeid/beidp15correction.cpp

noinst_HEADERS = \
	p11.h \
	phash.h \
	cal.h \
	beid_p11.h \
	cert.h \
	asn1.h \
	util.h \
	log.h \
	display.h \
	common/thread.h \
	common/prefix.h \
	common/bytearray.h \
	common/mutex.h \
	common/dynamiclib.h \
	common/tlv.h \
	common/export.h \
	common/tlvbuffer.h \
	common/hash.h \
	common/configuration.h \
	common/util.h \
	common/mwexception.h \
	common/datafile.h \
	common/mw_util.h \
	common/log.h \
	common/svn_revision.h \
	common/tlvtagdefinitions.h \
	common/eiderrors.h \
	common/libtomcrypt/tomcrypt_hash.h \
	common/libtomcrypt/tomcrypt_cfg.h \
	common/libtomcrypt/tomcrypt_argchk.h \
	common/libtomcrypt/tomcrypt_macros.h \
	common/threaddefines.h \
	common/logbase.h \
	cardlayer/cardlayer.h \
	cardlayer/pkcs15parser.h \
	cardlayer/internalconst.h \
	cardlayer/card.h \
	cardlayer/cardfactory.h \
	cardlayer/pkcs15.h \
	cardlayer/context.h \
	cardlayer/cardpluginbeid/beidp15correction.h \
	cardlayer/cardpluginbeid/beidcard.h \
	cardlayer/cardreaderinfo.h \
	cardlayer/pinpadlib.h \
	cardlayer/threadpool.h \
	cardlayer/pcsc.h \
	cardlayer/cardlayerconst.h \
	cardlayer/pinpad2.h \
	cardlayer/pinpad.h \
	cardlayer/p15objects.h \
	cardlayer/p15correction.h \
	cardlayer/readersinfo.h \
	cardlayer/pkicard.h \
	cardlayer/unknowncard.h \
	cardlayer/reader.h \
	dialogs/langutil.h \
	dialogs/language.h \
	dialogs/dialogsqtsrv/dlgwndpinpadinfo.h \
	dialogs/dialogsqtsrv/dlgwndaskaccess.h \
	dialogs/dialogsqtsrv/dlgwndmodal.h \
	dialogs/dialogsqtsrv/dlgwndbase.h \
	dialogs/dialogsqtsrv/dlgwndaskpins.h \
	dialogs/dialogsqtsrv/dlgwndbadpin.h \
	dialogs/dialogsqtsrv/dlgwndaskpin.h \
	dialogs/sharedmem.h \
	dialogs/dialogs.h \
	dialogs/dialogsqtsrv/dlgs.qrc \
	dialogs/dialogsqtsrv/dlgwndaskaccess.ui \
	dialogs/dialogsqtsrv/dlgwndaskpins.ui \
	dialogs/dialogsqtsrv/dlgwndaskpin.ui \
	dialogs/dialogsqtsrv/dlgwndbadpin.ui \
	dialogs/dialogsqtsrv/dlgwndmodal.ui \
	dialogs/dialogsqtsrv/dlgwndpinpadinfo.ui \
	dialogs/dialogsqtsrv/qt.conf \
	dialogs/dialogsqtsrv/resource/ICO_CARD_DIGSIG_128x128.png \
	dialogs/dialogsqtsrv/resource/ICO_CARD_EID_PLAIN_16x16.png \
	dialogs/dialogsqtsrv/resource/ICO_CARD_INFO_64x64.png \
	dialogs/dialogsqtsrv/resource/ICO_CARD_NOK_64x64.png \
	dialogs/dialogsqtsrv/resource/ICO_CARD_PIN_128x128.png \
	dialogs/dialogsqtsrv/resource/ICO_CARD_QUESTION_64x64.png \
	dialogs/dialogsqtsrv/resource/ICO_CARD_WARNING_64x64.png \
	dialogs/dialogsqtsrv/resource/KeyPadButton0.png \
	dialogs/dialogsqtsrv/resource/KeyPadButton1.png \
	dialogs/dialogsqtsrv/resource/KeyPadButton2.png \
	dialogs/dialogsqtsrv/resource/KeyPadButton3.png \
	dialogs/dialogsqtsrv/resource/KeyPadButton4.png \
	dialogs/dialogsqtsrv/resource/KeyPadButton5.png \
	dialogs/dialogsqtsrv/resource/KeyPadButton6.png \
	dialogs/dialogsqtsrv/resource/KeyPadButton7.png \
	dialogs/dialogsqtsrv/resource/KeyPadButton8.png \
	dialogs/dialogsqtsrv/resource/KeyPadButton9.png \
	dialogs/dialogsqtsrv/resource/KeyPadButtonCE.png \
	dialogs/dialogsqtsrv/resource/KeyPadButton.png \
	dialogs/dialogsqtsrv/resource/PINdisplay.png \
	dialogs/dialogsgtk/beid-i18n.h \
	dialogs/dialogsgtk/single_dialog.h \
	dialogs/dialogsgtk/parent.h \
	dialogs/dialogsgtk/gtk_dialog_names.h
if NO_DIALOGS
libbeidpkcs11_la_CXXFLAGS += -DNO_DIALOGS
else
libbeidpkcs11_la_CXXFLAGS += -I$(srcdir)/dialogs
libbeidpkcs11_la_SOURCES += \
	dialogs/dialogsgtk/dlgs_gtk.cpp \
	dialogs/dialogsgtk/single_dialog.c
endif

libexec_PROGRAMS = beid-askpin beid-changepin beid-badpin beid-askaccess beid-spr-askpin beid-spr-changepin

beid_askpin_SOURCES = dialogs/dialogsgtk/parent.c dialogs/dialogsgtk/beid-askpin.c
beid_askpin_CPPFLAGS = -I$(srcdir)/dialogsgtk -I$(srcdir)/../common/src -I$(srcdir)/src @GTK_CFLAGS@
beid_askpin_LDADD = @GTK_LIBS@

beid_changepin_SOURCES = dialogs/dialogsgtk/parent.c dialogs/dialogsgtk/beid-changepin.c
beid_changepin_CPPFLAGS = -I$(dialogsdir)/dialogsgtk -I$(dialogsdir)/../common/dialogs -I$(dialogsdir)/dialogs @GTK_CFLAGS@
beid_changepin_LDADD = @GTK_LIBS@

beid_badpin_SOURCES = dialogs/dialogsgtk/parent.c dialogs/dialogsgtk/beid-badpin.c
beid_badpin_CPPFLAGS = -I$(dialogsdir)/dialogsgtk -I$(dialogsdir)/../common/dialogs -I$(dialogsdir)/dialogs @GTK_CFLAGS@
beid_badpin_LDADD = @GTK_LIBS@

beid_askaccess_SOURCES = dialogs/dialogsgtk/parent.c dialogs/dialogsgtk/beid-askaccess.c
beid_askaccess_CPPFLAGS = -I$(dialogsdir)/dialogsgtk -I$(dialogsdir)/../common/dialogs -I$(dialogsdir)/dialogs @GTK_CFLAGS@
beid_askaccess_LDADD = @GTK_LIBS@

beid_spr_askpin_SOURCES = dialogs/dialogsgtk/parent.c dialogs/dialogsgtk/beid-spr-askpin.c
beid_spr_askpin_CPPFLAGS = -I$(dialogsdir)/dialogsgtk -I$(dialogsdir)/../common/dialogs -I$(dialogsdir)/dialogs @GTK_CFLAGS@
beid_spr_askpin_LDADD = @GTK_LIBS@

beid_spr_changepin_SOURCES = dialogs/dialogsgtk/parent.c dialogs/dialogsgtk/beid-spr-changepin.c
beid_spr_changepin_CPPFLAGS = -I$(dialogsdir)/dialogsgtk -I$(dialogsdir)/../common/dialogs -I$(dialogsdir)/dialogs @GTK_CFLAGS@
beid_spr_changepin_LDADD = @GTK_LIBS@

pkgconfig_DATA=libbeidpkcs11.pc
