## stemre

A Python library for numerical analysis, simulation and data fitting in Science, Technology, Engineering and Mathematics (STEM).

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the Stemre library.

```bash
pip install stemre
```

## Usage

```python
import stemre as stm

# differentiation of parametric equations
t = sym.symbols('t')
x = t ** 3 - 3 * t ** 2
y = t ** 4 - 8 * t ** 2
parametric_differentiation(f = x, g = y, 
                           dependent_variable = t, n = 3)

# initial value problems
ode_function = '-1.2 * y + 7 * exp(-0.3 * t)'
exact_solution = '70/9 * exp(-0.3 * t) - 43/9 * exp(-1.2 * t)'
ivps(ode_equations = [ode_function, exact_solution],
     time_span = [0, 1],
     initial_y = 3,
     steps_stepsize = ['h', 0.12],
     ivp_method = ['Fourth order', None], 
     show_iterations = None, 
     decimal_points = 8)
```

## Support

For any support on any of the functions in this library, send us an email at: stemrelibrary@stemdatascience.com. We are willing to offer the necessary support where we possibly can.

## Roadmap

Future releases aim to make Stemre a full-featured numerical analysis, simulation and data fitting library for learning in STEM (Science, Technology, Engineering and Mathematics).

## Contributing

To make Stemre a successful library while keeping the code easy. We welcome any valuable contributions towards the development and improvement of this library. 

For major changes to the library, please open an issue with us first to discuss what you would like to change and we will be more than willing to make the changes.

## Authors and acknowledgement

We are grateful to the incredible support from our developers at Stem Research.

## License
[MIT](https://choosealicense.com/licenses/mit/)
