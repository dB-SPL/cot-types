# cot-types
Copied from ESRI's solutions-geoevent-java repository at:
https://github.com/Esri/solutions-geoevent-java

     Copyright (C) 2003 MITRE Corporation
     Author: Mike Butler <mgb@mitre.org>
     Date: 02-Mar-03
     Desc: Type mapping for CoT schemas...
           This is the mapping from CoT target types to other
           message format target types.  At present, the CoT type
           serves as a prefix for the type.  Upper case
           strings are taken directly from the mil-std-2525
           type hierarchy, lower case characters are CoT
           extensions.  The matching *is* case sensitive!!!
           (This avoids clashes is mil-std-2525 gets extended.)
           Note that these types presently are exclusive to
           the "atom" part of the CoT hierarchy (a-*) and that
           they do not include the initial a-x- prefix.
           This allows the same type mapping to be used for all
           variants (a-h-, a-f-, a-u-, ...)
           Conversion in the inverse direction (from some other
           type e.g., TADIL-J to CoT) can be accomplished similarly,
           but there is the caveat that the mappings are not
           one-to-one.  (E.g., several Tadil-J "SAM" types may
           map to a single CoT SAM, so it's tough to use the
           same table both ways...)
           Coversion from CoT types to other display types...
           Note that tadil-j displays can't show the full tadil-j
           type catalog, so we settle for a few arbitrary mappings...
           **NOTE** tadilj mappings are presently overridden in the
           Tadilj.pm module!!!  (What's here don't matter for TADILJ!)
    17-Feb-05
           Add in other portions of the MS2525 type tree, specifically
           for MOOTW.
