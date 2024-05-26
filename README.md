# BikeService 

## Overview

The `BikeService` contract is designed to help manage bike maintenance based on the distance traveled. It includes thresholds for minimal service distance, oil and tire replacement, and engine rebore requirements.

## Contract Details

### Variables

- `minDistance`: The minimum distance a bike must travel to require any service (500 units).
- `oilAndTierThreshold`: The distance after which oil and tires should be replaced (2000 units).
- `engineReboreThreshold`: The distance after which the engine should be rebored (4000 units).

### Functions

 **serviceBike(uint256 _distance)**
   - Ensures the bike has traveled at least `minDistance`.
   - If the distance exceeds `oilAndTierThreshold`, it triggers a requirement to replace the oil and tires.

 **checkEngineRebore(uint256 _distance)**
   - If the distance exceeds `engineReboreThreshold`, it indicates that the engine needs to be rebored.

## Usage

- Use `serviceBike` to check if the bike needs an oil and tire replacement based on the distance traveled.
- Use `checkEngineRebore` to determine if the bike's engine needs rebore based on the distance traveled.

The contract ensures proper bike maintenance by setting specific distance-based thresholds for different services.

## License

This project is licensed under the MIT License.

## Author 

Pramod 

pramodmech9148@gmail.com
