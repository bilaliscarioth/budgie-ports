COMMENT =	budgie screensaver, screen saver and locker
DISTNAME =	budgie-screensaver-5.1.0

GH_ACCOUNT = BuddiesOfBudgie
GH_PROJECT = budgie-screensaver
# Tag is too old
GH_COMMIT = dcf496d04ae9741405c32b92c625ab082588a007

REVISION = 4

CATEGORIES=	x11

MAINTAINER=	Bilal Emohmadian <bilal@iscarioth.org>

# GNU GPLv2
PERMIT_PACKAGE=	Yes

WANTLIB = Xxf86vm c cairo dbus-1 gdk-3 gdk_pixbuf-2.0 gio-2.0
WANTLIB += X11 glib-2.0 intl gobject-2.0 gtk-3

COMPILER =	base-clang

RUN_DEPENDS = \
	x11/gnome/libgnomekbd

LIB_DEPENDS = \
	devel/gettext,-tools \
	devel/gsettings-desktop-schemas \
	x11/gnome/desktop

CONFIGURE_ARGS = \
	-Dwith-systemd=false \
	-Dwith-bsd_auth=true

MODULES= devel/meson 

CFLAGS +=	-I${LOCALBASE}/include/

.include <bsd.port.mk>
