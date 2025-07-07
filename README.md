## QuantStart Quantitative Finance source code  

This repo contains Quantitative Finance source code taken from **QuantStart**  

https://www.quantstart.com/

There were some bugs in the code which I fixed and made it work.

## Details

The code are taken from these articles and its equivalent executable:

Statistical Distributions in C++  
https://www.quantstart.com/articles/Statistical-Distributions-in-C/
```cmake
./standard_distribution
```

Random Number Generation via Linear Congruential Generators in C++ 
https://www.quantstart.com/articles/Random-Number-Generation-via-Linear-Congruential-Generators-in-C/
```cmake
./linear_congruent_generator
```

Generating Correlated Asset Paths in C++ via Monte Carlo 
https://quantstart.com/articles/Generating-Correlated-Asset-Paths-in-C-via-Monte-Carlo/
```cmake
./correlated_stocks
```

Asian option pricing with C++ via Monte Carlo Methods 
https://www.quantstart.com/articles/Asian-option-pricing-with-C-via-Monte-Carlo-Methods/
```cmake
./asian_option_mc
```

European vanilla option pricing with C++ via Monte Carlo methods 
https://www.quantstart.com/articles/European-vanilla-option-pricing-with-C-via-Monte-Carlo-methods/
```cmake
add_executable(european_option_mc src/main_european_option_mc.cpp)
```

European vanilla option pricing with C++ and analytic formulae 
https://www.quantstart.com/articles/European-vanilla-option-pricing-with-C-and-analytic-formulae/
```cmake
add_executable(european_option_bs src/main_european_option_bs.cpp)
```

Heston Stochastic Volatility Model with Euler Discretisation in C++ 
https://www.quantstart.com/articles/Heston-Stochastic-Volatility-Model-with-Euler-Discretisation-in-C/
```cmake
add_executable(heston src/main_heston.cpp)
```


## Build

**MacOS**

```sh
mkdir build
cd build
cmake ..
make
```

## Usage example

These are the executables to run.

```sh
./standard_distribution

./linear_congruent_generator

./correlated_stocks

./asian_option_mc

./european_option_mc

./european_option_bs

./heston
```


## Release History

* tag 0.0.1 Initial release of working code

## Link

[https://github.com/alokswaincontact/quantstart](https://github.com/alokswaincontact/quantstart)

## Contributors

Michael Halls-Moore - support@quantstart.com  
Alok Swain – alokswaincontact@gmail.com
