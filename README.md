# smartpairs.vim

Smartpairs.vim will add proper pairings as you type:

    You type    You get    Notes ~
    (           (_)        "_" represents the cursor
    <BS>        _
    [           [_]
    ]           []_
    <BS>        [_
    <BS>        _
    (           (_)
    <Space>     ( _ )
    <BS>        (_ )
    <BS>        _ )       Here the pair won't be deleted, as there's a space
    <C-O>df)    _         So we manually clear it
    {           {_}
    <CR>        {         Cursor will be indented based on current syntax
                  _
                }

It has multiple options you can use to configure it. See the
[documentation](doc\smartpairs.txt) for all the details.

# Why

There are other plugins which do pairings as well, but in my opinion they do
too much. They do so much, there are lots of edge cases where you don't want
the pairing functionality to trigger.

This plugin aims to be minimal, and err on the side of doing nothing, rather
than trying to guess all cases.
