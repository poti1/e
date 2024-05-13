# LOGO

               ____
      ___     / __/___  _____   ____ ___  ___
     / _ \   / /_/ __ \/ ___/  / __ `__ \/ _ \
    /  __/  / __/ /_/ / /     / / / / / /  __/
    \___/  /_/  \____/_/     /_/ /_/ /_/\___/

# NAME

e - Unleash the power of e!

# SYNOPSIS

Convert a data structure to json:

    perl -Me -e 'say j { a => [ 1..3] }'

Convert a data structure to yaml:

    perl -Me -e 'say yml { a => [ 1..3] }'

Pretty print a data structure:

    perl -Me -e 'p { a => [ 1..3] }'

Data dump a data structure:

    perl -Me -e 'd { a => [ 1..3] }'

Devel::Peek dump a data structure:

    perl -Me -e 'dd { a => [ 1..3] }'

Add a trace marker:

    perl -Me -e 'dd {'
    perl -Me -e 'sub f1 { trace } sub f2 { f1 } f2'

Watch a reference for changes:

    perl -Me -e 'my $v = {}; sub f1 { watcg( $v ) } sub f2 { f1; $v->{a} = 1 } f2'

Launch the Runtime::Debugger:

    perl -Me -e 'repl'

Invoke the Tiny::Prof:

    perl -Me -e 'prof'

# SUBROUTINES

## monkey\_patch

insert subroutines into the symbol table.

Extracted from Mojo::Util for performance.

Can be updated once this issue is resolved:
[https://github.com/mojolicious/mojo/pull/2173](https://github.com/mojolicious/mojo/pull/2173)

## import

Inserts commands into caller's namespace.

# AUTHOR

Tim Potapov, `<tim.potapov[AT]gmail.com>`

# BUGS

Please report any bugs or feature requests to
[https://github.com/poti1/e/issues](https://github.com/poti1/e/issues).

# SUPPORT

You can find documentation for this module
with the perldoc command.

    perldoc e

You can also look for information at:

[https://metacpan.org/pod/e](https://metacpan.org/pod/e)

[https://github.com/poti1/e](https://github.com/poti1/e)

# LICENSE AND COPYRIGHT

This software is Copyright (c) 2024 by Tim Potapov.

This is free software, licensed under:

    The Artistic License 2.0 (GPL Compatible)
