# Makefile generated by imake - do not edit!
# $XConsortium: imake.c,v 1.65 91/07/25 17:50:17 rws Exp $

CAMLC=camlc
COMPFLAGS=-W
CAMLLIBR=camllibr
CAMLLEX=camllex
CAMLYACC=camlyacc
CPP=/lib/cpp -P
CAMLDEP=camldep
RM=rm -f
TOP=../.
CONFIG=$(TOP)/config

all::

# (begin Imakefile)

all::kb

kb: prelude.zo terms.zo equation.zo order.zo kb.zo go.zo
	$(CAMLC) $(LINKFLAGS)  prelude.zo terms.zo equation.zo order.zo kb.zo go.zo -o kb

clean::
	$(RM) kb

# (end Imakefile)

clean::
	$(RM) *.zi *.zix *.zo *~ #*#

beforedepend::

makefile: beforedepend
	imake -I$(CONFIG) -DTOPDIR=$(TOP)
	$(CAMLDEP) *.mli *.ml >> Makefile

makefiles:: makefile

.SUFFIXES: .mli .zi .ml .zo

.mli.zi:
	$(CAMLC) $(COMPFLAGS) -c $<

.ml.zo:
	$(CAMLC) $(COMPFLAGS) -c $<

# Generated dependencies below

equation.zo: prelude.zo terms.zo 
go.zo: order.zo kb.zo terms.zo 
kb.zo: equation.zo prelude.zo terms.zo 
order.zo: terms.zo 
