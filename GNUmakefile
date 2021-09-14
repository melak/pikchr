
PIKCHR	?= pikchr
PFLAGS	+= --svg-only
SRCS	:= $(wildcard *.pikchr)
OBJS	:= $(SRCS:.pikchr=.svg)

%.html:	%.pikchr
	$(PIKCHR) $< > $@

%.svg:	%.pikchr
	$(PIKCHR) $(PFLAGS) $< > $@

all:	$(OBJS)
clean:
	-rm -f *.html *.svg
