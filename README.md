# Firebase Transaction Error: Null or Undefined Snapshot

This repository demonstrates a common error when using Firebase Realtime Database transactions and provides a solution.

## Problem

The issue arises when a transaction callback attempts to access a property of the data snapshot before verifying its existence.  If the data at the specified location is null or undefined, this will throw an error or cause unexpected behavior.

## Solution

The solution involves adding a check to ensure the snapshot exists and has the expected properties before attempting to access them. This prevents errors and makes the code more robust.

## How to reproduce

1.  Set up a Firebase project and initialize the Realtime Database.
2. Clone this repository.
3. Install dependencies (`npm install`)
4. Run `node bug.js` to see the error.
5. Run `node bugSolution.js` to see the corrected code. 