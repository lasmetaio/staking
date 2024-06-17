# Lasm Staking Smart Contract

## Overview

The `Staking` contract manages staking, unstaking, and reward claiming functionalities. It allows users to participate in multiple staking schedules, each with its own parameters such as duration, rate, penalty, and allocation. The contract ensures secure token transfers and validates contract interactions. It also allows the owner to update configurations, manage schedules, and rescue tokens.

## Tech Stack

- **Solidity**
- **OpenZeppelin Contracts**
  - `SafeERC20`
  - `Pausable`
  - `ReentrancyGuard`
  - `EnumerableSet`

## Features

- **Staking and Unstaking**: Users can stake tokens into predefined schedules and unstake them with potential penalties.
- **Reward Claiming**: Users can claim rewards based on the staking schedule.
- **Multiple Schedules & Staking Agreements**: Supports multiple staking schedules with unique configurations.
- **Administrative Control**: Update configurations, manage staking schedules, and rescue tokens.
- **Event Notifications**: Emit events for key actions like staking, unstaking, and reward claiming.

## Events

- `VestingClaimContractUpdated`
- `ThresholdForDurationUpdated`
- `ThresholdForRatesUpdated`
- `MinimumStakeAmountUpdated`
- `VestingTokensClaimed`
- `StakingScheduleCreated`
- `StakingScheduleStarted`
- `Staked`
- `Unstaked`
- `ClaimRewards`
- `Withdrawal`

## Security

- **Pausable Functionality**: Allows pausing of contract operations in case of emergency.
- **Reentrancy Protection**: Prevents reentrancy attacks for secure contract interactions.
