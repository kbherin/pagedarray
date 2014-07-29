# Tie::PagedArray

This tieable module helps deal with very large arrays by paging. The array is broken into pages and only one page is in memory. Rest of them are written to disk. The elements of the paged array can be anything.

## SYNOPSIS

    tie my(@large_array), 'Tie::PagedArray';
    tie my(@large_array), 'Tie::PagedArray', page_size => 10000, paging_dir => '/tmp';

## DEPENDENCIES

    Storable

## LICENSE AND COPYRIGHT

Copyright (C) 2013 Kartik Bherin

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.
