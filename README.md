dekugrid -- multiple implementations of the Deco Grid System
by Tobias Bengfort <tobias.bengfort@gmx.net>
based on deco.gs by Alexander Limi <http://limi.net/deco.gs>
Placed in the Public Domain.

Decogrid is a simple, small and flexible grid system.  The base technique used
in Deco is something that is documented in the article [Faux Absolute
Positioning][1] at A List Apart.  Deco is just a system that applies that
method to the notion of a CSS grid system.  Dekugrid (note the 'ku') in turn is
just a system to generate decogrids using CSS preprocessors (currently
[SASS][2] and [LESS][3]).

Why would you want to use it? Because you need an unusual number of columns
(the original decogrid provides 12 and 16) or want to configure the margin
between columns (the original decogrid provides 2.08333% and 0%).

Just set the appropriate values for `$cols` and `$margin` and the preprocessor
will do all the math. In addition you get mixins to use in your existing
classes.

Dekugrids is designed as a drop-in replacement for decogrid.  However you
can set a `$prefix` for the generated CSS classes (e.g. `'deco-'`) to avoid
naming collisions.

[1]: http://www.alistapart.com/articles/fauxabsolutepositioning/
[2]: http://sass-lang.com
[3]: http://lesscss.org
