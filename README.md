
# Temperature Value Type
![Version 1.0.0](https://img.shields.io/badge/Version-1.0.0-brightgreen.svg) ![Licence MIT](https://img.shields.io/badge/Licence-MIT-blue.svg)
[![codecov](https://codecov.io/gh/FredEkstrand/TemperatureValue/branch/master/graph/badge.svg)](https://codecov.io/gh/FredEkstrand/TemperatureValue)

![image](https://github.com/FredEkstrand/ImageFiles/raw/master/Temperature/TemperatureGauge.jpg)

# Overview
This project takes the idea of temperature as a defined type in the .Net Framework.


#### Features
The Temperature value type have the following features:
* Create instances in desire temperature scale: Celsius, Fahrenheit, Kelvin, and Rankine.
* Default temperature scale is Celsius.
* Min/Max value are ±1.7976931348623157E+308.
* Temperature value type have properties to allow quick conversion to Celsius, Fahrenheit, Kelvin, and Rankine from default defined scale.
* Implicit/explicit conversion for UInt16, UInt32, UInt64, Int16, Int32, Int64, Single, Decimal, and Double.
* Defined operator: + unary, - negation, - subtract, + addition, * multiplicity, / division, ==, !=, <, >, <=, and >=.
* Defined IComparable, IEquatable, IConvertible, and IFormattable.

# Getting started
The source code is written in C# and targeted for the .Net Framework 4.0 and later.
Download the entire project and compile.

# Usage
Once you have compiled the project reference the dll in your Visual Studio project.
Then in your code file add the following to the collection of using statement.

```csharp
using Ekstrand;
```
#### Examples
Creates a new instance of Temperature at default Celsius scale.
```csharp
Temperature tempValue = new Temperature(23.5);
```
Create a new instance of Temperature with defined temperature scale and default value of 0.
```csharp
Temperature tempValue = new Temperature(TemperatureScaleTypes.Celsius);
```
Create a new instance of Temperature with a value and defined scale.
```csharp
Temperature tempValue = new Temperature(23.5, TemperatureScaleTypes.Fahrenheit);
```
Implicit conversion from integer to temperature
```csharp
int value = 32
Temperature tempValue = new Temperature();
tempValue = value;
```
Operators
```csharp
Temperature first = 55;
Temperature second = 60;
Temperature three = first + second;
if(three < 115)
{ ... }
else if(three >= 115)
{ ... }
...
```

# Code Documentation
MSDN-style code documentation can be found [here](http://fredekstrand.github.io/ClassDocTemperatureValue).

# History
 1.0.0 Initial release into the wild.

# Contributing

If you'd like to contribute, please fork the repository and use a feature
branch. Pull requests are always welcome.

# Contact
Fred Ekstrand
email: fredekstrandgithub@gmail.com
# Licensing

This project is licensed under the MIT License - see the LICENSE.md file for details.
