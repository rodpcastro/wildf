# WildF

[![Fortran][Fortran Badge]][Fortran Website]
[![Docs][Docs Badge]][Docs Website]
[![Test][Test Badge]][Test Workflow]
[![Coverage][Coverage Badge]][Coverage Website]
[![License][License Badge]][License File]

WildF is a [Fortran][Fortran Website] library for evaluating mathematical [Special Functions]. Just like wild creatures, Special Functions are unusual, but interesting mathematical objects that arise in many areas of applied mathematics. This library aims to serve as a support for any project that needs the computation of these rare species.

## Functions
The following list describes the implemented functions, each validated to at least 8 digits of precision within the specified domains. Outside these domains, the same precision is not guaranteed.

* Exponential integral $\mathrm{Ei}(x)$
    * $\lbrace x \in \mathbb{R} \mid  x \in [10^{-16}, 10^2] \rbrace$
* Exponential integral $\mathrm{E}_1(x)$
    * $\lbrace x \in \mathbb{R} \mid  x \in [10^{-16}, 10^2] \rbrace$
* Exponential integral $\mathrm{E}_1(z)$
    * $\lbrace z \in \mathbb{C} \mid 10^{-16} \leq |\Re(z)| \leq 10^2,\thinspace 10^{-16} \leq |\Im(z)| \leq 10^2,\thinspace z \notin (-61, 0] \times (-0.6, 0.6) \rbrace$

This list will be updated as new functions are added and tested.

## Tests
Tests are conducted by comparing the WildF results with those of [mpmath], an arbitrary-precision numerical library. These tests ensure at least 8 digits of precision within the specified domains.

Testing routines are built using [test-drive], a standard Fortran unit testing framework.

## Documentation
The [API documentation][Docs Website] for this library is generated using [FORD] and is deployed and hosted on [ReadTheDocs].

## References
[[1][Book Zhang]] Shanjie Zhang, Jianming Jin. 1996. Computation of Special Functions. Wiley, New York, NY.

<!-- Links -->
<!-- Badges -->
[Fortran Website]: https://fortran-lang.org/
[Fortran Badge]: https://img.shields.io/badge/Fortran-734f96?logo=fortran&style=flat
[Docs Website]: https://wildf.readthedocs.io/
[Docs Badge]: https://img.shields.io/readthedocs/wildf?color=blue
[Test Workflow]: https://github.com/rodpcastro/wildf/actions/workflows/CI.yml
[Test Badge]: https://github.com/rodpcastro/wildf/actions/workflows/CI.yml/badge.svg
[Coverage Website]: https://app.codecov.io/gh/rodpcastro/wildf
[Coverage Badge]: https://codecov.io/github/rodpcastro/wildf/badge.svg
[License File]: https://github.com/rodpcastro/wildf/blob/main/LICENSE
[License Badge]: https://img.shields.io/badge/License-MIT-yellow
<!-- Introduction -->
[Special Functions]: https://www.britannica.com/science/special-function
<!-- Tests -->
[mpmath]: https://mpmath.org/
[test-drive]: https://github.com/fortran-lang/test-drive
<!-- Documentation -->
[FORD]: https://forddocs.readthedocs.io/
[ReadTheDocs]: https://about.readthedocs.com/
<!-- References -->
[Book Zhang]: https://search.worldcat.org/title/33971114
