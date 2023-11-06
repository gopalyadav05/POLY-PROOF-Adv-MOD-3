# ZK SNARK Designer Project 

## Overview
This Project provides the "Multiplier2" circuit  implemented in Pragma Circom 2.0.0. The circuit is designed to check if the output signal `Q` is the result of multiplying two input signals, `a` and `b`. Pragma Circom is a domain-specific language for specifying and verifying cryptographic circuits.

## Circuit Description
The "Multiplier2" circuit consists of three sub-components: `AND`, `NOT`, and `OR` gates, which are combined to check if the output signal `Q` correctly represents the multiplication of `a` and `b`. Here's a breakdown of the circuit structure:

### Circuit Signals 
- Input signals:
  - `a`: First input signal
  - `b`: Second input signal
- Intermediate signals:
  - `x`: Intermediate signal to store the result of the AND operation between `a` and `b`
  - `y`: Intermediate signal to store the result of the NOT operation on `b`
- Output signal:
  - `Q`: Output signal representing the result of the multiplication of `a` and `b`

The `Multiplier2` template combines these signals using sub-components to ensure that `Q` is the correct product of `a` and `b.

### Sub-components
#### AND Template
- Input signals:
  - `a`: First input signal
  - `b`: Second input signal
- Output signal:
  - `out`: Output signal representing the result of the AND operation between `a` and `b`

#### NOT Template
- Input signal:
  - `in`: Input signal to be negated
- Output signal:
  - `out`: Output signal representing the result of the NOT operation on `in`

#### OR Template
- Input signals:
  - `a`: First input signal
  - `b`: Second input signal
- Output signal:
  - `out`: Output signal representing the result of the OR operation between `a` and `b`

The sub-components are used to implement the logic of the `Multiplier2` template.

## Usage
To use this circuit in your Pragma Circom 2.0.0 project, follow these steps:

1. Include the circuit template in your Pragma Circom project.

2. Define the input signals `a` and `b` for the `Multiplier2` template.

3. Connect the `main` component to the `Multiplier2` template.

4. Compile your Pragma Circom project to generate the circuit.

5. Use the generated circuit for cryptographic or verification purposes, such as proving that `Q` is the correct result of multiplying `a` and `b.
## Author 
- Gopal Yadav
  
## License
This circuit is Under MIT License 
