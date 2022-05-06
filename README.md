<div align="center">

  <img width="200" height="auto" src="logo.svg">
  <br>
  <h1>Sherlock Pattern Initiative</h1>
</div>

Umbrella for different diagnostics, symptoms and pattern transformers

# Sherlock Pattern Process

The process consists of three transformers that essentially take a balena device diagnostics file as an input, match it to a set of pattern files that contain symptoms, and then attach the detected patterns to a given thread in Jellyfish. 

![diagram](https://github.com/balena-io-playground/sherlock-pattern-initiative/blob/master/images/block-diagram.png)


## Logfile / Diagnostics translation
Translating diagnostics outputs or logfiles into structured diagnostics JSON files

## Matching / Checking Symptoms for patterns

A symptom parser matches symptom rules (regex, regexmatch, ...) according to [formulajs](https://github.com/formulajs/formulajs) by utilisting the [jellyscript](https://github.com/product-os/jellyfish-jellyscript) parser.
