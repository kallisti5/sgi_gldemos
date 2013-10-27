#
# Copyright (c) Mark J. Kilgard, 1996, 1997.
# Copyright (c0 Alexander von Gluck IV, 2012-2013
#

LN = ln -s
MV = mv
RM = -rm -rf

TARGETS = glutmech

LDFLAGS = -lglut -lGLU -lGL

SRCS =	glutmech.c
OBJS =	$(SRCS:.c=.o)

default : $(TARGETS)

glutmech : $(OBJS)
	$(RM) $@
	$(CC) -o $@ $(OBJS) $(LDFLAGS)

clean:
	$(RM) $(OBJS) $(TARGETS)

include $(COMMONRULES)
