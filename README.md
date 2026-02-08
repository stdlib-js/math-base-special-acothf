<!--

@license Apache-2.0

Copyright (c) 2026 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# acothf

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Compute the [inverse hyperbolic cotangent][hyperbolic-arctangent] of a single-precision floating-point number.



<section class="usage">

## Usage

```javascript
import acothf from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-acothf@deno/mod.js';
```
The previous example will load the latest bundled code from the deno branch. Alternatively, you may load a specific version by loading the file from one of the [tagged bundles](https://github.com/stdlib-js/math-base-special-acothf/tags). For example,

```javascript
import acothf from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-acothf@v0.1.1-deno/mod.js';
```

#### acothf( x )

Computes the [inverse hyperbolic cotangent][hyperbolic-arctangent] of a single-precision floating-point number.

```javascript
var v = acothf( 2.0 );
// returns ~0.5493

v = acothf( 1.0 );
// returns Infinity
```

The domain of the inverse hyperbolic cotangent is the union of the intervals `(-inf,-1]` and `[1,inf)`. If provided a value on the open interval `(-1,1)`, the function returns `NaN`.

```javascript
var v = acothf( 0.0 );
// returns NaN

v = acothf( 0.5 );
// returns NaN
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
import uniform from 'https://cdn.jsdelivr.net/gh/stdlib-js/random-array-uniform@deno/mod.js';
import logEachMap from 'https://cdn.jsdelivr.net/gh/stdlib-js/console-log-each-map@deno/mod.js';
import acothf from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-acothf@deno/mod.js';

var x = uniform( 100, 1.0, 5.0, {
    'dtype': 'float32'
});

logEachMap( 'acothf(%0.4f) = %0.4f', x, acothf );
```

</section>

<!-- /.examples -->

<!-- C interface documentation. -->



<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2026. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-acothf.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-acothf

[test-image]: https://github.com/stdlib-js/math-base-special-acothf/actions/workflows/test.yml/badge.svg?branch=v0.1.1
[test-url]: https://github.com/stdlib-js/math-base-special-acothf/actions/workflows/test.yml?query=branch:v0.1.1

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-acothf/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-acothf?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-acothf.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-acothf/main

-->

[chat-image]: https://img.shields.io/badge/zulip-join_chat-brightgreen.svg
[chat-url]: https://stdlib.zulipchat.com

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-acothf/tree/deno
[deno-readme]: https://github.com/stdlib-js/math-base-special-acothf/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/math-base-special-acothf/tree/umd
[umd-readme]: https://github.com/stdlib-js/math-base-special-acothf/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/math-base-special-acothf/tree/esm
[esm-readme]: https://github.com/stdlib-js/math-base-special-acothf/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/math-base-special-acothf/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-acothf/main/LICENSE

[hyperbolic-arctangent]: https://en.wikipedia.org/wiki/Inverse_hyperbolic_function

<!-- <related-links> -->

<!-- </related-links> -->

</section>

<!-- /.links -->
