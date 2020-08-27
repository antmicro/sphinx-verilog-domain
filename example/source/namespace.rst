verilog:namespace{,-push,-pop}
******************************

* :verilog:ref:`$root::in_global_ns`
* :verilog:ref:`$root::A::B::inside_a_b`
* :verilog:ref:`$root::A::B::C::D::inside_a_b_c_d`
* :verilog:ref:`$root::A::B::inside_a_b_again`
* :verilog:ref:`$root::A::B::refname_inside_a_b`
* :verilog:ref:`$root::A::B::X::Y::inside_a_b_x_y`
* :verilog:ref:`$root::A::namespaces_test_module_in_a`
* :verilog:ref:`$root::B::C::D::module_inside_b_c_d`
* :verilog:ref:`$root::A::input_in_a`
* :verilog:ref:`$root::global_ns_again`

.. verilog:port:: input in_global_ns;

::

    .. verilog:namespace:: A::B

.. verilog:namespace:: A::B

.. verilog:port:: input inside_a_b;

::

    .. verilog:namespace-push:: C::D

.. verilog:namespace-push:: C::D

.. verilog:port:: input inside_a_b_c_d;

::

    .. verilog:namespace-pop::

.. verilog:namespace-pop::

.. verilog:port:: input inside_a_b_again;

.. verilog:port:: input inside_a_b_with_refname;
    :refname: refname_inside_a_b

::

    .. verilog:namespace-push:: X::Y

.. verilog:namespace-push:: X::Y

.. verilog:port:: input inside_a_b_x_y;

::

    .. verilog:namespace:: A

.. verilog:namespace:: A

.. verilog:module:: module namespaces_test_module_in_a(a);

    ::

        .. verilog:namespace:: B::C
        .. verilog:namespace-push:: D

    .. verilog:namespace:: B::C
    .. verilog:namespace-push:: D

    .. verilog:module:: module module_inside_b_c_d(a);

Namespace changes applied inside a directive's content (e.g. in module description above) should not be propagated to a parent rst scope.

.. verilog:port:: input input_in_a;

::

    .. verilog:namespace::

.. verilog:namespace::

.. verilog:port:: input global_ns_again;



----

Some text to enable scrolling...

- Lorem
- ipsum
- dolor
- sit
- amet,
- consectetur
- adipiscing
- elit.
- Donec
- ac
- mattis
- metus.
- Praesent
- faucibus
- tortor
- eu
- euismod
- imperdiet.
- Mauris
- a
- porta
- mauris,
- ac
- faucibus
- magna.
- Aliquam
- lacinia
- hendrerit
- interdum.
- Nullam
- tempor,
- massa
- ac
- scelerisque
- porta,
- nunc
- nunc
- dignissim
- ex,
- id
- commodo
- ligula
- lorem
- sit
- amet
- ligula.
- Morbi
- rhoncus
- et
- orci
- ut
- euismod.
- In
- eu
- scelerisque
- lectus,
- tempor
- vulputate
- risus.
- Proin
- imperdiet
- dignissim
- condimentum.
- Nunc
- ultrices
- laoreet
- faucibus.
- Morbi
- fringilla
- efficitur
- dolor,
- et
- eleifend
- erat
- pellentesque
- at.
- Donec
- sed
- ligula
- ac
- ligula
- consequat
- lobortis.
- Integer
- nec
- diam
- id
- magna
- scelerisque
- placerat.
