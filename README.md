# Smart Contract Example

This repository contains a simple Solidity smart contract demonstrating the usage of `require()`, `assert()`, and `revert()` statements.

## Table of Contents

- [Introduction](#introduction)
- [Contract Details](#contract-details)
- [Functions](#functions)

## Introduction

This smart contract showcases how to implement `require()`, `assert()`, and `revert()` statements in Solidity. It includes functions that take parameters to trigger different conditions.

## Contract Details

- **Owner**: [OwnerAddress]
- **Initial Value**: 100

## Functions

### `setValue(uint _newValue)`

Allows the owner to set a new value.

### `requireExample(bool condition)`

Demonstrates the usage of `require()`. Takes a boolean `condition` parameter. If `condition` is `false`, it will revert the transaction.

### `assertExample(uint a, uint b)`

Demonstrates the usage of `assert()`. Takes two parameters `a` and `b`. It will trigger an assertion failure if `a` is not equal to `b`.

### `revertExample(uint a, uint b)`

Demonstrates the usage of `revert()`. Takes two parameters `a` and `b`. It will revert the transaction with a specific error message if `a` is not equal to `b`.
