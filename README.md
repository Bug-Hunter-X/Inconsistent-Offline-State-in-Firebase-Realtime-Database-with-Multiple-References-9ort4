# Inconsistent Offline State in Firebase Realtime Database

This repository demonstrates a bug where the Firebase Realtime Database incorrectly reports an offline state even when the client is connected to the internet. This occurs specifically when using multiple database references simultaneously.  The problem stems from inconsistencies in how each reference manages its connection state.

## Problem
Multiple database references can lead to a situation where one reference correctly reflects the online status, while another reports offline.  This inconsistency can cause unexpected application behavior and disruptions.

## Solution
The solution involves ensuring consistent connection management by using a single database instance and centralizing connection state checks.

## Steps to Reproduce
1. Clone this repository.
2. Install dependencies using `npm install`.
3. Run the `bug.js` file. Observe the erratic offline/online reporting.
4. Run the `bugSolution.js` file. Observe the consistent online status.

## Contributing
Contributions are welcome!