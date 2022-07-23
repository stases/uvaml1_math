Calculus
=====

Foundations
-----------

Limits and Continuity
.....................

Differentiability
.................

Basic derivatives
...........

Chain rule
..........

Application of derivative
.........................

Integrals
.........

Advanced
--------

Logarithmic Differentiation
...........................

A common trick in differentiating function is the idea of 'logarithmic differentiation'.
Let :math:`f: \mathbb{R} \to \mathbb{R}` be a differentiable function. If we differentiate :math:`\log f`, we note that by the chain rule we have

.. math::

   \frac{d \log f(x)}{dx}  \frac{1}{f(x)} \cdot \frac{d f(x)}{dx}.

A direct consequence of this is that

.. math::

   \frac{df(x)}{dx} = f(x) \cdot \frac{d \log f(x)}{dx}.

Note that this holds in general, which is quite a neat identity on its own. However, this also allows us to differentiate functions we else cannot easily differentiate,
specifically when functions are of the form :math:`(f(x))^{g(x)}.`

If we consider the function :math:`f(x) = x^x`, you might be surprised that differentiating such a simple looking function is not as straight forward as expected.
Using the above identity, we know that

.. math::

   \frac{dx^x}{dx} = x^x \cdot \frac{d\log x^x}{dx}.

Using properties of the logarithm, we notice that :math:`\log x^x = x \log x`, which is something that looks less scary
(and in particular, differentiable with our current tools):

.. math::

   \frac{d x \log x}{dx} = \log x + \frac{x}{x} = \log x + 1.

We therefore find

.. math::
   \frac{dx^x}{dx} = x^x \cdot \frac{d\log x^x}{dx} = x^x \cdot (\log x + 1).

Optimization
............

Taylor series
.............

Formal definition of a limit
............................