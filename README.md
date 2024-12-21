# Expo Linking API: Deep Link Registration Issue

This repository demonstrates a common issue with the Expo `Linking` API where deep links are not correctly registered, preventing the app from launching when a deep link is tapped.

## Problem

The provided `bug.js` file contains an incorrect implementation of the `Linking.makeUrl` function. This results in the app not correctly registering its URL scheme, thus failing to open deep links.

## Solution

The `bugSolution.js` file provides a corrected implementation that utilizes `Linking.getInitialURLAsync` along with `Linking.addEventListener`. This correctly handles both initial deep links and subsequent ones, ensuring proper deep link functionality.

## Setup

1. Clone the repository.
2. Install dependencies using `npm install`.
3. Run the app using `expo start`.