# Multiplier2 Circuit Template

This is a Circom circuit template that checks whether the value `c` is the result of multiplying values `a` and `b`. The circuit is built using custom gates for logical operations such as AND, NOT, and OR.

## Circuit Overview

The circuit consists of the following components:

1. `Multiplier2`: The main template that checks the multiplication relationship between inputs `a` and `b`.

2. `NOT`: A template representing a NOT gate, which inverts the input signal.

3. `AND`: A template representing an AND gate, which outputs `1` if both input signals are `1`, otherwise `0`.

4. `OR`: A template representing an OR gate, which outputs `1` if at least one of the input signals is `1`, otherwise `0`.

## Circuit Logic

1. `Multiplier2` template calculates the multiplication result using custom gates:
   - An `AND` gate is used to check whether both inputs `a` and `b` are `1`. The output is stored in signal `x`.
   - A `NOT` gate is used to invert the input `b`. The output is stored in signal `y`.
   - An `OR` gate is used to check whether either `x` (result of AND) or `y` (inverted `b`) is `1`, indicating that the multiplication condition is met. The final result is stored in signal `q`.

## How to Use

1. Install Circom version 2.0.0 or compatible version.

2. Create your own Circom file and include the provided templates and logic as needed for your application.

3. Instantiate the `Multiplier2` template or any other components you need within your Circom file.

4. Compile the Circom file to generate the corresponding circuit and constraints files using the Circom compiler.

5. You can then use the generated circuit and constraints files with a compatible zk-SNARK library to perform zero-knowledge proofs on the circuit's correctness.

## Credits

This project is created by ***[Rajat Verma](https://github.com/thewreckingpanda)***.

## License

This project is licensed under the MIT License. For more details, refer to the [LICENSE](LICENSE) file included in the repository.
