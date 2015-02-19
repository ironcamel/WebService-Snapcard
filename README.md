# NAME

WebService::Snapcard - Snapcard (http://www.snapcard.io) API bindings

# VERSION

version 0.0001

# SYNOPSIS

    use WebService::Snapcard;

    my $snap = WebService::Snapcard->new(
        api_key    => 'API_KEY',
        api_secret => 'API_SECRET',
        logger     => Log::Tiny->new('/tmp/snap.log'), # optional
    );
    my $balance = $snap->get_merchant_balance()->{balances}{usd};

# METHODS

## get\_merchant\_balance

    get_merchant_balance()

Get merchant account balance.

## get\_invoices

    get_invoices()

Get a list of all invoices on account.

# AUTHOR

Naveed Massjouni <naveed@vt.edu>

# COPYRIGHT AND LICENSE

This software is copyright (c) 2015 by Naveed Massjouni.

This is free software; you can redistribute it and/or modify it under
the same terms as the Perl 5 programming language system itself.
