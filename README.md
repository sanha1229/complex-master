# cpxn
Javascript complex number library

## Copyright
&copy; 2021 Sanha, all rights reserved.

## License
CC BY-NC-ND 4.0

## Notice
<del>한국어 문서 쓰실 분 구함</del>

## Use

## Get Started
```javascript
const { Complex, Cxmath } = require(PATH);

```
### Declaration
#### constructor(re: number, im: number)
declare with cartesian form (if the imaginary part equals zero, you can leave it out.)
```javascript
let z = new Complex(1, 2); // 1+2i
```
#### constructor(abs: number, arg: number, 'polar')
declare with polar form
```javascript
let z = new Complex(Math.PI, 2, 'polar'); // 2exp(iπ) = -2
```

#### constructor(cx: complex)
copy
```javascript
let z = new Complex(z); // 1+2i
```

### Properties
```javascript
z.re; // real part
z.im; // imaginary part
z.abs; // absolute value
z.arg; // the argument
```

### The four fundamental arithmetic operations & involution
```javascript
let p = new Complex(1, 2);
let q = new Complex(3, -4);
```
#### add(z: number/complex)
addition
```javascript
p.add(q); // 4-2i
p.add(6); // 7+2i
```

#### sub(z: number/complex)
subtraction
```javascript
p.sub(q); // -2+6i
p.sub(6); // -5+2i
```

#### mul(z: number/complex)
multifunction
```javascript
p.mul(q); // 11+2i
p.mul(6); // 6+12i
```

#### div(z: number/complex)
division
```javascript
p.div(q); // -0.2+0.4i
p.div(4); // 0.25+0.5i
```

#### inv(z: number/complex)
involution
```javascript
p.inv(q); // 932.1391946432212+95.9465336603415i
p.inv(6); // 117+44i
```

### Opposite Number (Additive Inverse)

#### Cxmath.opp(z: number/complex)
opposite number (additive inverse)
```javascript
Cxmath.opp(z);
```

### Complex Conjugate

#### Cxmath.conj(z: number/complex)
complex conjugate
```javascript
Cxmath.conj(z);
```

### Radical Roots

#### Cxmath.sqrt(z: number/complex)
principal square root
```javascript
Cxmath.sqrt(z);
```

#### Cxmath.cbrt(z: number/complex)
principal cube root
```javascript
Cxmath.cbrt(z);
```

### Exponential Function & Logarithm

#### Cxmath.exp(z: number/complex)
exp(z)
```javascript
Cxmath.exp(z);
```

#### Cxmath.ln(z: number/complex)
<a href="https://namu.wiki/w/복소로그함수#s-3">Log(z)</a>, natural logarithm defined in principal branch
```javascript
Cxmath.ln(z);
```

#### Cxmath.log(b: number/complex, a: number/complex)
logarithm with base b and antilogarithm a (defined in principal branch)
```javascript
Cxmath.log(b, a);
```

### Trigonometric Functions

#### Cxmath.sin(z: number/complex)
sine
```javascript
Cxmath.sin(z);
```

#### Cxmath.cos(z: number/complex)
cosine
```javascript
Cxmath.cos(z);
```

#### Cxmath.tan(z: number/complex)
tangent
```javascript
Cxmath.tan(z);
```

### Inverse Trigonometric Functions

#### Cxmath.asin(z: number/complex)
arcsine
```javascript
Cxmath.asin(z);
```

#### Cxmath.acos(z: number/complex)
arccosine
```javascript
Cxmath.acos(z);
```

#### Cxmath.atan(z: number/complex)
arctangent
```javascript
Cxmath.atan(z);
```

### Hyperbolic Functions

#### Cxmath.sinh(z: number/complex)
hyperbolic sine
```javascript
Cxmath.sinh(z);
```

#### Cxmath.cosh(z: number/complex)
hyperbolic cosine
```javascript
Cxmath.cosh(z);
```

#### Cxmath.tanh(z: number/complex)
hyperbolic tangent
```javascript
Cxmath.tanh(z);
```

### Inverse Hyperbolic Functions

#### Cxmath.asinh(z: number/complex)
inverse hyperbolic sine
```javascript
Cxmath.asinh(z);
```

#### Cxmath.acosh(z: number/complex)
inverse hyperbolic cosine
```javascript
Cxmath.acosh(z);
```

#### Cxmath.atanh(z: number/complex)
inverse hyperbolic tangent
```javascript
Cxmath.atanh(z);
```

### Sign Function

#### Cxmath.csgn(z: number/complex)
<a href="https://namu.wiki/w/부호함수#s-3">csgn(z)</a>
```javascript
Cxmath.csgn(z);
```

### Random

#### Cxmath.random()
random complex (both real part and imaginary part are more than or equal to 0 and less than 1)
```javascript
Cxmath.random();
```
